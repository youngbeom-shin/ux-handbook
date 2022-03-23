---
layout: handbook-page-toc
title: "GitLab 的战略研究"
---

### 什么是战略研究?

用户体验已经改变了产品管理部门选择开发产品和解决方案的方式。当我们为产品战略考虑用户体验时，我们开始[探索其他方式](http://interactions.acm.org/archive/view/january-february-2017/strategic-ux)来解决客户问题，了解市场痛点，并满足用户的期望。

{%youtube%}pYJEiC9Cs-A{%endyoutube%}

我们可以利用战略研究来：

- 了解如何在不同的领域或人群中应用一个解决方案。例如，考虑不同的行业，如律师策划的法律文件，如何利用源代码控制管理进行版本控制。
- 探索对当前问题的额外约束，使其更适合未来的发展 -- 例如，在一个功能上增加支持的并发用户数。 
- 考虑上游和下游的体验 - 例如，通过使用 Auto DevOps 来增强 GitLab 用户的验证体验，以帮助他们更容易地开始持续集成。
- 识别新兴的市场趋势。例如，如果客户对他们采用 DevOps 的成熟度表示兴趣，那么发现 GitLab 可以使用机器学习或人工智能来指导人们的成熟度的方法。

如需查看战略研究的实例和资源，请访问我们的[战略研究实例](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/strategic-research-at-gitlab/strategic-research-examples.html)网页。

### GitLab 是如何看待战略研究的？

**战略研究是指以下方面的研究：**

* 直接告知团队和/或组织的战略
* 旨在回答更广泛的研究问题，不针对单个阶段或特征
* 与问题验证的联系比解决方案验证更紧密
* 独立于每月发行周期
* 专注于未来 6 个月到 3 年

**它不是：**

* [解决方案的验证](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/solution-validation-and-methods/)
* 专门针对单一阶段的小组（大多数情况下）。
* 与特定议题/功能相联系的问题验证研究

**战略研究是什么样子的?**

* 为用户体验或产品方向提供信息的研究
* 跨越用户旅程的研究，而不是针对产品阶段组的研究 
* 寻求理解和挑战当前功能假设的研究 
* 让跨阶段或多阶段的利益相关者参与的研究
* 界定未满足需求的研究
* 对用户角色的添加、细化或删除的研究

**如何衡量战略研究？**

* 在项目层面，成功将由研究的影响来衡量。 随着战略研究在 GitLab 的成熟，我们将寻找可适用于所有战略研究项目的通用成功衡量标准。

**优秀的战略研究实例**

* 了解阶段组的使用趋势
* 扩大对客户动机、目标、挑战和需求的了解
* 识别我们客户最大的 IT 举措/目标
* 了解 GitLab 如何克服采用 DevOps 的困难
* 进一步了解跨阶段的用例和工作流程
* 确定 Ops 能够推动多个阶段和阶段组采用的方式

了解更多[跨阶段研究计划](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/strategic-research-at-gitlab/cross-stage-research-program.html)

### 战略性研究成果

战略研究的成果可以在议题中找到，对文件的修改，以及对一个类别方向页（包括1年和3年的愿景）的公开修改，例如：

* [GitLab 3 年战略](https://about.gitlab.com/direction/#3-year-strategy)
* [GitLab 的方向性用户画像](https://about.gitlab.com/direction/#personas)
* [Dev 部分 1 年计划](https://about.gitlab.com/direction/dev/#dev-section-fy22-themes)
* [Ops 部分 1 年计划](https://about.gitlab.com/direction/ops/#ops-section-plan)
* [Sec 部分 1 年计划](https://about.gitlab.com/direction/security/#1-year-plan) 

### 战略研究计划是如何运作的？

**注：**首席用户体验研究员是设计研究概要并提供研究目标和假设的初步纲要的人。首席用户体验研究员可以拥有任何级别的资历和经验，从研究协调员到员工用户体验研究员。首席用户体验研究员是该研究的[DRI](https://about.gitlab.com/handbook/people-group/directly-responsible-individuals/)。他们应该在利益相关者会议上和研究议题中传达他们是DRI。

1. 首席用户体验研究员与相关项目管理人员、其他用户体验研究员、研究协调员和用户体验研究经理会面，讨论研究的目标和他们的假设。这个会议的目的是为了得到所有利益相关者的支持。如果一个利益相关者不能参加会议，请记录会议内容，并提供异步提供反馈的机会。
1. 首席用户体验研究员使用[问题验证模板](https://gitlab.com/gitlab-org/gitlab/-/blob/master/.gitlab/issue_templates/Problem_Validation.md)创建一个问题。
1. 首席用户体验研究员将~ `workflow::problem validation` 标签应用于相关议题，这将自动删除~`workflow::validation backlog`标签。
1. 首席用户体验研究员尽其所能完成一个[机会画布](https://about.gitlab.com/handbook/engineering/ux/ux-research/#opportunity-canvas)。确保问题和角色得到很好的阐述，并将机会画布添加到议题的[Designs](https://docs.gitlab.com/ee/user/project/issues/design_management.html#the-design-management-page)中。注意，你应该在内容中包含 解决方案 和 go-to-market 部分的内容，这一部分不需要有非常高的确信。这部分可能会改变，但是仔细思考会帮助你理清思路。
1. 首席用户体验研究员使用用户体验研究项目中的可用模板打开一个问题验证研究议题，并完成它，使用 `UX问题验证` 标签，并将该议题分配给相关用户体验研究员。
1. 按照[用户访谈](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/writing-usability-testing-script/)或调查概述的步骤进行。然而，对于多阶段小组计划，首席用户体验研究员应该负责用户访谈或调查过程中列出的所有步骤 — 例如，编写讨论指南。如果他们需要帮助，欢迎他们将职责委派给其他用户体验研究人员。
1. 首席用户体验研究员与相关项目经理、用户体验研究员和用户体验研究经理会面，讨论研究结果和下一步。
首席用户体验研究员可能需要:
  * 通过综合反馈完成机会画布。
  * 向 Scott Williamson, Christie Lenneville 和相关的产品总监展示机会画布。
