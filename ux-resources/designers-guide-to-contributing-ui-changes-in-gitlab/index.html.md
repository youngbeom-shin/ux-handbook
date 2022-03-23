---
layout: handbook-page-toc
title: "How to do UI Code Contributions"
description: "There are multiple opportunities to improve GitLab by doing small UI text changes or small CSS refactorings."
---

#### On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## 为GitLab的主代码库做贡献

GitLab的主代码库包含 [GitLab 项目](https://gitlab.com/gitlab-org/gitlab)的所有代码，包括其用户界面。做出贡献需要技术知识，但不一定要对编程概念有深刻的理解才能做出有意义的贡献。有很多机会可以通过对 UI 文本的小改动或对 CSS 的小重构来改进 GitLab。

为GitLab的代码做贡献需要 HTML、CSS、终端（CLI）和 Git 知识。我们也鼓励具备基本的 Ruby 和 JavaScript 知识。

任何为 GitLab 的主代码库做贡献的人都应该有一个正在运行的 [GDK](https://gitlab.com/gitlab-org/gitlab-development-kit)，熟悉使用代码编辑器（最好是 [Visual Studio Code](https://code.visualstudio.com/)） 并知道基本的Git命令。

一般来说，一个问题如果它能在浏览器的检查器中被修复，那么它就可以在 GitLab 代码库中被真正修复。 

我们鼓励大家发现小的UI问题，并通过 [合并请求（MRs)](https://docs.gitlab.com/ee/user/project/merge_requests/) 提交他们的修改。 

## GitLab的主要代码库贡献基础知识

### 第1步：安装GDK

[GitLab Development Kit](https://gitlab.com/gitlab-org/gitlab-development-kit) (GDK)提供了一个本地的 GitLab 实例，允许您在您本地设备上测试更改。

1. [了解如何准备您的设备以运行 GDK](https://gitlab.com/gitlab-org/gitlab-development-kit/-/blob/main/doc/prepare.md)
1. [了解如何运行 GDK](https://gitlab.com/gitlab-org/gitlab-development-kit/-/blob/main/doc/index.md)
1. [GDK命令备忘单](https://gitlab.com/gitlab-org/gitlab-development-kit/-/blob/main/HELP)

### 第二步：了解 GitLab 的代码库结构

三种文件处理用户界面的渲染。GitLab 的核心是一个 Ruby on Rails 应用程序。Rails 上的Ruby应用通过 `.haml` 文件来渲染 GitLab 的前端。HAML（HTML抽象标记语言）是一个基于 Ruby 的 HTML 模板系统。它很容易学习，它甚至可以为你关闭 HTML 标签!

对于样式表，GitLab 使用了一个名为 SASS 的 CSS 预处理器。SASS（Syntactically Awesome Style Sheets）使用 `.scss` 文件来处理所有常见的CSS功能，但更复杂一些，有助于我们保持 GitLab 的 CSS 更有条理。

最后，对于交互性和客户端应用逻辑，GitLab 使用了一个叫做 Vue.js 的框架。除非你改变一个 [Pajamas](https://design.gitlab.com/) 组件，或创建一个新的组件，否则很少需要改变 `.vue` 文件。

### 第3步：选择一个代码编辑器并开始进行小的修改

你可以选择任何你喜欢的代码编辑器，但 Visual Studio Code 是一个安全的选择和行业标准。

一旦你安装了你的代码编辑器，打开 **gitlab-development-kit/gitlab** 文件夹。它包含了所有的 GitLab 文件，这些文件在添加新功能和贡献时都会发生变化。

一个好的起步是在产品中找到一些要更新的文本。使用代码编辑器中的**搜索功能**，找到代码库中存在的文本，将文本改为其他内容，并保存文件。当你重新加载 GitLab 的本地实例时，你应该看到 UI 中反映的变化。

## 贡献 UI 代码修改的步骤指南

关于如何针对 GitLab 的主代码库进行 UI 代码修改的详细步骤指南，请访问此页面。
[一步一步地进行代码修改的指南](https://about.gitlab.com/handbook/engineering/ux/ux-resources/designers-guide-to-contributing-ui-changes-in-gitlab/)

### 关于如何寻找机会做UI代码贡献的展示视频

{%youtube%}GUTalaJt_qU{%endyoutube%}


<hr>

## 为GitLab UI（组件系统）做贡献

[GitLab UI](https://gitlab.com/gitlab-org/gitlab-ui) 是我们的 [Pajamas](https://design.gitlab.com) UI组件库的源代码。它构建和部署了 [Vue.js](https://vuejs.org/) 组件，这些组件被用于我们的一些 GitLab 项目，包括 [gitlab.com](https://gitlab.com/gitlab-org/gitlab)。虽然不要求 GitLab 的设计者对 GitLab UI 进行编码或积极贡献，但对它的作用以及它如何部署我们设计的组件有一个基本的了解是很重要的。

### GitLab UI基础知识

* GitLab UI 构建和部署了组件。然后我们将这些组件导入到整个 gitlab.com 中使用。
* 如果你曾经创建过一个利用 [npm](https://www.npmjs.com/) 的网站或应用程序，你就会像使用其他npm包一样，使用 `npm install @gitlab/ui` 来[安装 GitLab UI 作为一个包](https://www.npmjs.com/package/@gitlab/ui)。由于我们的组件是在Vue中构建的，你的项目也需要基于 Vue 才能使用 GitLab UI 组件。
* 我们使用 [Storybook](https://gitlab-org.gitlab.io/gitlab-ui/?path=/story/base-button--default) 进行开发和组件文档，然后在 [Pajamas](https://design.gitlab.com/) 的组件页面上显示。
* 我们使用[视觉回归测试](https://gitlab.com/gitlab-org/gitlab-ui#visual-regression-tests)来防止在组件上的 CSS 和布局变化引入意外回归。在向GitLab UI合并请求提交修改后，运行手动作业 `update_screenshots` 来检查视觉回归并自动更新。

![Update screenshots manual job](https://about.gitlab.com/images/ux/update_screenshots.png)

### 更新一个现有的 GitLab UI 组件

如果你正在更新一个现有的组件，如果你改变或删除了目前在 gitlab.com 上使用的属性，可能会出现问题。在这种情况下，你需要在 [gitlab repo](https://gitlab.com/gitlab-org/gitlab) 上创建一个集成测试合并请求，以更新现有的组件，这些组件可能会因为你的 GitLab 用户界面的改变而变得破损。幸运的是，这和运行手动作业 `create_integration_branch` 一样简单。

![Create integration branch job](https://about.gitlab.com/images/ux/create_integration_branch.png)

* 运行这个手工作业后，点击它，你会看到一个链接，从创建的集成分支创建一个合并请求。打开这个链接，创建你的合并请求。

![Integration branch MR](https://about.gitlab.com/images/ux/integration_branch_mr.png)

一旦合并请求被打开，它将使用你的 GitLab UI 分支作为 GitLab UI 的源代码，允许你更新那些你可能已经改变或删除的现有组件的属性。

![MR gitlab-ui source](https://about.gitlab.com/images/ux/mr_gitlabui_source.png)

如果你在本地查看 [Storybook](https://gitlab-org.gitlab.io/gitlab-ui/?path=/story/base-button--default) 以查看你的 GitLab 用户界面的变化，你可以选择复选框 `Include GitLab CSS bundle` 来拉入 GitLab 的主 CSS 文件，看看是否有组件的样式会被覆盖掉。如果在选择这个复选框时存在样式差异，你可能会因此得到流水线失败的结果。

![Include GitLab CSS bundle](https://about.gitlab.com/images/ux/include_gitlab_css.png)

**注意：**不要害怕向 [GitLab UI维护者](https://about.gitlab.com/handbook/engineering/projects/#gitlab-ui)寻求建立集成测试的帮助。

### 关于更新 GitLab 用户界面的展示视频

{%youtube%}WWwQ2-UtWRg{%endyoutube%}

## 终端(CLI)备忘单

* 在我们的 GitLab 文档中立的[命令行基本命令](https://docs.gitlab.com/ee/gitlab-basics/command-line-commands.html) 。
* 在我们的 GitLab 文档里的[Git基本命令](https://docs.gitlab.com/ee/gitlab-basics/start-using-git.html#basic-git-commands) 。

## 视频演练

#### [向 GitLab 贡献(设计师版)](https://www.youtube.com/embed/SSo97VwVn4Y&feature=youtu.be) 作者[Annabel Dunstone Gray](https://gitlab.com/annabeldunstone)。

{%youtube%}SSo97VwVn4Y{%endyoutube%}

<hr>

#### [如何在 GitLab 更改 UI 文本(设计版)](https://www.youtube.com/embed/AEv3XFw0xJQ&feature=youtu.be)由[' @jj-ramirez '](https://gitlab.com/jj-ramirez)。

{%youtube%}AEv3XFw0xJQ{%endyoutube%}

<hr>

#### [更新已弃用的按钮](https://www.youtube.com/embed/AEv3XFw0xJQ&feature=youtu.be)由[' @aregnery '](https://gitlab.com/aregnery)。

{%youtube%}dqazqqwvnOs{%endyoutube%}

---

本页面改编自[精美的设计PDF](https://gitlab.com/gitlab-org/gitlab-design/-/blob/master/misc/infographics/How_to_Contribute_UI_Code_to_GitLab.pdf)，由[' @jj-ramirez '](https://gitlab.com/jj-ramirez)创建😃
