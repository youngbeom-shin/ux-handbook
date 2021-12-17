---
layout: handbook-page-toc
title: "Product Design"
description: "We support the business of GitLab by becoming experts in our stage group, educating ourselves about the entire product, and staying engaged with user and business goals"
---

## GitLab 的产品设计

我们支持 GitLab 的业务，成为我们阶段小组的专家，学习关于整个产品的知识，并与用户和业务目标保持联系。我们与产品管理和开发部门的对应人员紧密合作。 


## 团队架构

每个产品设计师被分配到我们产品的一个部分，称为阶段组。他们尽可能地学习关于用户及其工作流程的一切知识，以便为真正的客户问题设计解决方案。

关于产品类别和到团队成员和方向页面的链接的信息可以在[这里](https://about.gitlab.com/handbook/product/categories/)找到。

一些UX团队记录了关于他们的工作方式和阶段性小组的详细信息，这些信息可以在这里找到:

* [Ops](https://about.gitlab.com/direction/ops/) (@gitlab-com/gitlab-ux/ops-ux)
    * [CI/CD](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/ci-cd/) (@gitlab-com/gitlab-ux/cicd-ux)
        * [Verify UX](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/verify/)
        * [Package UX](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/package/)
        * [Release UX](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/release/)
    * Configure and Monitor (@gitlab-com/gitlab-ux/configure-monitor-ux)
        * [Configure](https://about.gitlab.com/direction/configure/)
        * [Monitor](https://about.gitlab.com/direction/monitor/)
* [Enablement](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/enablement/) (@gitlab-com/gitlab-ux/enablement-ux)
* [Sec](https://about.gitlab.com/direction/security/)
    * [Secure and Protect](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/sec/) (@gitlab-com/gitlab-ux/secure-protect-ux)

## 产品设计流程

产品设计师在与稳定的同行进行阶段小组工作时，遵循[产品开发流程](https://about.gitlab.com/handbook/product-development-flow/)中概述的指导。

具体细节：

* [计划和管理能力](https://about.gitlab.com/handbook/engineering/ux/product-designer/#planning-and-managing-capacity)
* [优先级](https://about.gitlab.com/handbook/engineering/ux/product-designer/#priority-for-UX-issues)
* [使用议题工作](https://about.gitlab.com/handbook/engineering/ux/product-designer/#working-on-issues) 
* [设计流程](https://about.gitlab.com/handbook/engineering/ux/product-designer/#product-design-process)
* [与UX Resesarch合作](https://about.gitlab.com/handbook/engineering/ux/product-designer/#product-design-process)
* [与技术写作人员合作](https://about.gitlab.com/handbook/engineering/ux/product-designer/#partnering-with-technical-writers)
* [为 "Pajamas" 做贡献](https://design.gitlab.com/get-started/contribute)

你是一名新的 GitLab 产品设计师吗?如果是这样的话,欢迎你!请务必查看[产品设计师工作流程](https://about.gitlab.com/handbook/engineering/ux/product-designer/)手册页，这将帮助你如何开始。

## 了解用户体验并查看我们的工作

* [展示用户体验的YouTube播放列表](https://www.youtube.com/playlist?list=PL05JrBw4t0Kq89nFXtkVviaIfYQPptwJz) 
* [UX 学习和开发页面](https://about.gitlab.com/handbook/engineering/ux/learning-and-development)

## 设计原则

我们的[设计原则](https://design.gitlab.com/get-started/principles)可以通过睡衣设计系统找到。

## 宏观用户体验

将DevOps的所有阶段集中在一个平台上，可以创造出比单一工具链更好的用户体验。然而，我们知道我们不能止步于此。在我们的产品内部，产品区域之间的工作流必须具有内聚性和连接性，以便用户能够完成更高级别的待完成任务(主要任务)。

### 建议

在22年第四季度，我们将进行一项实验，将一名资深工程师与高级/资深产品设计师配对，以完善现有的工作流程。工程师和产品设计师将一起工作，以确定工作流程中的摩擦领域，他们将通过在配对的同时向产品实时提交合并请求来解决这些问题。被指派的工程师将专注于进行较大、较复杂的产品变更的MR，而产品设计师将贡献较小的CSS更改、文档和设计专业知识。

在实验过程中，团队将关注的初步议题包括:

| 议题                            | 工作流程 | 工程师 | 产品设计师 |
| -------------------------------- | --------   | -------- | ---------------- |
| Auto DevOps                      | TBD        | TBD      | TBD              |
| Kubernetes agent                 | Run, deploy, manage, and observe a container-based application  | Shinya Maeda | Mike Nichols |
| 安装部署体验               | TBD        | TBD      | TBD              |

### 我们将如何衡量成功？

- **被合并的MR:** 使用 `Macro UX` 标签合并的MR总数。 
- **视频介绍:** 在项目开始时，产品设计师将与工程师一起创建一个视频演练，该演练主要关注特定的更高级别JTBD，以及该工作流的当前用户体验如何支持它。在项目结束时，产品设计师将创建一个视频演练，展示改进的体验。

### 风险
- 我们不知道这些配对在实验过程中需要多少时间才能成功，所以我们无法预测对参与者的常规里程碑工作、okr等的影响。
- 实验的重点是修复启发式审查中发现的摩擦点，这意味着我们不会进行用户研究。我们有可能在无意中引入新的摩擦点。
- 第四季度实验确定的主题不是我们在用户研究中经常听到的项目，因此，在实验过程中，我们很可能将重点放在那些不会提高我们的整体产品可用性得分的领域上，正如[SUS](https://about.gitlab.com/handbook/engineering/ux/performance-indicators/#system-usability-scale-sus-score)所衡量的那样。

