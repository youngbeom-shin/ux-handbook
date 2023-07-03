---
layout: handbook-page-toc
title: "发布用户体验团队"
description: "发布用户体验团队的目标是设计简单明了的方法，使GitLab成为用户在任何地方、任何时间、任何方式进行部署的首选工具。"
---

## 概述

[发布阶段](https://about.gitlab.com/stages-devops-lifecycle/release/)包括所有帮助你保证软件交付的功能，通过自动发布和交付应用程序，缩短交付生命周期，精简人工流程，并加快团队速度。

发布用户体验团队的目标是通过提供软件交付的最佳体验来实现这些复杂的流程。我们的设计任务是把简单、干净的方法带到最前沿，使 GitLab 成为用户在任何地方、任何时间、任何方式进行部署的首选工具。

我们最大的合作伙伴是 Ops 部分 ([验证](https://about.gitlab.com/direction/ops/#verify), [打包](https://about.gitlab.com/direction/ops/#package), [配置](https://about.gitlab.com/direction/configure/) 和 [监控](https://about.gitlab.com/direction/monitor/)), Dev 部分 ([管理:优化](https://about.gitlab.com/direction/dev/#manage-1)), 和 基础设施 ([交付](https://about.gitlab.com/handbook/engineering/infrastructure/team/delivery/)).

### 相关用户体验团队

- [Daniel Fosco](https://gitlab.com/dfosco) - 高级产品设计师
- [Rayana Verissimo](https://gitlab.com/rayana) - 产品设计经理
- [Russell Dickenson](https://gitlab.com/rdickenson) - 高级技术撰稿人
- [Will Leidheiser](https://gitlab.com/wleidheiser) - 高级用户体验研究员

### 稳定的对接方

其他职能团队的以下成员是我们稳定的对接方。

- [Nicole Williams](https://gitlab.com/nicolewilliams) - 研发经理
- [Chris Balane](https://gitlab.com/cbalane) - 高级产品设计师

### 当前的工作重点

了解发布阶段背后的战略和愿景的最好方法是阅读 [部署方向](https://about.gitlab.com/direction/deployment) 手册页。

截至22财年第四季度，我们专注于改善客户的部署体验，实现对部署的更好跟踪和协调，包括：

- [使部署和状态信息在环境页面上更容易阅读](https://gitlab.com/groups/gitlab-org/-/epics/6938)  
- [跨项目共享生产环境](https://gitlab.com/groups/gitlab-org/-/epics/4276)

你可以在 [Release Plan](https://gitlab.com/groups/gitlab-org/-/boards/1489550?label_name[]=devops%3A%3Arelease&label_name[]=group%3A%3Arelease&label_name[]=Next%20Up) 看板上的 `~ready-for-design` 和 `~design` 栏目下看到我们正在进行的 UX 工作，以及正在进行的 [里程碑规划议题](https://gitlab.com/gitlab-org/ci-cd/release-group/release/-/issues?scope=all&state=all&search=%22Planning+Issue%22)。

### Shared UX

从 GitLab 仓库发布代码的用户体验跨越了我们产品的许多领域和页面。为了提供无缝的用户体验，我们的团队包括以下方面:

- 环境
- 部署
- 发布
- 特性开关
- gitlab-ci.yml
- CI 流水线

其他领域和页面也可能包括。 

- 项目设置
- 合并请求
- 基础设施 & Kubernetes
- Runners
- Audit log

更具体地说，发布阶段组负责 GitLab 产品的几个类别，您可以在 [手册页面](https://about.gitlab.com/handbook/product/categories/#release-group) 中看到这些产品。

### 类别用户体验概述

**类别用户体验概述**是对发布组中的类别和功能的介绍，包括其界面和用户体验的例子。你可以观看下面的视频或阅读[本议题](https://gitlab.com/gitlab-org/ci-cd/release-group/release/-/issues/101)中的内容。

这是一个活生生的文档，作为我们的用户体验如何工作的视觉参考，但它不是一个正式的真实来源。会定期审查和更新，但其中一些信息可能已经过时。

{%youtube%}S8iFdfPQmbw{%endyoutube%}

视频中的内容可以在[本期](https://gitlab.com/gitlab-org/ci-cd/release-group/release/-/issues/101)中找到，在那里你可以看到每个功能的链接和截图。Figma 上也有 [完整的可视地图](https://www.figma.com/file/m86hcciGMQJ4RzvVq6Wlnu/Release-Stage---Categories-UX-Overview?node-id=0%3A1)。 

### 我们的用户

我们在设计体验时考虑了不同的用户类型。即使用户拥有相同的头衔，他们的职责也可能因组织规模、部门、组织结构和角色而有所不同。以下是我们所服务的一些人:

- [发布经理](https://about.gitlab.com/handbook/marketing/strategic-marketing/roles-personas/#rachel-release-manager)
- [软件开发人员](https://about.gitlab.com/handbook/marketing/strategic-marketing/roles-personas/#sasha-software-developer)
- [开发技术主管](https://about.gitlab.com/handbook/marketing/strategic-marketing/roles-personas/#delaney-development-team-lead)
- [DevOps 工程师](https://about.gitlab.com/handbook/marketing/strategic-marketing/roles-personas/#devon-devops-engineer)
- [产品经理](https://about.gitlab.com/handbook/marketing/strategic-marketing/roles-personas/#parker-product-manager)
- [质量评估工程师](https://about.gitlab.com/handbook/product/personas/#simone-software-engineer-in-test)

### 用户体验 策略 & 研究

我们将致力于尽可能与开发团队保持共享用户体验的一致，成为与产品经理和其他同行对话的驱动因素。

发布 UX 团队正在一起工作，以发现客户的核心需求，我们的用户工作流程是什么样子的，并定义我们如何使任务变得更容易。我们的策略包括以下行动:

| 策略 | Cadence |
| -------- | ------- |
| Jobs to be Done 框架 | 每季度审查一次 |
| [用户体验记分卡和建议](https://about.gitlab.com/handbook/engineering/ux/ux-scorecards/) | Ad hoc |
| [机会画布](https://about.gitlab.com/handbook/product/product-processes/#opportunity-canvas) | Ad hoc |
| 利益相关者访谈 | Ad hoc |
| 用户和客户访谈 | Ad hoc |

访问 [CI/CD UX](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/ci-cd/) 页面，阅读有关部门的整体战略。

关于我们小组最近一直在进行的所有相关研究，请查看以下链接。

- [Release UX - 研究报告汇编 - FY22 Q3-Q4](https://gitlab.com/gitlab-org/ci-cd/release-group/release/-/issues/92)
- [研究概要 – 共享的环境 & 部署](https://gitlab.com/gitlab-org/uxr_insights/-/issues/1254)
- [Dovetail](https://dovetailapp.com/projects)
- [用户体验研究资料库](https://gitlab.com/gitlab-org/ux-research/-/issues?scope=all&state=all)

### Jobs to be Done

查看所有 [发布阶段](https://about.gitlab.com/handbook/engineering/development/ops/release/jtbd/) JTBDs.

### 团队会议

- **发布组每周**：每周一次，与工程团队开会，调整正在进行的开发工作
- **发布用户体验/ PM 同步**：每周一次，设计师和产品经理之间的会议，以调整当前和未来的设计工作
- **发布用户体验/前端同步**：每两周，设计和前端工程师会面，讨论正在进行的工作并分享反馈。
- **CI/CD 用户体验会议**：每两周一次。会议讨论我们阶段性的用户体验共享工作，审查设计，并迭代我们的战略。

### 关注我们的工作

[Release UX YouTube频道](https://www.youtube.com/playlist?list=PL05JrBw4t0KoyqCjN4f79w0dYZusHLx15)包括用户体验记分卡演练、用户体验审查、小组反馈会议、团队会议，以及更多。
