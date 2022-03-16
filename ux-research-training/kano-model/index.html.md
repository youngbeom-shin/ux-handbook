---
layout: handbook-page-toc
title: "卡诺模型与功能优先度调查"
description: "卡诺模型提供了一种简单而强大的方式来思考我们计划建立的功能。"
---

## 卡诺模型

卡诺模型是一种将产品开发与用户满意度联系起来的理论。
它是由 Noriaki Kano(狩野纪昭) 教授于 20 世纪 80 年代在日本开发的。
<!-- TODO: Mention that 卡诺 model theory originated in the same atmosphere as other theories that influenced DevOps movement -->
卡诺模型根据产品功能的开发对用户满意度的影响，将产品功能分为五类:

- **Must-be**:对于最初的采用来说非常重要，但却不能带来高满意度的功能，无论你在这些功能上投入多少。
- **Performance**:(又称一元化)没有这些是一个问题，满意度会随着投资的增长而增长。
- **Attractive**:这些都是不错的功能，但如果你执行得好，用户满意度就会直线上升。
- **Indifferent**:投资于这些功能不会增加或降低用户满意度。
- **Reverse**:没有这些功能实际上比有它们更好。

<!--TODO: Change the list to a diagram -->

一旦你知道你的功能属于哪一类，你就可以优先考虑最重要的功能进行开发。
理论上说，来自 Must-be 类别的功能应该被优先考虑，其次是 Performance，然后是 Attractive。
在实践中，可能有很好的理由遵循不同的类别顺序，或者根据功能在多个类别中的得分来单独确定其优先级。

<!-- TODO: Explain that it is a model – a simplification -->

