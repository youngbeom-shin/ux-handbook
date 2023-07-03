---
layout: handbook-page-toc
title: "寻找SaaS用户"
description: "我们如何锁定满足特定标准的研究参与者"
---


## 寻找SaaS（GitLab.com）用户

### 何时在数据仓库中寻找用户

我们有多种方法来识别和[为研究招募参与者](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/recruiting-participants)，包括我们的[First Look用户小组](https://about.gitlab.com/community/gitlab-first-look/)和通过社交媒体招募。然而，在有些情况下，这些方法并不适合，你需要能够根据客观的使用数据而不是自我报告或推断的数据支持的非常具体的标准来寻找用户。做到这一点的最好方法是利用我们的数据仓库中的使用和人口数据。

**在通过数据仓库寻找用户的时候，有一个非详尽的例子。**

* 你正在寻找对某一功能或阶段有一定使用量的用户，而不仅仅是某一阶段的用户
* 你正在寻找与 GitLab上 某一特定类型的对象或内容（例如：史诗、代码片段、wiki等）有过互动的用户。
* 你需要了解用户所在的组或项目的大背景（例如：用户少于30人的组中的用户、premium计划组中的用户、没有使用仓库的项目中的用户）。

### 前提条件

1. 使用结构化查询语言(Structured query Language, SQL)查询数据仓库。在网络上有无数免费的学习 SQL 的指南。SQL 有许多不同的风格，我们使用的是[Snowflake](https://docs.snowflake.com/en/index.html)。然而，在 SQL 的主要变体中，大多数基本功能是一致的，所以您不需要寻找特定于 snowflake 的具体功能.
1. 为了查询数据仓库，您需要[编辑访问](https://about.gitlab.com/handbook/business-ops/data-team/platform/periscope/#editor-access)Sisense(之前是 Periscope)。这需要完成一个[访问请求](https://about.gitlab.com/handbook/business-ops/team-member-enablement/onboarding-access-requests/access-requests/)。
1. [产品经理的数据](https://about.gitlab.com/handbook/business-ops/data-team/programs/data-for-product-managers/)概述了如何访问 Sisense 中的 SQL 资源管理器，你将在那里编写和执行你的查询，并提供了一个关于仓库结构的高层次视图。
1. 数据团队[记录各个数据仓库表](https://dbt.gitlabdata.com/#!/overview)使用一个叫做 dbt 的工具。有些表的记录比较好，包含了不同列的目的描述和解释，而遗憾的是有些却没有。然而，文档确实会随着时间的推移而改进。

### SaaS专用表

我们的数据仓库包含各种不同领域的数据。就我们的目的而言，我们对详细说明用户信息和 GitLab.com（SaaS）使用情况的数据感兴趣。

大多数存放 SaaS 相关数据的表都使用前缀`gitlab_dotcom_*`，但不是全部。一个很好的起点是探索使用此前缀的不同表，并查看它们包含哪些数据。

### 用户表

我们的 SaaS 总体用户表是`gitlab_dotcom_users_xf`。它包含了个人用户的最完整情况，包括账户创建日期、活跃天数、角色和最高付费计划（如果有）等信息。该表中的 `user_id` 变量是 [GitLab.com](http://gitlab.com) 用户的主要标识符，并在其他表中用于识别与记录相关的用户。例如， `gitlab_dotcom_merge_requests_xf` 表包含了在 GitLab.com 上创建的 MR 的记录，并包含一个名为 `author_id` 的列，用来识别特定 MR 的作者。这个  "author_id " 是 GitLab.com 的用户 ID，你可以用这个 "user_id" 变量将合并请求的作者与用户表（或任何其他表）的记录联系起来。

你可以使用这个表来查找在过去七天内创建账户的100个用户的用户id:

```sql
SELECT user_id FROM analytics.gitlab_dotcom_users_xf
WHERE account_age >= 7
LIMIT 100
```

### 对象表(项目、议题、合并请求等)

我们有一个表，其中包含了 GitLab 中所有 "顶级 "对象的记录，还有其他的。

* 项目
* 群组
* 议题
* 合并请求
* 史诗

如果你能在 GitLab.com 上创建它，可能会有一个表格。这些表遵循与其他SaaS表相同的结构。例如:

- `gitlab_dotcom_issues_xf`
- `gitlab_dotcom_epics_xf`
- `gitlab_dotcom_merge_requests_xf`

这些表格中的记录不是完全保真的。它们可能不包括对象在界面中呈现时的所有数据。当你在GitLab.com用户界面上加载一个问题时，你会看到评论和各种元数据。这些数据中的大部分不会在仓库中的问题表中找到，它们要么无法访问，要么存储在单独的表格中，以保持表格的合理大小。此外，我们不会在仓库中公开那些本来属于隐私的数据。例如，虽然你可以看到GitLab.com上公开的问题的标题和描述（就像你在网上查看它们一样），但你将无法看到非公开问题的这些信息。

当你想了解一个用户或一个团体创造了多少东西或与之互动时，或者你想从某种类型的实体（例如，一个被提升为史诗的议题）开始，然后看看哪些用户与这样的实体进行了互动，这些表格就很好。这些表格不提供事件级别的数据，所以你不一定能知道用户何时或如何创建或互动的，只是知道他们做了（或没有）。

比如说。你在研究议题的权重，你想找到 100 个在过去 30 天内创建了一个有权重的议题的用户的用户 ID。你还需要知道他们在这段时间内创建了多少个议题。你可以使用这个查询。

```sql
SELECT
  author_id,
  COUNT(1) as num_issues
FROM analytics.gitlab_dotcom_issues_xf
WHERE
  weight IS NOT NULL
  AND issue_created_at >= DATEADD(day, -30, current_timestamp)
GROUP BY 1
LIMIT 100
```

### 阶段组月度活跃用户

我们不在具体的事件记录中记录用户 ID，所以你无法准确地找到某个用户何时完成了某个特定的行动。然而，我们确实记录了用户每月与不同的高级功能和阶段互动的次数和天数。`gitlab_dotcom_monthly_stage_active_users` 表. 表格当你在寻找某些功能或阶段的“轻”或“重”用户时，或者当你想确保你的用户至少在某个阶段使用了最少的时间时，这是一个很好的标准。

比如说。你需要找到 50 个与 CI 流水线互动至少 17 次或在某月的 9 个不同日子（或更准确地说，某月的最后 28 天）的用户 ID。

```sql
SELECT user_id
FROM analytics.gitlab_dotcom_monthly_stage_active_users
WHERE
	event_name='ci_pipelines'
	AND (event_count >= 17 OR event_day_count >= 9)
	AND smau_month='2020-04-01'
LIMIT 50
```

### 如何获得帮助

* 对于在哪里可以找到仓库中的某些数据的问题，Slack上的#data频道可以解决这些问题。
* 如果你是用户体验研究员或协调员，有SQL问题，请联系Slack上的[Jeff Crow](https://gitlab.com/jeffcrow)。
