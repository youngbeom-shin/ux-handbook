---
layout: handbook-page-toc
title: "Secure & Protect 用户体验"
description: "我们正在设计一种体验，使贡献者能够提交他们最安全的工作，并保护他们在生产中拥有的东西。"
---

### 概述
我们正在设计一种体验，使贡献者能够提交他们最安全的工作，并保护他们在生产中拥有的东西。这是通过将安全合并到 DevOps 流程中来实现的，给予开发团队更多的所有权，通常被称为 DevSecOps。这种体验将跨职能的利益相关者聚集在一起，以做出更好、更快、更安全的决策。我们通过将体验集中在自动化、教育、授权和将安全转移到左边来实现这一目标。

**自动化** 指的是约定俗成的配置，有助于为用户画出一条清晰的路径，产生有意义的结果。当涉及到网络安全时，没有一个应用程序会是100%的安全。这就是为什么我们专注于将自动化整合到用户旅程的每一步，从配置中抽出猜测的时间，以便将更多的时间用于重要的事情上：解决已知的漏洞和识别攻击或威胁。

**教育** 我们的用户，使他们了解安全基础知识，并意识到他们的应用程序的安全需求。我们希望我们的用户知道在哪里检测到了漏洞或威胁，将其含义可视化，提供资源以理解问题，并提供工具以促进关于下一步的明智决策。

**授权** 所有用户解决安全问题的权力是至关重要的，因为跨职能部门共享安全所有权。我们的工具力求实现开发人员负责、安全团队负责组织安全的体验。

**左移** 是指将 QA 和其他通常出现在运维周期后期的流程转移到开发中。就可以更早、更频繁地处理安全问题。

### 客户
各种规模的组织都从我们的工具和将团队聚集在一起的经验中受益。我们通过高效的工作流程、明智的团队决策、降低安全漏洞的风险以及达到合规要求，为客户提供价值。我们关注产品的各个方面——从客户体验开始。当决定使用我们的工具时，组织通常会考虑以下几点:

* 该工具支持哪些语言？
* 我们需要涵盖哪些测试？
* 该工具涵盖哪些测试？
* 它能自动化吗？
* 设置需要多长时间？
* 设置涉及什么？
* 使用起来有多方便？
* 你需要使用什么技术？(例如：Docker、Kubernetes)
* 这个工具有多轻？
* 它如何与我们的工具整合？
* 它是如何与 GitLab 的产品整合的？
* 提供哪些客户支持？
* 即将推出的功能有哪些？(我们销售的是合同制服务，而不是月度服务)

