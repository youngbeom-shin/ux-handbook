---
layout: handbook-page-toc
title: Jobs to be Done (JTBD) Overview
description: >-
  JTBD is a framework for viewing products and solutions in terms of jobs
  customers want to achieve. It's about understanding the goals that people want
  to accomplish.
---

#### On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## JTBD Overview

JTBD 是一个框架, 用于从客户试图实现的工作角度看待你的产品和解决方案。 这是关于了解人们想要实现的目标。它让我们从我们的业务中退后一步，了解我们所服务的人的目标。它打开了创新之门。

在 GitLab，我们有自己的 JTBD 风格，并在整个设计过程中使用它，但最值得注意的是:

- 定义范围
- 验证方向
- 评估现有经验
- 评估类别成熟度

JTBD直接来自于研究和与那些完成我们需要设计的任务/工作的人的客户对话。[问题验证](/handbook/engineering/ux/ux-research-training/problem-validation-and-methods/#what-is-problem-validation) 是确定编写JTBD的最有效方法之一。

### 更多关于 JTBD

深入了解我们的JTBD理念:

- [JTBD 的深入研究](/handbook/engineering/ux/jobs-to-be-done/deep-dive/)
- [什么是 JTBD，什么不是](/handbook/engineering/ux/jobs-to-be-done/deep-dive/#what-is-a-jtbd)
- [JTBD 核心原则](/handbook/engineering/ux/jobs-to-be-done/core-jobs-to-be-done-principles/)
- [如何创建工作图](https://about.gitlab.com/handbook/engineering/ux/jobs-to-be-done/mapping-jobs-to-be-done/)

请观看以下视频，了解为什么JTBD对于产品开发过程如此重要:

{%youtube%}H6j1Xd4yufI{%endyoutube%}
For a quick how-to, follow the below guidance.

### JTBD术语

首先，让我们设置用于JTBD的术语。

- **工作**: 客户想要完成的事情。例如，GitLab客户的主要工作可以表述为："构建和部署软件"。这项工作总是以动词开头。
- **工作执行者**: 执行这项工作的人。通常情况下，我们用角色/用户画像来谈论这些人。他们是 [买家](/handbook/marketing/strategic-marketing/roles-personas/#buyer-personas), [developers](/handbook/marketing/strategic-marketing/roles-personas/#sasha-software-developer), [sysadmins](/handbook/marketing/strategic-marketing/roles-personas/#sidney-systems-administrator), [and so on](/handbook/marketing/strategic-marketing/roles-personas/#personas).
- **工作陈述**: 一篇简明扼要的陈述，把工作的环境、目标和结果结合起来。
- **任务**: 完成一项工作过程中的一个步骤。
- **需求**: 工作的需求。这些可以是系统、业务或用户的需求。例子可能包括快速、廉价、高效、更少、更多、必须有、应该有这样的词。
- **场景**: 描述一个人需要完成工作时所处的环境。
- **结果**: 工作执行者在做某项工作时期望的最终状态和/或感觉。

### 如何编写 JTBD

我们使用标准的格式来写我们的工作声明。

**"当[场景]时，我想[工作]，这样我才能[结果]。."**

JTBD 是很难做好的。在你开始之前，你必须清楚地了解某人想要实现的目标，而且这种了解应该通过过去的研究和客户的对话来验证。

确保工作陈述是基于经验而不是理论是至关重要的。我们必须对自己的工作陈述有高度的信心，才能将其付诸实践。

#### 快速提高信心的方法

- 参考以前的研究和行业标准。
- 进行 [生成性问题验证研究](/handbook/engineering/ux/ux-research-training/problem-validation-and-methods/#when-to-use-problem-validation) (广义问题).
    - 例如，提出诸如“告诉我您作为软件工程师做什么”之类的问题。
- 进行简略的30分钟的工作面试，至少有5名参与者（直接提问）。
    - 例如，根据JTBD问一些问题，比如“告诉我您最近一次创建多阶段pipeline是什么时候。哪些方面做得好？哪些地方不太顺利？"
    - 用以下方法记录你的采访 [JTBD 访谈笔记模板](https://docs.google.com/spreadsheets/d/e/2PACX-1vSX5b57MKfLFl59TfiN61rWNkm2Qctb8cVy40JUGsF6FyEcy3jhPBUxY-4D3exXxqXPwwBkcSOb0HT8/pub?output=xlsx)

### JTBD、用户故事和任务

任务陈述不同于用户故事和任务。它们被设计成与角色、产品和解决方案无关，并且与用户故事和任务有密切的关系。这使我们能够更深入地思考背景，而不仅仅是一个有目标的角色。

_示例:_

**工作:**

帮助我 **做出有效的架构决策**.

**工作陈述:**

当我的开发生态系统开始成熟时，我希望全面了解我的组织的注册表和具体的包的使用情况，这样我就可以做出有效的架构决策。


**任务:**

查看我们使用的软件包列表。

在其最基本的形式中，你将有一个与一个或多个用户故事相关联的工作陈述，这些用户故事是由多个任务组成的。你会在设计过程中的不同时刻使用这些任务。

职位描述提供了主要目标的一个高层次的观点。当您创建线框时，用户故事将指导您的解决方案，任务将成为完成任务所需的步骤。

如果你想详细了解工作说明书的每个部分，请了解更多关于 [JTBD 的结构](/handbook/engineering/ux/jobs-to-be-done/deep-dive/#how-do-i-structure-a-jtbd).

#### 确定JTBD的范围

工作陈述可以写在不同的层次或高度。在我们的大部分工作中，我们在为功能或相关功能集设计体验时为阶段组编写工作陈述。

JTBD 还可以为阶段或跨阶段工作编写，以帮助确定长期的产品方向。

如果你要为你的阶段组写一份工作说明书，请考虑这个指导原则来确定合适的高度：如果该工作适用于3个以上的用户类型，那么很可能是高度设置得太高了。

### 优先考虑JTBD

我们经常发现一个类别有许多JTBD。使用 [用户研究](/handbook/engineering/ux/jobs-to-be-done/prioritizing-jobs-to-be-done) 来帮助确定哪些JTBD对我们的用户来说是最重要的，这有助于规划未来的研究、设计和产品需求。