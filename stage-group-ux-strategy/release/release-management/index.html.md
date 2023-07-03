---
layout: handbook-page-toc
title: "发布管理用户体验"
description: "发布管理用户体验团队专注于为所有与持续交付和发布自动化相关的功能创造愉悦的体验。"
---

## 概述

[发布管理小组](https://about.gitlab.com/handbook/product/categories/#release-management-group)专注于持续交付和发布自动化方面的所有功能。

- [Release Orchestration 产品方向](https://about.gitlab.com/direction/release/release_orchestration/) (viable)
- [Release Evidence 产品方向](https://about.gitlab.com/direction/release/release_evidence/) (minimal)
- [Secrets Management 产品方向](https://about.gitlab.com/direction/release/secrets_management/) (minimal)
- [Pages 产品方向](https://about.gitlab.com/direction/release/pages/) (complete)

### 了解更多

- 关于我们的用户体验愿景和战略，请看[发布用户体验战略](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/release/).
- 关于产品的愿景和使命，请看[发布:发布管理小组](https://about.gitlab.com/handbook/engineering/development/ops/release/release-management/)页面。
- 要了解 Ops 阶段的内容，请查看[产品愿景](https://about.gitlab.com/direction/ops/#release)。

你也可以联系发布管理 Slack 频道`#g_release-management`。

## 用户体验愿景图 - 下一步是什么

我们正在努力增加发布管理功能的深度和丰富性，以支持我们的愿景，即允许用户从任何他们想要的 API、YAML 和 UI 来计划和协调发布。我们的下一个大项目是:

- 3年愿景 mockups ([gitlab&3825](https://gitlab.com/groups/gitlab-org/-/epics/3825))
- GitLab 运行手册 ([gitlab&4218](https://gitlab.com/groups/gitlab-org/-/epics/4218))
- 高级部署冻结 ([gitlab&2884](https://gitlab.com/groups/gitlab-org/-/epics/2884))
- 在 GitLab 中测量 DORA 4 指标 ([gitlab&4358](https://gitlab.com/groups/gitlab-org/-/epics/4358))
- 发布 <> 群组里程碑 ([gitlab&4362](https://gitlab.com/groups/gitlab-org/-/epics/4362))
    - 将群组里程碑与版本联系起来 ([gitlab#121476](https://gitlab.com/gitlab-org/gitlab/-/issues/121476))
- 跨项目共享生产环境 ([gitlab&4276](https://gitlab.com/groups/gitlab-org/-/epics/4276))
- 获取和配置 Secrets ([gitlab&2875](https://gitlab.com/groups/gitlab-org/-/epics/2875))
    - 在 UI 中定义 Vault credential ([gitlab#218677](https://gitlab.com/gitlab-org/gitlab/-/issues/218677))
- 从 CI/CD 变量中分离 secrets ([gitlab#217355](https://gitlab.com/gitlab-org/gitlab/-/issues/217355))

我们也在不断研究如何通过以下举措改善 GitLab 发布的整体用户体验：

- 发布的可用性 ([gitlab&2355](https://gitlab.com/groups/gitlab-org/-/epics/2355))
- 改善环境 ([gitlab&3293](https://gitlab.com/groups/gitlab-org/-/epics/3293))
- 发布管理 UX 债务和 UI 优化 ([gitlab&3416](https://gitlab.com/groups/gitlab-org/-/epics/3416))

## 我们的客户

发布管理的产品愿景已变得更加专注于为 GitLab 的发布协调和部署跟踪提供高级管理功能。这是为了建立在我们在 GitLab 拥有的数据资产上，这些数据资产始于用户购买 GitLab 以持续集成的方式快速构建产品。我们将通过帮助他们协调和大规模部署来扩展这一旅程。

今天，使用 Kubernetes 部署的单存储库项目能够充分利用我们的产品。我们的目标客户需要跨多个团队和小组进行协调才能成功部署。受监管的行业是我们产品的最大受益者。

### 竞争分析

查看全部 [发布管理竞争分析](https://gitlab.com/groups/gitlab-org/-/epics/2622)。

## 我们的 Jobs To Be Done (JTBD)

查看全部 [发布阶段 JTBD](https://about.gitlab.com/handbook/engineering/development/ops/release/jtbd/)。

## 我们如何工作

- 我们使用 [**UX Planning epic**](https://gitlab.com/groups/gitlab-org/-/epics/2439) 来收集需要 UX 审查的议题。因为这些议题是在 `workflow:design` 中，它们不需要分配一个里程碑，大部分被分配到 `Backlog`。UX 和 PM 会在我们的1:1、ThinkBig！会议，以及其他同步和非同步的方法中讨论这些的范围和优先级。一旦设计方案被添加到议题描述中（SSOT），我们就会把它从史诗中移除，并按照[研发工作流程阶段](https://about.gitlab.com/handbook/engineering/development/ops/release/release-management/#workflow-stages)进入下一个步骤。
- 我们以持续的看板方式工作，同时仍然与里程碑保持一致。请参阅[发布管理计划工作流程](https://about.gitlab.com/handbook/engineering/development/ops/release/release-management/planning.html)。
- 我们用 `UX`、`devops::release` 和 `group::release-management` 来**标注**我们的议题。
- PM 将根据研发能力和交付优先级将 UX-ready 议题分配到一个特定的里程碑。
- 在将议题转移到 `workflow:design` 之前，PM 将对议题进行范围划分，并标注 `workflow:ready for design`。
- 我们通过审查标有 `UX` 的 MR，创建后续问题，并随着交付范围的变化更新SSOT，来支持正在某个特定里程碑上进行的研发议题。
  - 查看 [所有标有 P1 标签的与发布相关的 UX 议题](https://gitlab.com/groups/gitlab-org/-/boards/1488065?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=cicd%3A%3Aactive&label_name[]=group%3A%3Arelease%20management&label_name[]=Release%3A%3AP1&label_name[]=UX).

### 用户体验对 "完成" 的定义 (DoD)

> 这是我们在 12.10 中启动的一个试验过程--[release-management#21](https://gitlab.com/gitlab-org/ci-cd/release-management-group/release-management/-/issues/21)。在 [release-management#40](https://gitlab.com/gitlab-org/ci-cd/release-management-group/release-management/-/issues/40#note_430976408) 中进行迭代。

产品设计师与产品经理一起，将 DoD 应用于史诗，以便更好地分解设计工作，让同行更好地了解在 MVC 进入开发阶段之前，需要完成设计工作流程的哪些步骤。

```
### 用户体验对 "完成 "的定义

- [ ] 问题已被验证
- [ ] 问题已经准备好进入~“workflow::ready for design” 阶段
- [ ] 已经创建了 MVC 的用户故事和验收标准
  - 提醒：考虑每个用户故事的边缘案例
- [ ] 已经确定了跨团队依赖关系(如果适用的话)
- [ ] 为每个用户故事创建了 Prototype 或 mockup
- [ ] 解决方案已被验证
- [ ] Pajamas
    - [ ] UI组件设计已被确定
    - [ ] Pajamas 议题被创建（新的工作流程）
- [ ] 如果修改涉及到文案，~ "Technical Writing" 和~ "UI text" 的标签已被添加。
- [ ] MVC 的 SSOT 已被更新，并被标记为~"workflow::ready for development"

```

[查看 CI/CD 阶段组中的其他设计师如何使用 UX DoD](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/ci-cd/#definition-of-done-for-ux-pilot)

### 用户体验和研发合作

我们与研发团队紧密合作，对发布管理功能的设计进行构思、完善、审查和迭代。产品设计师的职责包括：

- 在议题准备开发之前，提供[指导和促进设计讨论](https://about.gitlab.com/handbook/engineering/ux/product-designer/#product-design-process)。
- 尽可能严格遵守[MR审查指南](https://about.gitlab.com/handbook/engineering/ux/product-designer/mr-reviews/)，以减少对速度的影响，同时保持质量.
- 通过确保影响用户体验但在开发阶段未被产品设计师验证的变化作为 `UX debt` 进行跟踪，来消除研发团队的障碍。

在 Unfiltered 上观看。[前端/UX MR审查过程。我们可以在未来改进什么？](https://www.youtube.com/watch?v=aqRolFLULzE)

## 绩效指标

### UX 债务

**Chart** ([Sisense↗](https://app.periscopedata.com/app/gitlab/641753/UX-Debt?widget=8474988&udv=0))

<embed width="100%" height="350" src="<%= signed_periscope_url(dashboard: 641753, chart: 8474996, embed: 'v2') %>">

**Chart** ([Sisense↗](https://app.periscopedata.com/app/gitlab/641753/UX-Debt?widget=8474991&udv=0))

<embed width="100%" height="350" src="<%= signed_periscope_url(dashboard: 641753, chart: 8474998, embed: 'v2') %>">

- 在 UX 部门绩效指标页面 [了解更多关于 UX 债务](https://about.gitlab.com/handbook/engineering/ux/performance-indicators/#ux-debt)
- [发布管理团队 UX 债务议题](https://gitlab.com/gitlab-org/gitlab/-/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=UX%20debt&label_name[]=group%3A%3Arelease%20management)

## 关注我们的工作

我们的[发布(CD) UX YouTube 频道](https://www.youtube.com/playlist?list=PL05JrBw4t0KoyqCjN4f79w0dYZusHLx15)包括 UX 记分卡演练，UX 审查，小组反馈会议，团队会议，以及更多内容。
