---
layout: handbook-page-toc
title: "在 Qualtrics 中创建设计评估"
description: "我们在 GitLab 有两种方法来评估设计。每种方法都是通过 Qualtrics 完成的。"
---

经常有这样的情况：团队有一个以上的潜在解决方案，可以满足用户的需求，并且在技术上是可行的。这时的问题是，当两种设计都能解决问题时，如何继续前进。设计评估的目标是确定用户会更喜欢哪种解决方案。

我们在 GitLab 有两种方法来评估设计。每种方法都是通过 Qualtrics（[请求 Qualtrics 访问-内部链接](https://about.gitlab.com/handbook/business-technology/team-member-enablement/onboarding-access-requests/access-requests/)）进行的：
 
* [首次点击测试](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/creating-design-evaluations/#first-click-tests)
* [偏好测试](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/creating-design-evaluations/#preference-tests)


## 如何计划设计评估研究 
在评估设计时，最好先对设计的某个方面[创建一个假设](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/defining-goals-objectives-and-hypotheses/)。 

在确定你的研究目标和目的时，请考虑以下问题：
 
* 你在什么地方最自信和最不自信？
* 在一个设计中包括某些元素与其他变化的结果会是什么？
* 是什么决定了这种设计是否成功？


在确定了你需要测试的内容之后，你就需要确定衡量设计是否成功的方法。这就是设计评估研究的意义所在。

可用性指标帮助你回答关于你的设计的可用性的问题。无论你有关于可寻性或可读性的问题，还是你只是想知道首选方案，可用性指标可以为你的研究勾勒出一个清晰的目标，并改善你的分析。

常见的可用性指标包括：

* 成功率
* 任务完成时间
* 错误率
* 满意度
* 信心程度


NNGroup 有一篇[非常棒的文章](https://www.nngroup.com/articles/usability-metrics/)，可以提供更多关于可用性指标的见解。

## 首次点击测试
首次点击测试检查参与者在界面中首先会点击什么来完成他们的预期任务。它可以在一个正常运行的网站、一个原型或一个线框上进行。它允许你评估你的网站/产品的链接结构的有效性，包括导航，以了解用户是否知道如何绕过并完成他们的预期任务。

### 创建首次点击测试的技巧
* 当创建任务时，专注于为参与者提供一个问题来解决——例如，“你感兴趣的是找出多少……多少……在哪里……”以培养更自然的互动。
* 指示参与者在这部分会议中保持沉默。因为我们要捕捉的是任务时间，所以参与者的任何发言都会影响这个指标。
* 确保你知道并记录了完成每项任务的正确路径，无论是对你自己还是对你的观察员。 这将简化笔记工作。
* 追踪每次点击。
* 计算用户需要多长时间才能完成这次点击。你可以使用 Qualtrics 中的[时间问题](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/question-types-guide/advanced/timing/)来做这个。 花费很长的时间进行第一次点击可能表明导航存在问题，需要进行监控或解决。
* 每项任务结束后，用满意度或信心量表来评估参与者是否觉得他们能够找到正确的信息。
* 接下来，评估完成每项任务的难易程度。 在这里使用反应量表也会有助于分析，但也要考虑自由回答的选项，以提供额外的背景。
* 在启动前彻底试验你的测试，这样你就有时间解决任何问题。
* 最好不要告诉参与者他们正在参加首次点击测试。 

### 如何使用 Qualtrics 进行首次点击测试：
综合使用[描述性文本](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/question-types-guide/static-content/descriptive-text-and-graphic/)、[热图](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/question-types-guide/specialty-questions/heat-map/)和[计时](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/question-types-guide/advanced/timing/)问题类型来创建任务场景并记录受访者对图片的第一次点击。

**步骤 1:** 登录 Qualtrics 后，点击顶部导航中的项目，并点击页面右上方的创建新项目按钮。

![Create a new project](create_a_new_project.png)


*注意：如果您打算从头开始创建自己的调查，首先您应该选择创建一个新的 CoreXM，然后创建自己的调查。

![New CoreXM](Create_new_CoreXM.png)

**步骤 2:** 选择创建一个空白项目，或者复制用户体验研究和产品库中的设计评估调查样本。

![Sample design evaluation survey](survey_template.png)

**步骤 3:** 添加您的问题:

* 使用一个 ***描述性文本*** 问题来设置任务场景。
   * 创建一个新的问卷模块
   * 创建一个新的问题
   * 从修改问题类型的下拉菜单中，选择 "描述性文本"。


* 使用以下步骤来设置一个***热力图***问题。
   1. 创建一个新的问题
   2. 从修改问题类型的下拉菜单中，选择 "热力图"。
   3. 点击 "选择一个图形用于这个问题"。
   4. 选择一个你已经上传到 Qualtrics 账户的图形（或从你的电脑上上传一个新的）。
   5. 设置每个受访者可以对图片进行的点击次数（默认为'1'）。
      * **注意**：如果被调查者的点击次数超过了允许的次数，他们最新的点击将被替换。
        * 如果你计划根据用户的最初直觉来分析数据（仅一次点击），你应该允许一次点击。
        * 如果你想评估多个正确的位置或看到用户的第一次点击和最后一次点击，你应该允许超过一次点击。
   6. 单击 "添加区域"。
      * 添加区域将帮助你更有效地计算出在正确位置点击的用户的百分比。
      * 如果您没有为正确的地点添加区域，那么在 Qualtrics 的数据报告中，所有的点击都会被归类为 "其他"。
      * 区域不是热力图问题的必要条件，但它们可以使报告更容易。
   7. 点击并拖动区域来移动它，或者点击并拖动角落来调整它的大小。
   8. 单击区域下方的文本框，输入区域名称（确保使用描述性的名称，因为该名称不会显示给受访者，但会在您的调查结果中使用）。

![First-click test](first-click-test.png)

* 在您的调查中创建另一个区块，并添加一个文本输入问题，让用户解释他们点击某个区域的动机。例如。你为什么点击那里？(开放文本)
  * 你也可以使用[多选](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/question-types-guide/standard-content/multiple-choice/)问题，让他们评价自己的信心水平。
    * 例子：你有多大把握点击了正确的位置？
      * 完全有信心
      * 有一点信心
      * 中立的
      * 有点不确定
      * 完全不确定



## 偏好测试 
偏好测试通过让用户选择他们的首选方案来帮助你在设计的变体之间进行选择。你可以让受试者根据设计的外观、它传达信息的能力、或者其他能够评估你的假设的品质来选择偏好。参与者并不根据与设计的互动来选择他们的偏好。如果你想根据行动来收集数据，可以进行可用性测试。

偏好测试可以用来评估各种静态设计：图标、单页模拟图、调色板、设计组件等等。值得注意的是，你不应该用这种方法来测试工作流程或任何需要互动的东西。

### 创建偏好测试的技巧:
* 任何使用的视觉效果必须包含完整的背景，以便对设计进行准确评估。
* 截图必须足够大，以便清楚地查看和容易阅读。
* 这些测试通常用于衡量审美吸引力，但也可以指示参与者根据设计的可信度或其传达特定信息或想法的程度来判断。


### 如何使用 Qualtrics 进行倾向性测试:

**步骤 1:** 登录 Qualtrics 后，点击顶部导航中的 "项目"，然后点击页面右上方的 "创建新项目 "按钮。

![Create a new project](create_a_new_project.png)

***注意：如果你打算从头开始创建你自己的调查，首先选择 "创建一个新的 CoreXM"，然后选择 "创建你自己的调查 "***。

**步骤 2:** 选择创建一个空白项目或复制用户体验研究和产品库中的设计评估调查样本。

![New CoreXM](Create_new_CoreXM.png)

**步骤 3:** 添加您的问题:
使用“单一答案，垂直，图形”类型的多项选择题来设置偏好测试。

![Preference Test](preference-test.png)


* 在这个问题之后，再加上一个[文本输入](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/question-types-guide/standard-content/text-entry/)问题，以了解参与者为什么选择那个选项。
   * 问题示例:
     * 你为什么喜欢这种设计?
     * 你为什么选择这个选项?
     * 为什么那个选项看起来是最 [形容词] 的一个？?
