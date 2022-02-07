---
layout: markdown_page
title: "Package 用户体验团队"
description: "Package 用户体验团队支持任何使用 GitLab 来构建、测试和部署软件的人，或者想使用各种包或镜像库来管理依赖关系的人。"
---

## 概述
Package 阶段组负责 GitLab 的[Package 阶段](https://about.gitlab.com/handbook/product/categories/#package-stage)，它与 GitLab 的 [CI/CD 产品](https://about.gitlab.com/direction/ops/) 集成。我们的任务是创建一个安全的环境，在这个环境中，源代码和依赖项都可以存在，允许您在一个地方发布、使用和发现各种语言和平台的包。

Package 设计优先考虑尽可能有效地给我们的用户提供价值。虽然设计是一个适应性的对应团队，但设计过程往往属于两类中的一类：

1. **大规模的愿景** -这个设计过程旨在创建大规模愿景，并与我们的用户验证方向。在此基础上，与更广泛的团队协作，创建并分解为小的MVC迭代。
1. **小规模的设计** - 这种设计过程更注重于满足团队的直接需求，为边缘案例提供解决方案，完善已验证的经验等。在最高层次上，设计集中在三个广泛的领域。

    1.  为存储和访问软件包和容器镜像提供无缝体验，以实现更安全更可靠的构建。
    1.  建立透明、高效的供应链，确保每个人都能做出贡献。
    1.  围绕安全策略和漏洞修复构建工具，同时限制对已知漏洞的暴露

### 我们的客户
我们的客户是任何使用 GitLab 来构建、测试和部署软件的人，或者想利用各种包或镜像库来管理他们的依赖关系的人。这类客户可以是任何规模或特定行业的。另一种客户是一个大型组织，他们在不同的团队中使用几种编程语言，他们希望将所有的外部依赖关系集中在一个地方，即 GitLab。

### 我们的用户
在我们的体验设计工作中，我们考虑了几种不同类型的用户。即使一个用户有相同的头衔，他们的职责也可能因组织规模、部门、组织结构和角色而不同。下面是我们服务的一些角色：

* [系统管理员](https://about.gitlab.com/handbook/marketing/strategic-marketing/roles-personas/#sidney-systems-administrator)
* [软件开发人员](https://about.gitlab.com/handbook/marketing/strategic-marketing/roles-personas/#sasha-software-developer)
* [Devops 工程师](https://about.gitlab.com/handbook/marketing/strategic-marketing/roles-personas/#devon-devops-engineer)
* [安全分析员](https://about.gitlab.com/handbook/marketing/strategic-marketing/roles-personas/#sam-security-analyst) (将来)

### 我们的团队
我们的团队在继续成长。我们目前有2名成员为 Package 用户体验工作作出贡献。

* [Rayana Verissimo](https://gitlab.com/rayana) - 产品设计经理
* [Katie Macoy](https://gitlab.com/katiemacoy) - 产品设计师, Package

#### 我们的团队会议
遵循 GitLab 的传统，我们大部分的交流是通过议题和合并请求完成的。我们确实有一些定期的同步会议：

* 产品管理部和设计部每周召开会议，协调 Package 组的设计工作。
* 前端和设计部门每周都会开会，协调用户界面的改进工作。
* 围绕 CI/CD 的设计师们每隔一周就会开会，协调整个平台的工作。

### SSOT 设计文件
为了提高透明度，Package 用户体验团队为 Package 阶段组内的产品类别创建了单一真实来源（SSOT）。并非所有的类别都有核心的 SSOT Figma 文件。

| 类别 | SSOT 设计文件 | 史诗 |
|---|---| --- |
| [软件包库](https://about.gitlab.com/direction/package/#package-registry) | [Figma File](https://www.figma.com/file/AnBWA0HLLLRWUK6c8oePzv/Package-Registry-SSOT?node-id=1%3A1) | [&3693](https://gitlab.com/groups/gitlab-org/-/epics/3693) |
| [容器镜像库](https://about.gitlab.com/direction/package/#container-registry) | [Figma File](https://www.figma.com/file/kZh5V0YEHoKqZZdqIPF92I/Container-Registry-SSOT?node-id=0%3A1) | [&2899](https://gitlab.com/groups/gitlab-org/-/epics/2899) |
| [依赖项代理](https://about.gitlab.com/direction/package/#dependency-proxy) | [Figma File](https://www.figma.com/file/5LlIZjcgDe9QNNRK2vZEyc/Dependency-Proxy-SSOT?node-id=0%3A1) | [&2920](https://gitlab.com/groups/gitlab-org/-/epics/2920) |
| [依赖防火墙](https://about.gitlab.com/direction/package/#dependency-firewall) | tbd | [&5133](https://gitlab.com/groups/gitlab-org/-/epics/5133) |
| [Help Chart Registry](https://about.gitlab.com/direction/package/#helm-chart-registry) | tbd | [&2281](https://gitlab.com/groups/gitlab-org/-/epics/2281) |
| [发布证据](https://about.gitlab.com/direction/package/#release-evidence) | tbd | [&5135](https://gitlab.com/groups/gitlab-org/-/epics/5135) |
