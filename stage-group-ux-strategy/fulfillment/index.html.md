---
layout: handbook-page-toc
title: Fulfillment 用户体验团队
description: "Fulfillment 用户体验团队支持 Fulfillment 部门为客户提供购买、升级和更新 GitLab 的良好体验。"
---

## 概述



## 用户体验团队成员

- [Jacki Bauer](https://about.gitlab.com/company/team/#jackib) ([Jacki's ReadMe](https://gitlab.com/jackib/jacki-bauer/blob/master/README.md)) - 用户体验经理
- [Tim Noah](https://about.gitlab.com/company/team/#timnoah) - 高级产品设计师, 许可证
- [Emily Sybrant](https://about.gitlab.com/company/team/#esybrant) - 产品设计师, 购买
- [Matthew Nearants](https://about.gitlab.com/company/team/#mnearents) - 高级产品设计师, 使用量


## 我们如何工作

我们遵循手册中[产品设计部分](https://about.gitlab.com/handbook/engineering/ux/product-designer/)描述的[产品设计师工作流程](https://about.gitlab.com/handbook/engineering/ux/ux-research/)和[用户体验研究员工作流程](https://about.gitlab.com/handbook/engineering/ux/research/)。作为 Growth 设计师，我们坚持不懈地按照[实验工作流程](https://about.gitlab.com/handbook/engineering/development/growth/experimentation/)测量我们的设计变化的影响。此外。

- 我们有议题看板，所以我们可以看到每个人都在做什么。
- 我们用 UX、devops::fulfillment、section::fulfillment 和group:: 来**标注**我们的议题。
- 我们使用[工作流标签](https://gitlab.com/groups/gitlab-org/-/labels?utf8=%E2%9C%93&subscribed=&search=workflow%3A%3A)。
- 我们使用**里程碑**来帮助规划和确定优先次序。
- 我们使用[用户体验议题权重](https://about.gitlab.com/handbook/engineering/ux/product-designer/#ux-issue-weights)。
- 我们为用户体验工作创建单独的议题，并以 [UX] 为前缀命名。这允许产品设计师增加一个专门针对 UX 的议题权重。我们倾向于将设计和设计反馈保留在 [UX] 议题中，以使其清晰明了。


#### 为设计做好工作准备

我们使用产品开发流程来帮助解决产品生命周期中的问题。在设计阶段，以下内容是重要的:

- [ ] 问题已被充分理解，并已得到验证
- [ ] JTBD 已被充分理解并得到验证
- [ ] PM 已经将机会画布传达给稳定的同行和集团利益相关者，包括产品设计师和产品设计经理。

[链接到议题模板](https://gitlab.com/gitlab-org/gitlab/-/issues/new?issue%5Bmilestone_id%5D=#)

模板也可以复制到主要议题，即唯一可信源(SSOT)。

#### 确定工作的优先次序 

| 类型                         | 占里程碑的百分比 | 描述                                                                                    |
|------------------------------|----------------|-------------------------------------------------------------------------------------------------|
| 可交付的成果                  | 65%            | 业务优先级，包括设计和解决方案验证                                    |
| 积极的用户体验和测量 | 25%            | 对未来的改进进行研究和构思，CM记分卡，竞争性评估的修复      |
| 用户体验部的优先事项     | 5%             | Pajamas, 用户体验 OKR, 专业发展                                                      |
| 其他                       | 5%             | 挑选设计师，参加公司范围内的会议，行政任务，专业发展 |


#### 协作 

Fulfillment 组之间有很多重叠，所以我们的工作非常紧密。为了使事情简单明了，我们遵循 [GitLab 内部沟通](https://about.gitlab.com/handbook/communication/internal-communications) 准则。此外，下面的提示将使我们更容易与跨越多个小组的产品设计师合作。

- 沟通过度总比沟通不足好，特别是在这种情况下。
    - 清楚和透明地传达优先级。通过优先级标签（即~"milestone::p1""）、到期日和议题看板沟通用户体验优先级，而不是在1:1文档或Slack频道中。
    - 欢迎在多个渠道（GitLab + Slack + email）中与设计师联系。覆盖多个阶段的小组时，很容易错过一些东西。
- 在我们的月度计划一体上，每个设计师都应该指出其他团队的高优先级或耗时的议题。另一个规划一体的链接也很好，这样用户体验经理和产品经理就可以很容易地导航到这个信息。
- 减少会议:跨阶段小组的设计师的会议次数是单阶段小组的设计师的2-3倍，所以他们的团队可以帮助他们，确保我们遵循 GitLab 的异步会议实践，让他们错过这些会议而不会产生负面后果。

#### 沟通截止日期

我们处理工作的顺序可能很复杂，因为我们有优先级和严重级别，有里程碑计划，产品设计团队也有他们自己的[选择下一个工作的指导](https://about.gitlab.com/handbook/engineering/ux/product-designer/#priority-for-ux-issues)。此外，有些用户体验问题需要在里程碑中比其他问题更早交付。为了帮助沟通，你可以使用截止日期字段。作为一名项目管理人员，如果你选择这条路线，请做好以下工作：

- 继续使用优先级标签和议题权重。截止日期并不能代替这些。
- 添加一个议题评论，附上建议截止日期，并提及产品设计师。
- 产品设计师应在一天内答复该截止日期是否可行。如果截止日期可行，产品设计师将添加截止日期。如果不可行，他们将提供折衷方案供 PM 考虑。
- 如果截止日期发生变化，请在议题中发表评论，并@提及将受到影响的人。请注意，截止日期的变化不会引发通知。
- 当变化通过Slack或1:1沟通时，更新该议题，以便其他人可以看到变化。考虑在同步会议上分享。

#### 对 MR 的视觉审查

工程团队将 `UX` 标签用于任何引入视觉、交互或流程变化的 MR。这些 MR 可以与新议题、bug、后续工作或任何类型的 MR 有关。如果工程师不确定 MR 是否需要 UX，他们应该咨询从事相关议题的设计师，或分配给该阶段组的设计师，或 UX 经理。

任何带有 `UX` 标签的 MR 都需要视觉审查。当 MR 处于 `workflow::In review` 时，工程师会使用侧边栏的[reviewer 功能](https://docs.gitlab.com/ee/development/code_review.html#getting-your-merge-request-reviewed-approved-and-merged)将 MR 分配给设计师进行视觉审查。这可以与维护者审查同时进行，但设计者应该优先考虑这些审查，尽快完成。

有些时候，设计师不可能通过 Review Apps 或 GDK 来完成他们的视觉审查，也不现实。在这些时候，设计师和工程师应该协调一个演示。


### 记录交易流程

当处理与新购买、更新、升级和试用相关的交易议题时，将流程分解成几个部分会有所帮助。这种解决议题的方法使产品设计师能够以一种易于理解的方式记录用户旅程的开始和结束。

- 切入点：用户互动的最初接触点。(例如：页面、CTA 或表单等)
- 决定：给予用户决定产品、选项或套餐的能力。
- 确认：购买成功或不成功的总结。

每个步骤不一定需要，也不一定是线性的。例如，一个切入点也可能是用户选择产品的一个点（决定）。

我们已经记录了 [Figma 中的 Fulfillment 用户流程](https://www.figma.com/file/DCq7K8Srsv79tbH1yRkGbl/Document-user-flows-%5Bgitlab-org%2F-%2Fepics%2F3603%5D?node-id=0%3A1)。这些反映了目前生产环境中的情况。产品设计师负责在他们的工作发布后更新这些用户流。