### Jobs to be Done
我们使用[Jobs to be Done (JTBD)框架](https://about.gitlab.com/handbook/engineering/ux/jobs-to-be-done/)来保持我们对用户目标的关注，并确保我们在用户的价值上对他们提供支持。请看安全和保护要完成的工作的分类[这里](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/sec/jtbd/index.html)。

我们还为我们的 JTBD 进行了[用户体验记分卡评估](https://about.gitlab.com/handbook/engineering/ux/ux-scorecards/)。参见安全和保护以及其他阶段的用户体验记分卡，[这里](https://gitlab.com/groups/gitlab-org/-/epics/1714)。

### 团队
* [Justin Mandell](https://gitlab.com/jmandell) - 产品设计经理
* [Andy Volpe](https://gitlab.com/andyvolpe) - 产品设计师
* [Becka Lippert](https://gitlab.com/beckalippert) - 高级产品设计师
* [Camellia Yang](https://gitlab.com/cam.x) - 高级产品设计师
* [Michael Fangman](https://gitlab.com/mfangman) - 产品设计师

#### 团队架构
我们已经将我们的阶段划分为专门的体验小组，以便与我们的工程和项目管理同行进行的类似[分割](https://about.gitlab.com/handbook/product/categories/#sec-section)保持一致。这是管理我们资源的一个很好的方法，但我们的思维方式仍然集中在为我们的小组提供整体的用户体验。

**Secure**

| 小组                  | 类别                                            | 负责设计师                   |
| ---------------------- | --------------------------------------------------- | --------------------------------- |
| 构成分析   | 依赖性扫描，许可证合规性             | Secure & Protect 用户体验团队 (共享) |
| 动态分析       | DAST, 模糊测试                                 | Michael Fangman                   |
| 静态分析        | SAST, Secret 检测, 代码质量                | Michael Fangman                   |
| 威胁洞察       | 漏洞管理                            | Becka Lippert, Andy Volpe         |

**Protect**

| 小组                    | 类别                                                                                            | 负责设计师 |
| ------------------------ | --------------------------------------------------------------------------------------------------- | --------------- |
| 容器安全       | 容器网络安全、容器主机安全、安全编排和容器扫描 | Camellia Yang   |   

Secure & Protect 用户体验团队在所有 Secure & Protect 方面紧密合作，并在以下领域共享覆盖范围:

- 安全仪表板
- 安全报告 
- 合并请求中的安全部件
- 状态、指标和报告
- 安全配置

这种细分使我们有更好的机会：

- 在我们的分组内增长我们的专业知识和知识，同时与团队其他成员分享相关信息。
- 发展和维护与我们的专业工程团队和 PM 的关系。
- 担任已知的主要联络点。
- 通过发起或领导针对我们体验组的研究活动，深入了解我们用户的需求。
- 专注于迭代和推进我们的经验，从 MVC 到 Lovable。

在[这里](https://gitlab.com/gitlab-org/gitlab-design/issues/458)阅读更多关于我们如何创建这些专门的经验小组。

#### 团队战略
**短期 (6 - 12个月)** (截止到 2021-09-22)

* 💕 🧠 教育我们的团队和合作伙伴了解我们的目标、战略和背后的原因
* 🖼 制定一个路线图框架，供所有安全与保护团队使用。
* 📐 审查、评估和解决我们现有的用户界面的可学习性和可用性问题
* 🚀 基于 JTBD 为未满足的需求提供解决方案，使用户能够采用 GitLab 作为其 DevOps 平台。

**长期 (1 - 3年)** (截止到 2021-09-22)

* 📚 评估应用程序的安全成熟度情况，并帮助我们的用户提高他们的成熟度（见[概述部分](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/sec/#overview)中的赋权）。
* 🚌 帮助我们的用户学习和提高他们的团队对使用我们工具的重要性的知识，以及如何有效地使用它们的技能(参见[概述部分](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/sec/#overview)的教育、赋权和左移)
* 💕 🧠 继续教育我们的团队和合作伙伴，让他们了解我们的目标、战略和背后的原因。

#### UX pages
* [Secure UX](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/secure/)
* [Protect UX](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/protect/)

### 我们如何工作
我们遵循 [GitLab 工作流程](https://about.gitlab.com/handbook/engineering/workflow/#product-development-timeline)和[额外的日期](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/sec/)以及与我们的工作直接相关的行动。

对于与 ux 相关的问题或涉及到 Secure and Protect 所有组的 MRs(如果你不确定 DRI 是谁)，我们通过使用  `@gitlab-com/gitlab-ux/secure-protect-ux` 来鼓励透明度和协作。

对于安全仪表板和漏洞报告页面上的任何功能开发，或影响其性能的功能开发，应通过使用 `@gitlab-org/secure/threat-insights-backend-team` 尽早通知威胁洞察后端工程团队，以评估该功能的性能影响。

### 团队会议
* 用户体验小组的每周团队 social（Secure & Protec，Configure 和 Montior团队签到）会议在周二上午8:00（PST）举行（更多细节见下文）。
* Secure & Protect 用户体验 - 产品设计和产品管理每4周在周三上午 7:00（PST） 举行一次完善会议（我们审查即将到来的里程计划，在新的里程碑开始前2周）。
* 里程碑前的计划会议 每月一次，时间是第二个星期一上午9:00（PST）（我们为即将到来的里程碑敲定计划）。

这些包括与安全设计、用户体验和研究相关的主题。一些例子的主题可以包括：

- 关于进行中和计划中的研究的最新情况
- 关于设计议题的更新
- 可能有风险或有阻碍的议题
- 最近在进行研究时发现的见解
- 更新我们的用户体验记分卡
- 更新用户体验工作流程和过程的变化
- 关于我们正在进行的试点举措的最新情况
- 战略迭代

有些议题更适合在专门的会议上讨论，应该根据需要来创建：

- 里程碑的规划和细化
- 关键性设计
- 研究报告宣读
- 对麻烦的议题进行同步

##### 我们所使用的标签
我们使用`devops::stage_name`和`UX`标签来表示需要用户体验工作的问题。我们处理的用户流经常跨越多个类别，所以我们在一个里程碑开始之前审查每一个议题，以确定设计分配人或受让人。

* `UX`+`devops::stage_name`。这是一个共同的用户体验工作，工程方面的工作还没有确定。
* `UX`+`devops::stage_name`+`Category::name`。有一个用户体验的 DRI（可以共享）和明确的工程合作。
* `UX`+ `devops::stage_name`+ `UX debt`。当提议的设计被取消范围或未按计划实施时，用于后续问题。

有关我们如何使用标签的更多信息，请参见我们的 [UX工作流程](https://about.gitlab.com/handbook/engineering/ux/ux-department-workflow/#how-we-use-labels)页面。

##### 问题和解决方案的验证议题
当在处理一个`workflow::problem validation` 或 `workflow:solution validation`的议题时，需要在接下来的两个版本中实施，确保有一个占位的实施议题。这个议题必须与史诗相关联，并有一个暂定的里程碑。

#### 规划和完善
我们使用[团队计划板](https://gitlab.com/groups/gitlab-org/-/boards/2131151?milestone_title=13.11&)作为工具，帮助我们监测我们的速度，使我们能够更有效地将我们的时间传达给我们的同行们。

在每个里程碑的开始，我们创建一个团队里程碑计划议题(使用下面的[模板](#Team-Milestone-Planning-Issue-template))来启动团队讨论，围绕下一个即将到来的里程碑(不是刚刚开始的里程碑)需要处理的议题展开讨论。我们这样做是为了确保每个小组都有:

* 产品设计师覆盖到
* 让人们更清楚地了解每个小组正在进行的工作
* 增加跨组合作的潜力
* 增加各组的知识

**`M-1, 17th` (里程碑开始前1个月)**

* 产品设计经理（PDM）：从团队的计划议题模板中为该里程碑创建一个计划议题。
* PDM：将议题分配给整个团队
* 团队：与你的产品经理（PM）讨论下一个里程碑的设计工作的需求。
* 产品设计师（PD）将在产品设计师的可用能力表中填写他们预期的组别、灵活性和总能力。

**`M-1, 24th` (里程碑开始前约3周)**

* 每个 PM 和产品设计师（PD）的同行将一起工作一周，为他们小组的用户体验需求表添加内容。
* 每个 PD 将在 OKR/额外 UX 需求表中添加任何他们希望在即将到来的里程碑中处理的 OKR 或额外议题

**`M-1, 1st` (里程碑开始前约2周)**

* 现在，所有小组的用户体验需求表都已经填写完毕，是时候讨论是否有人需要额外的产品设计师协助了（例如，一个议题的优先级被认为高于另一个小组的优先级列表，或者一个没有对应 PD 的 PM 有工作需要完成）。

**`M-1, 8th` (里程碑开始前约1周)**

* 为圆桌团队签到添加新的评论 👍/ 👎，以确保每个人都被覆盖并对结果满意。

**`M, 17th` (里程碑的开始)**

* PDM: 关闭规划议题

<!--
* By month `M-1, 4th` (at least 14 days before milestone `m` begins):
     * PM updates planning boards to propose issues that may be included in the next release (released 22nd of next month).
     * Product Designers hold a UX Planning session to review the issues, make assignments, and discuss capacity. UX proposes additional issues to include in the milestone.
     * Each issue is followed with a discussion (comment) to inform our capacity or request additional information.
* By month `M-1, 13th` (at least 5 days before milestone `m` begins):
     * PM finalizes the Release scope. In-scope issues are marked with milestone `m`; label `deliverable` applied.
     * PM updates the Kickoff document with relevant items to be included.
* By month `M-1, 17th` (at least 1 day before milestone `m` begins):
     * Group Kickoffs calls recorded and uploaded by PM.
* On month `M-1, 18th` (or next business day, milestone `m` begins): Kick off! 📣
     * Company Kickoff call live streamed by PM.
     * Development on milestone `m` begins
-->

#### 团队里程碑规划议题模板

<!-- 
它是如何工作的?
	1.	(M1, 22nd)  在每个里程碑的开始，将创建一个新的安全设计规划议题来讨论下一个里程碑的设计工作的需求。 
	2.	(M1, 1st) 每个产品经理(PM)和产品设计师(PD)的同行将一起工作一周，为他们小组的用户体验需求表添加内容，如下。
	3.	(M1, 8th) 小组表格已经填写完毕，现在是时候讨论是否有人需要额外的产品设计师协助了（例如，一个问题的优先级被认为高于另一个小组的优先级列表，或者一个没有对应的产品设计师的PM有工作需要完成）。
	4.	(M1, 15th) 为圆桌团队签到添加新的评论 👍/ 👎，以确保每个人都被覆盖并对结果满意。
	5.	(M, 22nd) 关闭议题并开展工作 :)
--> 
    ### 产品设计师的可用工作量
    <!-- 小组工作量是指你在这个里程碑中能够为小组工作贡献的权重点的数量.
    弹性工作量是指你将保留的任何额外的权重点，以适应任何OKR、UX部门或任何其他你期望在这个里程碑期间突然出现的额外工作。  -->
    | 设计师 | 小组工作量 | 弹性工作量 | 所有工作量 |
    | ------ | ------ | ------ | ------ |
    | Andy     |   |   |   |
    | Becka    |   |   |   |
    | Camellia |   |   |   |
    | Michael  |   |   |   |

     ### 产品设计师休假 (OOO)
     | 设计师 | OOO 开始 - 结束 |
     | -------- | --------------- |
     | Andy     |                 |
     | Becka    |                 |
     | Camellia |                 |
     | Michael  |                 |

     ### 审查现有的用户体验债务和用户体验 SUS 相关议题
     注意：我们需要迅速对这些议题采取行动，因为它们会影响我们的可用性。
     * [用户体验债务议题看板](https://gitlab.com/groups/gitlab-org/-/boards/3760565?label_name[]=UX%20debt)
     * [SUS 相关议题看板](https://gitlab.com/groups/gitlab-org/-/boards/3738104?label_name[]=UX&label_name[]=severity%3A%3A2&label_name[]=type%3A%3Abug)

    ### 构成分析 用户体验需求
    | 优先级 | 议题/史诗 | State | 💯 Need / 💪 Nice to have | 设计师 | 准备构建 | ≅ 权重 | 结转注释 |
    | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
    | 1 | <!-- 链接到这里  --> | <!-- 准备设计 --> | <!-- 💯  --> | <!-- 设计师名称  --> | <!-- 里程碑 --> | <!-- 权重 --> | <!-- 添加注释，为什么在前一个里程碑中没有完成 --> |
    | 2 | <!--  链接到这里  --> | <!-- 需要解决方案的验证 --> | <!-- 💪  --> | <!-- 设计师名称  --> | <!-- 里程碑  --> | <!-- 权重 --> | <!-- 添加注释，为什么在前一个里程碑中没有完成 --> |

    ### 容器安全用户体验需求
    | 优先级 | 议题/史诗 | State | 💯 Need / 💪 Nice to have | 设计师 | 准备构建 | ≅ 权重 | 结转注释 |
    | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
    | 1 | <!-- 链接到这里  --> | <!-- 准备设计 --> | <!-- 💯  --> | <!-- 设计师名称  --> | <!-- 里程碑 --> | <!-- 权重 --> | <!-- 添加注释，为什么在前一个里程碑中没有完成 --> |
    | 2 | <!--  链接到这里  --> | <!-- 需要解决方案的验证 --> | <!-- 💪  --> | <!-- 设计师名称  --> | <!-- 里程碑  --> | <!-- 权重 --> | <!-- 添加注释，为什么在前一个里程碑中没有完成 --> |

    ### 动态分析：DAST/Fuzz 用户体验需求
    | 优先级 | 议题/史诗 | State | 💯 Need / 💪 Nice to have | 设计师 | 准备构建 | ≅ 权重 | 结转注释 |
    | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
    | 1 | <!-- 链接到这里  --> | <!-- 准备设计 --> | <!-- 💯  --> | <!-- 设计师名称  --> | <!-- 里程碑 --> | <!-- 权重 --> | <!-- 添加注释，为什么在前一个里程碑中没有完成 --> |
    | 2 | <!--  链接到这里  --> | <!-- 需要解决方案的验证 --> | <!-- 💪  --> | <!-- 设计师名称  --> | <!-- 里程碑  --> | <!-- 权重 --> | <!-- 添加注释，为什么在前一个里程碑中没有完成 --> |

    ### SAST 用户体验需求
    | 优先级 | 议题/史诗 | State | 💯 Need / 💪 Nice to have | 设计师 | 准备构建 | ≅ 权重 | 结转注释 |
    | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
    | 1 | <!-- 链接到这里  --> | <!-- 准备设计 --> | <!-- 💯  --> | <!-- 设计师名称  --> | <!-- 里程碑 --> | <!-- 权重 --> | <!-- 添加注释，为什么在前一个里程碑中没有完成 --> |
    | 2 | <!--  链接到这里  --> | <!-- 需要解决方案的验证 --> | <!-- 💪  --> | <!-- 设计师名称  --> | <!-- 里程碑  --> | <!-- 权重 --> | <!-- 添加注释，为什么在前一个里程碑中没有完成 --> |

    ### 漏洞管理的用户体验需求
    | 优先级 | 议题/史诗 | State | 💯 Need / 💪 Nice to have | 设计师 | 准备构建 | ≅ 权重 | 结转注释 |
    | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
    | 1 | <!-- 链接到这里  --> | <!-- 准备设计 --> | <!-- 💯  --> | <!-- 设计师名称  --> | <!-- 里程碑 --> | <!-- 权重 --> | <!-- 添加注释，为什么在前一个里程碑中没有完成 --> |
    | 2 | <!--  链接到这里  --> | <!-- 需要解决方案的验证 --> | <!-- 💪  --> | <!-- 设计师名称  --> | <!-- 里程碑  --> | <!-- 权重 --> | <!-- 添加注释，为什么在前一个里程碑中没有完成 --> |

    ### OKR/额外 用户体验需求
    | 优先级 | 议题/史诗 | State | 💯 Need / 💪 Nice to have | 设计师 | 准备构建 | ≅ 权重 | 结转注释 |
    | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
    | 1 | <!-- 链接到这里  --> | <!-- 准备设计 --> | <!-- 💯  --> | <!-- 设计师名称  --> | <!-- 里程碑 --> | <!-- 权重 --> | <!-- 添加注释，为什么在前一个里程碑中没有完成 --> |
    | 2 | <!--  链接到这里  --> | <!-- 需要解决方案的验证 --> | <!-- 💪  --> | <!-- 设计师名称  --> | <!-- 里程碑  --> | <!-- 权重 --> | <!-- 添加注释，为什么在前一个里程碑中没有完成 --> |

     * [ ] 设置里程碑（当前的里程碑）。
     * [ ] 为当前里程碑的结束设置到期日
     * [ ] 给整个团队分配PM和PD

    /label ~"section::sec" ~"Planning Issue"


##### 了解工作量
我们的里程碑计划活动的一部分包括考虑每个指定议题所需的工作量。我们使用以下量表:

| 大小     | 权重 | 描述                                                  |
| -------- | ------ | ------------------------------------------------------------ |
| 琐碎  | 1      | 主要是小到中等的用户界面变化，较小的用户体验改进，没有未回答的问题。用户体验可能需要继续参与这个议题，但可能不需要做工作。 |
| 小型    | 2      | 简单的用户界面或用户体验改变，我们了解所有的需求，但可能需要找到已知问题/难题的解决方案。 |
| 中等   | 3      | 一个中等的变化（需要大量的UI或UX变化/改进）。涉及多个页面，我们开始设计/重新设计小流程。在工作中可能会出现一些未知的问题。 |
| 大型    | 5      | 需要其他团队成员参与的复杂变更。跨越多个页面，我们致力于中等规模的流程。有很多悬而未决的问题需要回答。 |
| 庞大的     | 8      | 跨越大型流程的复杂变更，可能需要其他设计人员的参与。这是我们将在单个里程碑中进行的最大的流程设计/重新设计。 |
| 巨大的 | 13     | 一个跨越多个流程的重大变化，需要其他人（团队、团队成员、用户反馈）的大量投入，而且有许多未知的未知因素。我们不太可能在一个里程碑中承诺这一点，我们更倾向于进一步澄清需求和/或分解成更小的问题。 |

### 我们的战略
Secure 和 Protect 用户体验团队正在一起工作，以[发掘客户的核心需求](https://gitlab.com/groups/gitlab-org/-/epics/1611)，我们用户的工作流程是什么样的，并定义我们如何使用户的任务更容易。我们的策略包括以下行动：

* [用户体验记分卡和建议](https://about.gitlab.com/handbook/engineering/ux/ux-scorecards/) (季度)
* 内部了解：利益相关者访谈（每年）
* 迭代 Secure 产品 [foundation 文件](https://gitlab.com/gitlab-org/gitlab-design/issues/333) (进行中)
* 迭代 Protect 产品 [Foundation 文件](https://gitlab.com/gitlab-org/gitlab-design/issues/547) (进行中)
* 对至少3个竞争对手执行启发式评估，基于3个用户类型正在使用的竞争对手(每年，持续)
* 我们与我们的客户交谈（持续）
* 我们与我们的用户交谈（持续）
* 我们概述了当前的用户工作流程，并对其进行了改进（即将到来，正在进行）

此外，我们还重视以下方面：

* 用实用性和可用性研究来测试我们的功能
* “喝我们自己酿的酒”，并与我们内部的安全和合规团队密切合作，以获得反馈和功能采用。
* 与我们的销售和客户团队合作，直接与客户联系，了解客户为什么选择（或不选择）我们的产品。
* 与利益相关者合作进行概念验证的发现，以更好地了解未来的考量
* 在 Secure 和 Protect 团队之间进行合作，以确保我们提供一个一致的、有凝聚力的安全工作流程，这样我们的客户就可以将反应性结果应用到主动措施中，并确保他们的应用在整个应用生命周期中得到保护。
* 优先考虑有可能增加我们活跃用户数量的议题

可信源与已发布的特性一同存在，因此我们:

* 迅速而周到地做出数据驱动的决策
* 优化以尽快提供我们的解决方案
* 学习、迭代、测试和重复

### 学习和发展
下面是一个资源清单，它提供了对我们正在设计的行业的基础性理解，因为它与 GitLab 有关。

#### 网站和资源 

##### 入门
-[GitLab Secure UX 101](https://app.mural.co/t/gitlab2474/m/gitlab2474/1573242955373/e0edcc6d4be079e36a7e26eebb0950961b9506c7?sender=avolpe0924)

##### 安全框架和标准
- [NIST Cybersecurity framework](https://www.nist.gov/cyberframework)
- [OWASP Top Ten](https://owasp.org/www-project-top-ten/)

##### 漏洞类型和定义
- [MITRE - CWEs explained](https://cwe.mitre.org/about/index.html)
- [MITRE - CVEs explained](https://cve.mitre.org/about/index.html)
- [National Vulnerability Database NVD](https://nvd.nist.gov/)

#### LinkedIn学习课程
- [DevOps Foundations: DevSecOps](https://www.linkedin.com/learning/devops-foundations-devsecops?u=2255073) • 54m • 初学者
- [DevSecOps: Automated Security Testing](https://www.linkedin.com/learning/devsecops-automated-security-testing?u=2255073) • 1h 35m • 初学者 + 中级
- [Learning the OWASP top 10](https://www.linkedin.com/learning/learning-the-owasp-top-10?u=2255073) • 43m • 初学者 + 中级
- [Security for the SMB: Implementing the NIST Cybersecurity Framework](https://www.linkedin.com/learning/security-for-the-smb-implementing-the-nist-cybersecurity-framework?u=2255073) • 1h 23m • 中级
- [Vulnerability Management: Assessing the Risks with CVSS v3.1](https://www.linkedin.com/learning/vulnerability-management-assessing-the-risks-with-cvss-v3-1/welcome-to-this-course?u=2255073) • 1h 14m • 中级

### 关注我们的工作
我们的 [Secure and Protect UX YouTube 频道](https://www.youtube.com/playlist?list=PL05JrBw4t0KrFCe5BgUkzFrZifjforQOz) 包括用户体验记分卡演练、用户体验审查、小组反馈会议、团队会议，以及更多。


