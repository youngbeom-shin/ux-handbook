---
layout: handbook-page-toc
title: "流水线执行的用户体验"
description: "关于流水线执行用户体验团队的做法、目标、成就和计划的文件。"
---


## 概述

[Verify:Pipeline Execution Group](https://about.gitlab.com/handbook/engineering/development/ops/verify/pipeline-execution/) 专注于与流水线执行有关的所有功能，作为 [GitLab 持续集成](https://about.gitlab.com/stages-devops-lifecycle/continuous-integration/) 的一部分，这个用户体验团队负责以下类别的工作：

- **[持续集成](https://about.gitlab.com/direction/verify/continuous_integration/)**: 使流水线易于运行是我们的首要重点，这适用于手动运行流水线以及在提交代码提交或合并请求时自动触发流水线。此外，我们希望提供数据来检查流水线的性能，这样你就可以优化 CI 配置，使你的流水线更有效地运行。
- [**持续集成扩展**](https://about.gitlab.com/direction/verify/continuous_integration_scaling/): 在22财年，我们致力于实现 SaaS 优先。在验证阶段，这意味着要优先考虑持续集成的规模，并确保我们在 GitLab.com 上的用户使用可靠和可用的服务。
- [**合并队列**](https://about.gitlab.com/direction/verify/merge_trains/): 合并队列是一个排队的合并请求列表，等待被合并到目标分支。每个合并请求中的修改都与先前的合并请求中的修改相结合，并在合并前进行测试。

## 流水线执行 UX 计划

### 流水线执行下的类别愿景
- **[持续集成](https://about.gitlab.com/direction/verify/continuous_integration/)**: 展望未来，我们有计划帮助你更好地监测和了解你的流水线 [epic#4794](https://gitlab.com/groups/gitlab-org/-/epics/4794). 拥有流水线活动的细节（如工作持续时间）将使你在流水线运行时看到正在发生的事情并作出反应。除了将数据简单地用于反应目的外，我们还计划为历史流水线分析提供一个可定制的用户界面，这样你就可以看到指导你规划和决策的趋势。 我们也很想创建一个整体的方法，通过 [gitlab#325529](https://gitlab.com/gitlab-org/gitlab/-/issues/325529) 在流水线成功时自动合并，这在[代码审查](https://about.gitlab.com/direction/create/code_review/)和持续集成之间提供了很好的协作。 
- [**合并队列**](https://about.gitlab.com/direction/verify/merge_trains/): 我们的首要愿景项目是[合并队列应支持快进合并](https://gitlab.com/gitlab-org/gitlab/issues/35628)，因为这将消除经常需要手动重新设置的情况。我们从许多开发人员那里听说，他们每天的大部分时间都用于这项活动，有了这项功能，合并队列将为他们解决这个问题。

### 正在进行的倡议

在22财年第三季度，我们专注于简化合并策略，以及改善与上述类别相关的各种功能的整体可用性。

- [14.3 Pipeline Execution UX tracking issue](https://gitlab.com/gitlab-org/gitlab/-/issues/335073)
- [14.4 Pipeline Execution UX tracking issue](https://gitlab.com/gitlab-org/gitlab/-/issues/337486)
- [14.5 Pipeline Execution UX tracking issue](https://gitlab.com/gitlab-org/gitlab/-/issues/336562)

## 我们如何工作

### 用户体验和研发团队的合作

产品经理和产品设计师使用 [流水线执行设计跟踪史诗](https://gitlab.com/groups/gitlab-org/-/epics/5866) 和定期同步来跟踪准备进行设计的议题，通常与一个季度的主题一致。

在流水线执行组中，设计工作领先于开发。因此，设计者正在处理的问题只有在加入设计建议后才会被分配到一个里程碑，并且状态从 `workflow::design` 转移到 `workflow::planning breakdown`。

我们在每个里程碑中拿出~10%的生产能力（按权重计算）来处理 [UX 债务](https://about.gitlab.com/handbook/engineering/ux/performance-indicators/#ux-debt)议题，并在其 SLO 中解决这些议题。在 [流水线执行组页面](https://about.gitlab.com/handbook/engineering/development/ops/verify/pipeline-execution/#collaboration-with-ux-and-engineering) 上阅读更多关于用户体验和研发团队之间的合作。

### 用户体验定义的完成（DoD）

我们使用 [CI/CD UX Definition of Done (DoD)](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/ci-cd/#ux-definition-of-done-dod) 作为评估议题准备情况的工具，并跟踪预期的交付物、目标和批准过程。

### UX 权重

我们使用 [UX 权重定义](https://about.gitlab.com/handbook/engineering/ux/product-designer/#ux-weight-definitions) 来表示里程碑的生产能力。

### UX 债务和 UI 优化议题

CI 的 ~UX 债务和 ~UI 优化议题在[本史诗](https://gitlab.com/groups/gitlab-org/-/epics/4667)中被追踪。我们的目标是在每个里程碑中至少处理其中一个问题。

## 跨阶段的合作

| 议题 | 范围 | 受影响的阶段性群组 |
|-------|-------|-----------------------|
| [Simplify merge strategies with `Auto merge`](https://gitlab.com/groups/gitlab-org/-/epics/6687) | Merge Widget, Settings Page | `group::source code` `group::code review` |
| [Regular Merge button shows up when merge trains is enabled and pipeline for MR is waiting on a manual action](https://gitlab.com/gitlab-org/gitlab/-/issues/300663) | Merge widget | `group::code review` |
| [Remove duplicate status indicators on pipeline index page](https://gitlab.com/gitlab-org/gitlab/-/issues/338192) | Pipeline Index Page, Pipeline Mini-graph | `group::pipeline authoring` |
| [Support allow merging of MR when Pipeline must succeed is enabled in absence of pipeline](https://gitlab.com/gitlab-org/gitlab/-/issues/334281) | Merge widget | `group::source code` `group::code review` |
| [New MR widget to catch CI jobs' duration regression before and MR is merged into the main branch](https://gitlab.com/gitlab-org/gitlab/-/issues/342517) | Merge widget | `group::source code` `group::code review` |
