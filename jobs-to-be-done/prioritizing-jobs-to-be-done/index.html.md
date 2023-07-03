---
layout: handbook-page-toc
title: "Prioritizing Jobs To Be Done"
description: "How to determine which JTBD to focus on"
---

### 优先考虑 JTBD

通常情况下，一个类别的JTBD数量之多，会使我们很难知道该把设计和工程的精力集中在哪里。确定哪些JTBD对我们的客户来说是最关键的，最好的方法是采用用户研究。确定最关键的JTBD有助于为未来的研究、设计和产品需求做计划。确定这一重点的最流行的方法之一是利用调查，因为它们增加了你对特定类别的JTBD的正确列表的信心。

### 概述

JTBD的优先级调查是在 Qualtrics 中建立的[打开访问请求](/handbook/business-ops/team-member-enablement/onboarding-access-requests/access-requests/). [More information on how to use Qualtrics.](/handbook/engineering/ux/qualtrics/).

请记住:
- JTBD堆栈排名和JTBD细节部分可以为你的每个JTBD类别复制。
- 在创建调查问卷时，要避免围绕JTBD的具体语言或其他GitLab的具体言辞。相反，要专注于一个平易近人的和通用的问题风格。
- 针对你所在类别的[主要和次要角色](/handbook/marketing/strategic-marketing/roles-personas/#user-personas) 进行调查. 
- 如果你对执行调查有任何问题(需要回复的数量，如何最好地定位参与者，时间线等)，请与你的 [UX 研究员](/handbook/engineering/ux/ux-research/) 合作。

下面是一个Package阶段使用的一个 [调查示例](https://gitlab.eu.qualtrics.com/jfe/preview/SV_bjxethMCmXbavop?Q_CHL=preview&Q_SurveyVersionID=current)。 你可以复制使用，并根据你的需求修改它。


#### 角色识别

这些问题对参与者进行资格审查，确保他们符合你在 JTBD 反馈中所针对的角色。不符合你要求的参与者会被提前删除，从而减少参与者的挫败感，因为他们不需要回答他们没有资格回答的问题。

要包括的问题: 

- 职位名称或工作职责
- 团队、部门和组织规模
- GitLab的使用情况(当前用户、被动用户等)以及他们使用的级别(免费版到旗舰版)
- 其他问题，以帮助确定您的特定类别的参与者（此人是否积极使用Docker镜像进行包测试）。

#### JTBD堆栈排名 

调查的这一部分包含**1**个问题，要求参与者阅读一系列待完成的工作。

最佳做法，使你不至于让你的参与者不知所措:

- 为每个类别的JTBD创建一个排名问题，并列出每个排名问题的JTBD。
   
   - 同样的措辞:将最具影响力的选项放在最上方，将下列与软件包和图像相关的共同目标/计划按它们对团队或组织的影响程度排序。
- 使用随机排序来帮助保持结果的公正。

#### JTBD 详细内容

调查的这一部分是针对**某一项需要完成的工作**。
对于有许多JTBD的类别，使用调查逻辑确保参与者只被提出与他们排名前1-3的 JTBD 相关的问题。

问题包括:
- "GitLab能在多大程度上满足您与（该 JTBD）相关的需求?"
- "评价(某一特定任务)的影响(或重要性)."
- 包括一个开放性的问题“你没有看到列表中提到的与(JTBD)相关的其他任务是什么?”
  - 这个问题将告知你可能遗漏的任何重要任务，增加你对
 JTBD 和相关任务类别的信心。


### 结果

在获得你的目标所需的调查回应数量后 (如果你不确定，请联系你的 [用户体验研究员](/handbook/engineering/ux/ux-research/), 接下来的步骤是综合你的数据和 [在DoveTail中记录你的见解](/handbook/engineering/ux/ux-research-training/documenting-research-findings/). 

这些见解应该包括具体的

相关信息: 

- JTBD的重要性排名
- JTBD中具体任务的重要性排序
- 缺少的任何重要的 JTBD 或某个类别的任务

在Dovetail中创建见解后，你应该与更广泛的阶段组以及其他阶段组分享这些数据，以鼓励跨阶段合作。
