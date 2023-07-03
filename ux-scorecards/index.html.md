---
layout: handbook-page-toc
title: "用户体验记分卡"
description: "用户体验记分卡是一个类似于启发式评估的过程，它有助于识别可用性问题并对特定的体验进行评分。"
---

## 介绍和目标

用户体验记分卡是我们根据一套启发式的方法来识别和评分我们产品中的体验的可用性。我们使用用户体验记分卡来了解用户如何与我们的产品进行互动，并迅速发现改进的机会。

用户体验记分卡应该在每一个重要的工作流程中进行，并且应该不定期地重复，这样我们就可以不断地监测我们在为用户提供更好体验方面的进展。

作为用户体验从业者，我们必须从战略上考虑如何解决 GitLab 产品中的可用性问题，以便为用户提供高质量的体验。创建一个带有相关建议的用户体验记分卡，使我们能够在特定的工作流程中识别、界定和跟踪解决可用性问题的努力。当它完成后，我们就有了与产品经理合作的必要信息，将修复工作归入有意义的迭代中，并对用户体验相关问题进行优先排序。

所有的用户体验记分卡都可以在这个[史诗](https://gitlab.com/groups/gitlab-org/-/epics/1714)中找到。

## 关于流程

用户体验记分卡流程是为了平衡灵活性和一致性。有几种方法可以创建你的记分卡，从最轻到最重列出。根据你的时间、工作流程对用户的优先级，或者这是否是 JTBD 的第一个记分卡来选择一个合适的方法。

### 记分卡方法

在制作记分卡时，你可以选择:

#### 方案A:进行启发式评估

通过做一个[启发式](https://www.nngroup.com/articles/ten-usability-heuristics/)评估来回顾当前的经验。这可以在半天内完成，这是一个快速的方法，特别是如果你正在为一个以前已经打过分的任务做记分卡。

使用一个体验地图，比如在[记分卡体验模板](https://www.figma.com/file/GP810syJHzyIwHbCekBnPu/Scorecard-Experience-Map?node-id=0%3A1)中找到的那个，捕捉屏幕并记下观察结果。在评估过程中，要努力带入与 JTBD 相关的角色的场景，并且在这样做的时候，尽量从他们的角度来看待用户界面，就好像他们是一个新的用户一样。在评估过程中，你很容易忘记这一点，所以建议在你的视野中的某个地方放一个提醒，比如在你的显示器上贴一张便利贴，上面写着 "你是一个新用户！"

#### 选择B:进行形成性评价

你可以通过让内部或外部用户尝试完成JTBD来做一个[形成性评价](https://www.nngroup.com/articles/formative-vs-summative-evaluations/)。其目的是为参与者提供背景（JTBD 的情景），并倾听和观察他们如何尝试完成工作。我们学到的东西可能因参与者而异。

在做形成性评价时，做一个 "轻型 "的可用性测试，观察3-5个内部或外部用户，因为这可以提供有价值的见解并消除主观性。如果你要评估的场景在测试项目中的设置比较简单，这可以在一天内完成。如果你的方案是高度技术性的，需要复杂的定制，请提前计划，因为光是建立一个评估环境就需要几天的时间。

在每一种情况下，
- 在进行记分卡之前，定义[JTBD](https://about.gitlab.com/handbook/engineering/ux/jobs-to-be-done/)。
- 在评估经验时，使用我们的[启发式方法](https://about.gitlab.com/handbook/engineering/ux/heuristics/)。
- 使用[评分标准](#grading-rubric)来提供一个整体的衡量标准，成为体验的基准分数。
- 对用户的观察比纯粹的启发式评价更可取，因为它将消除主观性。 

这是一个旨在帮助为设计过程提供信息并保持高质量标准的过程。

### 用户体验记分卡与类别成熟度记分卡的关系

**何时创建 UX 记分卡:**

- 在一个体验中快速识别可用性问题和改进的机会，并按优先级排序。 
- 当加入一个新的产品领域，熟悉工作流程，并从一个新的角度评估经验。
- 与可用性测试工作流相结合。
- 为了评估你的工作流程的onboarding体验。
     
**何时创建[类别成熟度记分卡](https://about.gitlab.com/handbook/engineering/ux/category-maturity-scorecards/)：** 

- 当一个类别中需要进行更严格的测试时，这些测试与该类别提升所需的一组业务需求和/或特性有关。这是一个总结性的过程(不是为了确定可用性问题)，它允许我们收集指标和数据，帮助我们理解随着时间的推移，产品的变化如何影响用户体验。我们用这个过程来为产品的成熟度打分。

## 设置

下面是完成用户体验记分卡的推荐步骤。请注意，每个记分卡都是不一样的。我们欢迎产品设计师根据他们的需要来调整这些步骤，只要他们尽可能的客观，并且精神和结果保持一致。

1. 创建一个（或找到现有的）epic，它将包含该阶段组的所有用户体验记分卡。  
    > 例如："UX Scorecard - Create:Source Code"
1. 如果尚未完成，请将阶段组史诗添加到 [UX Scorecards - All Evaluations](https://gitlab.com/groups/gitlab-org/-/epics/1714) 史诗中。 
1. 与你的产品经理合作，确定你所在阶段的用户的首要工作（在频率或重要性方面）。理想情况下，你将根据用户研究（分析或定性研究结果）来制定这个任务清单。
1. 选择其中一个最重要的工作来完成一个UX记分卡。
1. [创建一个体验评分问题](https://gitlab.com/gitlab-org/gitlab-design/issues/new?issuable_template=UX%20Scorecard%20Part%201)，使用模板 “WIP: UX Scorecard Part 1”，并将其添加到阶段组史诗中。

    这个议题应该有**UX记分卡**的标签。如果它与 OKR 有关，也要贴上 **OKR** 标签，以方便追踪。
1. [创建一个建议议题](https://gitlab.com/gitlab-org/gitlab-design/issues/new?issuable_template=UX%20Scorecard%20Part%202)，使用模板 "WIP: UX Scorecard Part 2"，在体验评分之后进行。
    1. 如果您正在执行启发式伙伴评估，跳过此步骤，并继续使用[启发式伙伴计分卡模板](https://gitlab.com/gitlab-org/gitlab-design/-/blob/master/.gitlab/issue_templates/Heuristic%20Buddy%20UX%20Scorecard.md)
1. 按照模板中的指示，完成记分卡并使用评分标准。
1. 一旦你完成了评估并提供了你的建议，就把 "WIP: "的前缀从议题的标题中删除。

如果你想查看或编辑模板，你可以在这里找到它们:

* [Part 1 - UX Scorecard](https://gitlab.com/gitlab-org/gitlab-design/blob/master/.gitlab/issue_templates/UX%20Scorecard%20Part%201.md) 
* [Part 2 - Recommendations](https://gitlab.com/gitlab-org/gitlab-design/blob/master/.gitlab/issue_templates/UX%20Scorecard%20Part%202.md)
* [Heuristic Buddy Scorecard](https://gitlab.com/gitlab-org/gitlab-design/-/blob/master/.gitlab/issue_templates/Heuristic%20Buddy%20UX%20Scorecard.md)

## 评分标准

### 总体体验

| Badge | 总结 | 描述 |
| ------ | ------ | ------ |
| [![Badge level A High Quality/Exceeds](https://about.gitlab.com/images/grade/grade_a.svg)](https://about.gitlab.com/handbook/engineering/ux/ux-scorecards/index.html#grading-rubric) | 超出预期 | 体验超出预期，用户感到体验很愉快。<br/> - 难易程度: *极其容易* <br/> - 体验: *极好* |
| [![Badge level B Meets Expectations](https://about.gitlab.com/images/grade/grade_b.svg)](https://about.gitlab.com/handbook/engineering/ux/ux-scorecards/index.html#grading-rubric) | 符合预期 | 符合预期，但没有超过用户的需求。用户能够达到目标并完成工作。<br/> - 难易程度: *成功* <br/> - 体验: *好* |
| [![Badge level C Average](https://about.gitlab.com/images/grade/grade_c.svg)](https://about.gitlab.com/handbook/engineering/ux/ux-scorecards/index.html#grading-rubric) | 一般 | 用户可以完成工作，但没有超过他们的需求，需要不必要的步骤。<br/> - 难易程度: *成功，但存在不必要的步骤* <br/> - 体验: *尚可* |
| [![Badge level D Poor](https://about.gitlab.com/images/grade/grade_d.svg)](https://about.gitlab.com/handbook/engineering/ux/ux-scorecards/index.html#grading-rubric) | 不太好 | 该体验被看作是一种糟糕的经历，难以完成。 <br/> - 难易程度: *困难* <br/> - 体验: *不好* |
| [![Badge level F Terrible](https://about.gitlab.com/images/grade/grade_f.svg)](https://about.gitlab.com/handbook/engineering/ux/ux-scorecards/index.html#grading-rubric) | 糟糕 | 太多的用户无法完成工作。体验被视为极差，极难完成。<br/> - 难易程度: *极其困难* <br/> - 体验: *极其不好* |
| [![Badge level 0 Unknown](https://about.gitlab.com/images/grade/grade_-.svg)](https://about.gitlab.com/handbook/engineering/ux/ux-scorecards/index.html#grading-rubric) | 未知 | 这项工作还没有被分级。 <br/> - 挫折感: *未知* <br/> - 工作完成情况: *未知* |

## 评估 onboarding 体验

你的产品类别的 onboarding 体验会对 GitLab 的采用阶段产生很大的影响。你可以使用用户体验记分卡来评估 onboarding 体验的用户体验并确定需要改进的地方。

onboarding 可以指许多不同的情况，这可能会影响体验。

* SaaS 或者自助管理版本的用户
* 全新的 GitLab 管理员，建立一个 SaaS 或自助管理版本的账户/实例
* 新加入公司或团队的 GitLab 用户
* 试用用户
* 加入一个公司或团队的 GitLab 的现有用户
* 一个 GitLab 的现有用户在一个新的阶段或类别中尝试一个功能
* 一个 GitLab 功能，一组功能，或一个完整的 DevOps 阶段

例如，一个现有的 GitLab 用户加入一个新的团队，可能需要一些不熟悉的功能的帮助，或者需要熟悉团队中的组和项目。而一个全新的用户则需要更多的帮助来熟悉这个应用程序本身。

### 评估onboarding用户体验的步骤

* 思考与你的JTBD有关的最重要的任务/情景。
* 确定用户第一次执行此任务的场景。
* 对这些任务/场景进行用户体验记分卡或可用性测试，将每个场景合并到一起。
* 将你的评价集中在onboarding[启发式和评分标准](https://about.gitlab.com/handbook/engineering/ux/heuristics/)，对onboarding体验进行评分。
* 记录 onboarding 分数和日期(地点待定)。

如果你有最近的用户体验记分卡或最近的可用性测试的录音，你可以更新这些而不是重新开始。例如，如果你最近做了一个关于创建MR的可用性测试，你可以在考虑到 onboarding 启发式的情况下重新观看这些环节，以推断出 onboarding 体验的初始分数。然而，我们强烈建议你在某个时候有意地评估 onboarding 体验。
