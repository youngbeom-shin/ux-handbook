---
layout: handbook-page-toc
title: "Data for Design Decisions"
description: "Guide on tools used within GitLab to find the data to support design decisions."
---

#### On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## 在GitLab使用数据进行设计决策

数据是GitLab的设计师和研究人员了解用户行为的另一种方式。分析可以为整个产品开发流程提供有价值的输入。通过使用数据，我们可以了解和量化我们所运送的迭代的影响。

我们不应该完全依赖数据来做决定，但它应该是决策的一个重要输入。

{%youtube%}J-USG9BKH-g{%endyoutube%}

## 将假设与影响结合起来

设计过程的一部分是要有一个[强势假设](https:about.gitlab.com/handbook/engineering/ux/ux-research-training/write-strong-hypothesis/)来指导我们的工作。

理想情况下，假设将以用户研究的信息为基础

例如：

> 我们相信，以`一种便于负责事件管理的工程师访问的方式`，存储关于`事件如何解决`、`解决了多长时间以及结果是什么`的信息，将实现`事件解决时间加快20%`。

以下是利用数据了解 `事件解决时间加快20%`是否实现的可能方法：

- 测量用户旅程中两个步骤之间的时间
- 测量用于解决的总时间
- 进行A/B测试，比较两种解决方案

这些数据点在解决方案的验证过程中很难获得，但在测量时，它们有助于连接从研究、迭代到影响的点。

通过观察和测量，它应该引发进一步的问题，以帮助在未来产生更多可能的迭代。

## 如何采集数据

为了生成报告和仪表盘，我们使用了一个名为[Sisense](https://app.periscopedata.com/app/gitlab/403199/Welcome-Dashboard-%F0%9F%91%8B)的第三方工具来可视化所捕获的数据。

数据源决定了Sisense查询中使用的表名。从产品的角度来看，我们有三个主要的数据源：usageping、产品数据库和Snowplow。

**我们的目标是分析产品的使用情况。而不是为了追踪个别用户**。这意味着在前端我们尊重浏览器的 "不跟踪 "设置，并允许选择退出使用usage ping。除此之外，产品智能团队还负责数据的假名化，以便不保存个人身份信息。这个[视频强调了Snowplow、usage ping和假名化是如何一起工作的]（https://www.youtube.com/watch?v=awWhNtwuVNs）。

### 数据来源概述

- **Usage Ping** (针对 Self-Managed 和 GitLab.com)
    - 一个定制的GitLab工具，从我们的客户那里收集汇总信息，这些客户在他们自己的硬件上托管我们的产品。
    - 视频: [Usage Ping Workshop](https://www.youtube.com/watch?v=D4eGDbpIY5c)
    - 何时使用的举例：
        - 议题总数
        - 不同用户产生议题的数量
        - 实例设置- Git版本，数据库版本
        - 启用功能的数量
        - 在代码片段上创建内容的数量
        - 合并请求中的注释数量
- **GitLab.com Postgres 数据库** (针对 GitLab.com)
- **Snowplow** (针对 GitLab.com)
    - 捕获客户端/服务器端的事件和页面视图
    - 视频: [Snowplow 2.0 Workshop](https://www.youtube.com/watch?v=CaxhdskjWvg)
    - [查看事件的工具](https://docs.gitlab.com/13.12/ee/development/snowplow/#developing-and-testing-snowplow) 用于探索/测试

[GitLab的《产品经理的关键数据源》](https://about.gitlab.com/handbook/business-technology/data-team/programs/data-for-product-managers/#key-data-sources-for-product-managers-at-gitlab)详细介绍了每个数据源的使用和查询方式。

这些可视化的东西将帮助你了解这些系统是如何一起工作的。

- [简化图](https://about.gitlab.com/handbook/product/product-intelligence-guide/#systems-overview)显示了GitLab Inc和自我管理实例之间的相互作用。
- [数据平台的数据栈](https://about.gitlab.com/handbook/business-technology/data-team/platform/#our-data-stack)的详细图示。

## 使用数据进行设计决策的例子

下面的议题和合并请求是我们如何利用数据进行决策的例子。

-  [增加基于Snowplow的事件跟踪，以查看用户扩展单元测试报告MR小工具的频率](https://gitlab.com/gitlab-org/gitlab/-/merge_requests/46048)
- [左侧边栏和顶部导航的交互](https://gitlab.com/gitlab-data/analytics/-/issues/5357#note_596307748)
- [设置了多少用户来批准多个规则](https://gitlab.com/gitlab-data/analytics/-/issues/10862)
- [在textarea和input之间进行选择](https://gitlab.com/gitlab-org/gitlab/-/merge_requests/73506#note_722625421)
- [在设计中标准化设备宽度](https://gitlab.com/gitlab-org/gitlab-design/-/issues/1634)

## 常见问题

- **我可以向谁寻求数据帮助？**如果你有任何关于数据或Sisense的具体问题，你可以在Slack上以`#data`与他们联系。
- **当没有基准指标来衡量时，该怎么办？**当没有基准指标时，使用一个月的追踪数据的结果来作为基准。

## 资源

- [为产品经理提供的数据](https://about.gitlab.com/handbook/business-technology/data-team/programs/data-for-product-managers/)
- [Snowplow 命名规则](https://gitlab.com/gitlab-org/gitlab/-/blob/master/.gitlab/issue_templates/Snowplow%20event%20tracking.md)
- [Snowplow at GitLab](https://docs.gitlab.com/ee/development/snowplow/index.html)
- [Snowplow Inspector Chrome 插件](https://docs.gitlab.com/ee/development/snowplow/index.html)
- [来自docs.gitlab.com的SQL参考示例](https://docs.gitlab.com/ee/development/snowplow/index.html#reference-sql)
- [实验设计与分析](https://about.gitlab.com/handbook/product/product-analysis/experimentation/)
- [增长实验知识库](https://about.gitlab.com/direction/growth/#growth-experiments-knowledge-base)