参考资料:更多信息请查阅 Daniel Zacarias 的 [《卡诺模型完整指南》](https://foldingburritos.com/kano-model/) 或维基百科[卡诺模型](https://en.wikipedia.org/wiki/kano_model)条目。


### 为什么使用它？

使用卡诺模型可以帮助您在从待办事项列表中确定功能的优先级时做出更明智的决定，并更好地理解为什么这些功能能或不能与您的用户产生共鸣。

### 如何使用它？

卡诺模型最好从用户数据中形成，特别是当它为功能的优先次序提供信息时。
为了收集这些数据，我们建议进行一项研究，并使用作为卡诺模型理论的一部分而开发的标准化调查问卷（[详情见下文⬇️](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/kano-model/#standardized-questionnaire)）。
从研究的角度来看，为卡诺模型研究设计一份调查是相当简单的，然而它需要产品经理做大量的准备工作--特别是描述产品领域的特点和现状。
在下面几段中，我们将讨论组织这样一项研究的细节。

## 功能优先级调查

<!-- TODO: Add a section about issues structure for such a project -->

项目示例:[CI 功能优先级调查](https://gitlab.com/gitlab-org/ux-research/-/issues/1027)

项目摘要。*该团队正在考虑建立 12 个他们认为会使我们的用户受益的新功能。 由于建立新功能的成本和时间都很高，团队希望了解用户对每个功能的感受，以及优先级的确定。 我们的目标是要更清楚地了解团队应该首先建立哪 12 个功能。*

### 准备工作

精心设计的功能描述对于研究的成功至关重要。
参与者必须能够准确地理解你所询问的功能以及这些功能的价值，这样他们才能提供诚实的反馈。
只有在记录了功能之后才开始创建调查问卷是有意义的。

#### 类别描述

我们通常在已经存在的功能的背景下开发新的功能。
出于这个原因，你应该首先带领参与者了解包含所介绍的功能的现有经验。

**类别描述的例子：**

> GitLab 中的持续集成流水线被定义为项目的 Git 仓库中的一个版本控制文件。这个文件被称为 "gitlab-ci.yml"，用户通过编辑这个文件并将其推送到仓库中来配置 CI 流水线。流水线由工作和阶段组成。工作定义了流水线应该做什么。阶段由一个或多个作业组成，定义了作业运行的顺序。一个阶段的所有作业都是平行运行的，如果所有的作业都成功，流水线就会进入下一个阶段。可以为流水线指定不同类型的条件，如先决条件、例外情况等。你可以通过本地克隆项目或使用在线文本编辑器来编辑流水线 YAML 文件。

#### 功能描述

当创建功能描述时，请遵循以下原则:

1. 描述功能，而不是 mvc
   - 研究结果应该在相当长的时间内具有相关性。换句话说，你很可能无法在1或2个里程碑中开发它。
1. 使用简单、中性的语言
   - 没有像是 `sections`, `categories`这样的GitLab术语
   - 没有像 `易于使用`, `更好`, `更高效`这样的宣传口号
1. 将功能设置到系统的上下文中
   - 使用一致的术语，确保你的功能描述符合整体类别描述。
1. 争取每项描述都有一段文字
   - 少于 1 个正常段落可能是不够的。另一方面，如果文本太长，参与者将更有可能跳过它。
1. 只包括新的功能
   - 包括已经开发的功能可以设定一个基准；然而，它大多不具有可操作性，因此在这种情况下没有用处。
1. 用图片或 GIF 丰富描述内容

**功能描述示例:**

> CI 作业代码片段的列表，将显示在在流水线编辑器旁边。你使用这些代码片段作为你的流水线的构件，从这个列表中复制工作 YAML 并将其粘贴到你的流水线代码中。这将加快创建新流水线的速度并减少错误。

<details>
  <summary markdown="span">**更多特功能述实例**</summary>
  <figure class="video_container">
     <iframe src="https://docs.google.com/document/d/e/2PACX-1vQff1-XyGoZeWaAyHhANrPjIQ54WXX8Je06_DzIsUtMK6ZQ6IhzMrvM3PGdXJLzu_Q9Z0Jz_5W41FCm/pub?embedded=true"></iframe>
  </figure>
</details>

<!-- TODO: Create & add a feature descriptions doc template -->

<!-- TODO: Add a feature description structure recommendation – https://gitlab.com/gitlab-org/ux-research/-/blob/8abb8170124572620ff719760cf67fb8d8e7a79a/Survey%20about%20requirements%20for%20monitoring/Feature%20description%20guidelines.md#feature-description-structure -->

#### 技巧和窍门

💡**技巧**: 为调查做准备可能需要很多时间，而且可能很难跟踪。创建一个单独的问题（就像[这个议题](https://gitlab.com/gitlab-org/ux-research/-/issues/1143)）来跟踪这项工作，将减轻主要研究问题的负担，并将使谁是DRI更加明确。

 💡 **技巧**: 以异步方式准备功能描述会花费很多时间。如果你觉得你的团队进展不够快，[转为同步交流](https://about.gitlab.com/company/culture/all-remote/asynchronous/#when-to-pivot-to-synchronous)。

### 问卷

#### 标准化的调查问卷

卡诺模型的标准化问卷由两个问题组成，针对你感兴趣的每个功能进行提问。

<table style="width:100%">
  <tr>
    <th>功能性问题</th>
    <th>功能紊乱的问题</th>
  </tr>
  <tr>
    <td>
      <p>如果你<b>拥有</b>这个功能，你会有什么感觉？</p>
      <ul>
        <li>我对它感到很高兴</li>
        <li>我期待它</li>
        <li>我是中立的</li>
        <li>我可以容忍它</li>
        <li>我对它感到很沮丧</li>
      </ul>
    </td>
    <td>
      <p>如果你<b>没有</b>这个功能，你会有什么感觉？</p>
      <ul>
        <li>我对它感到很高兴</li>
        <li>我期待它</li>
        <li>我是中立的</li>
        <li>我可以容忍它</li>
        <li>我对它感到很沮丧</li>
      </ul>
    </td>
  </tr>
</table>

**Note**: 在[！28](https://gitlab.com/gitlab-org/ux-research/-/merge_requests/28)中，我们对答案选项做了一些调整，因为在试行期间，原来的答案被证明是难以理解的。关于这个决定的更多细节，请见[本线程](https://gitlab.com/gitlab-org/ux-research/-/merge_requests/28#note_382934909)。

使用标准化问卷的好处是，基本上所有的研究设计都已经完成，你可以重复使用以前的研究。 另外，采取一致的方法来处理这种方法，可以减少在这个过程中引入错误的风险。

<details>
  <summary markdown="span">**研究计划的范例**</summary>
  <figure class="video_container">
     <iframe src="https://docs.google.com/document/d/e/2PACX-1vRi6Dq6sDBtkggW5oEnmkTsLGx6WRvKrs8EV4aXaAhIlEpOgykK2PJEEp8uj2UfEymbQgLJYBVavR1c/pub?embedded=true"></iframe>
  </figure>
</details>

<!-- TODO: Create & add a research plan template -->

#### 结构调查表

使用 Qualtrics 创建问卷。每个带有相关问题的功能都应该放在一个单独的块上。

<!-- TODO: Add a diagram of survey structure -->

示例: 我们在[#1027](https://gitlab.com/gitlab-org/ux-research/-/issues/1027)中使用过 [问卷](https://gitlab.eu.qualtrics.com/jfe/preview/SV_3VoczISwBuK8ab3?Q_CHL=preview&Q_SurveyVersionID=current)

<!-- TODO: Review and mention a survey block template -->

#### 数据收集与分析

使用所提供的调查问卷，你将能够收集数据，分析数据，并使用定量和定性方法报告出调查结果。

##### 定性方法

这种方法可以让你更好地理解他们优先级背后的 _原因_ 。 另外，先收集和分析定性数据可以帮助你发现功能描述中的问题，在把它们发给很多人之前，你可以先解决这些问题。
我们建议进行 5 到 10 次有主持的会议或 20 到 30 次无主持的会议，在这些会议中，参与者的任务是通过问卷调查并解释他们答案背后的原因。

<!-- TODO: Add example UserTesting project -->
<!-- TODO: Add example Dovetail project -->
<!-- TODO: Add example of outcome -->
<!-- TODO: Ask Nels if you can embed video with him -->

##### 量化方法

我们建议从你的目标受众中收集 50 到 80 个用户的反馈，并使用 Daniel Zacarias 的文章[the Complete Guide to 卡诺 Model](https://foldingburritos.com/kano-model/)中描述的离散分析对他们进行分析。
这种方法将为您提供“数字”，支持您的优先级决定，但您仍然缺乏对优先级背后的理解。

<!-- TODO: Add example spreadsheet -->
<!-- TODO: Find out if you can publish a spreadsheet. If yes, anonymize it and embed to this page -->
对于分析，请使用这个电子表格模板。[卡诺模型：<类别>功能优先排序调查](https://docs.google.com/spreadsheets/d/14D-ayhw15J9o7ixzFh7pda_SZQkhZTRsyJvHi_5JXbk/edit?usp=sharing)

<!-- TODO: Explain that this type of analysis is not statistically sound and that we have to come up with something better -->
<!-- TODO: Add example of outcome -->

采取定量和定性的方法，将使数据背后的故事更加完整。除了确定优先次序外，你也能解释参与者为什么会有这样的得分。
将这两种方法结合起来，可以使你的卡诺模型研究得到最大的收益。

#### 技巧和窍门

💡 **技巧**: 如果问卷不是太长，而且你还有一些其他问题想问，请随时在最后为这些问题再加一个块。

## 资源
- 文章[卡诺模型完全指南](https://foldingburritos.com/kano-model/) 作者：Daniel Zacarias
- 维基百科条目[卡诺模型](https://en.wikipedia.org/wiki/kano_model)
- 文章 [卡诺模型--使用和不使用的方法](https://medium.com/design-ibm/kano-model-ways-to-use-it-and-not-use-it-1d205a9cf808) 作者：Cary-Anne Olsen-Landis
- 视频 [使用卡诺模型建立一个成功的用户体验战略](https://www.youtube.com/watch?v=Hr1rN3jibIk&feature=youtu.be) 作者：Jared Spool

## 在 GitLab 中的研究实例
- [监测功能的优先次序](https://gitlab.com/gitlab-org/ux-research/-/merge_requests/28)
- [CI功能的优先次序](https://gitlab.com/gitlab-org/ux-research/-/issues/1027)
- [威胁洞察力功能的优先排序](https://gitlab.com/gitlab-org/ux-research/-/issues/1295)

<!-- TODO: Use GitLab terminology – category, group -->
