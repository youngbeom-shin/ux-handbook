---
layout: handbook-page-toc
title: "Usability testing"
description: "Conducting usability testing at GitLab"
---


可用性测试是评估具有代表性用户的产品体验的过程。目的是观察用户如何完成一组任务并了解他们遇到的任何问题。由于用户执行任务的方式经常与预期不同，因此这种定性方法有助于揭示用户为何以他们的方式执行任务，包括了解他们的动机和需求。在 GitLab，可用性测试是[解决方案验证](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/solution-validation-and-methods/)的一部分。



## 不同类型的可用性测试

一般来说，我们可以区分为:

**适度与非适度可用性测试**

湿度可用性测试会有一个主持人在场，他将指导参与者完成任务。这让参与者能够就自己的体验进行交流，并帮助参与者在遇到困惑时帮助答疑。

Conversely, users complete [unmoderated usability](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/unmoderated-testing/) tests on their own without the presence of a moderator. This is helpful when you have a very direct question.

| 适度的可用性测试                                                                                                                                                                                         | 无节制的可用性测试                                                                                                                                                       |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 复杂的问题/关于“为什么？”之类的问题，例如：<br><br>  ““为什么用户在使用某个功能时会遇到问题？””<br>  “为什么用户不能成功使用某个功能？”<br>  “用户如何开始使用某个功能？” | 比较直接的问题，例如：<br><br>  “用户是否找到了完成任务的切入点？"<br> “用户是否认识新的 UI 元素？”<br> “用户更喜欢哪种设计选项？” |

**形成性与总结性的可用性测试**

形成性可用性测试是用于发现可用性问题的持续评估。它们的范围往往更小，例如专注于产品的一个特定功能或只是其中的一部分。通常情况下，原型用于评估。. 

总结性可用性测试的范围往往更大，并与实时产品一起运行。如果您缺乏有关用户为什么遇到特定问题的详细信息，或者想首先验证它的易用性，那么它就会很有用。. 

## 进行可用性测试的步骤
1. [创建你的研究问题](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/defining-goals-objectives-and-hypotheses/#step-1---start-thinking-of-a-problem).
2. 确定您希望在可用性测试中关注的任务. 
    - 当涉及到要包含多少任务时，没有什么神奇的数字。指导方针是有 [3 - 4 个任务](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/writing-usability-testing-script/#tasks), 因为这可以确保参与者不会感到疲倦。另一个需要考虑的方面是，无节制的测试会话最长应为 15 - 20 分钟，有节制的会话最长不超过 60 分钟。 
    - 编写任务时要记住的关键是 [这些任务反映了真实的用户目标](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/writing-usability-testing-script/#tasks). 在创建任务时考虑 JTBD 有助于将注意力集中在用户目标上。 参考 [编写优秀的任务](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/writing-usability-testing-script/#tasks) 里面包含有范例. 
3. 定义成功.
    - 在与用户进行测试之前，请在利益相关者之间就成功的样子达成一致，例如您的目标完成率。 例如，大于 80% 的完成率转化为 Complete 或 Lovable [CM 计分卡 等级](https://about.gitlab.com/handbook/engineering/ux/category-maturity-scorecards/#calculating-the-cm-scorecard-score). 
4. [确定您的目标受众并开始招募。](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/recruiting-participants/).
5. [准备您的原型或演示环境。](https://about.gitlab.com/handbook/engineering/ux/category-maturity-scorecards/#step-2-prepare-your-testing-environment).
6. [编写您的测试脚本，包括要收集的任务和指标。](https://docs.google.com/document/d/1_5Qu2JR9QE5LE6cK4eq9yJs-nXv2rlWWifcjacaiWdI/edit).
    - [国际标准化组织 (ISO) 对可用性的定义](https://www.iso.org/obp/ui/#iso:std:iso:9241:-11:ed-2:v1:en) 侧重于 [3 个因素：有效性、效率、满意度](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/usability-testing/#3-factors-to-measure). 在设置可用性测试时，我们建议捕获 [下面显示的指标](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/usability-testing/#3-factors-to-measure), 因为这将有助于随着时间的推移一致地衡量改进并 [评估它们对系统可用性的影响](https://about.gitlab.com/handbook/engineering/ux/#system-usability). 您可以衡量许多其他指标来了解可用性问题，例如错误率或用户需要帮助的次数。如果您发现它们对您的研究课题有帮助，请随时使用它们。
    - 提醒参与者在完成任务时大声思考，尤其是在无节制的测试中。
    - 关于如何编写出色的可用性测试脚本可以看看这些 [更详细的提示和技巧](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/writing-usability-testing-script/) 
    - 如果您运行未经审核的可用性测试，请使用或参考UserTesting.com 中提供的 [可用性指标模版](https://app.usertesting.com/test_plan_templates/11481/edit) UserTesting.com提供了与我们类似的任务成功和难度指标选择，但这些指标与我们研究所需的可用性指标不同。请使用此模板中列出的选项。
    - 如果你运行一个非适度可用性测试，它将在5分钟内运行，在构建测试计划时切换“短测试”选项。
7. [运行试点会话来测试可用性测试。](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/writing-usability-testing-script/#3-test-the-test).
8. [分析您的研究数据](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/analyzing-research-data/)
    - 对于每项任务，综合有多少用户成功或失败以及他们失败的原因。 
    - 对于每项任务, 计算参与者完成它的容易程度或困难程度。 了解他们给出对应分数的打分模式。
    -  计算 [SUS 形容词评分量表](https://uxpajournal.org/determining-what-individual-sus-scores-mean-adding-an-adjective-rating-scale/) 的平均分数, 并寻找他们给出对应分数的打分模式. 
    - 记下您的任何其他有趣的观察结果。 
9. [用Dovetail记录你的观点。](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/documenting-research-findings/). 如果你有可操作的见解，确保它们也被记录在[极狐GitLab UX Research](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/research-insights/#how-to-document-actionable-insights)项目中.
10. 决定接下来的步骤
    - 任何 [可行的见解](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/research-insights/#actionable-insights) 都需要后续跟进. 和您的同事共同针对已确定的可用性问题进行优先级排序。 记住请进行另一项可用性研究以验证您提出的解决方案。

### 3 衡量因素

#### 1. 有效性
- 测量什么?  
    - 有效性可以通过计算通过率来确定。这显示了每个任务的成功或完成率。
- 它是如何测量的？
    - 通过率可以通过将能够完成任务的参与者数量除以参与者总数来确定。
    - 确保您也在观察和记录参与者失败的原因。
- 我们为什么要测量它？
    - 我们希望用户成功实现他们的目标。了解它们失败的原因和位置将有助于我们改善体验。

#### 2. 效率
- 测量什么？
    - 可以通过了解参与者认为任务的难易程度来衡量效率。 这可以通过为每个任务询问一个 [难易度问题](https://about.gitlab.com/handbook/engineering/ux/category-maturity-scorecards/#the-3-questions-we-ask) 来完成。
- 它是如何测量的?  
    - 在每项任务后询问难易度问题。 
       - *“总的来说，这个任务是……”* <br> *- 非常困难* <br> *- 困难* <br> *- 不算困难也不简单* <br> *- 轻松* <br> *- 非常轻松* <br> *“为什么?”*                                       
    - 确保您在让参与者评价易用性后立即询问为什么参与者会以这种方式评价它。
- 我们为什么要测量它？
    - 主观感知的任务难度是我们在 CMS 期间收集的。收集它作为可用性测试的一部分，为以后的 CMS 研究提供预测和脉冲检查。
    - 了解参与者给出评级的原因很重要，尤其是在评级较低的情况下。当参与者数量也很少时，这在可用性测试中尤为重要。

#### 3. 满意度
- 测量什么？
    - 满意度可以用来了解并确定参与者眼中任务或者体验的友好程度
- 它是如何测量的？ 
    - 完成所有任务后，请参与者根据 [形容词评分量表](https://uxpajournal.org/determining-what-individual-sus-scores-mean-adding-an-adjective-rating-scale/) 对体验进行评分。
       - *“总的来说, 我将该产品的用户体验友好度评分为:”* <br> *- 印象中最坏* <br> *- 糟糕的* <br> *- 欠缺的* <br> *- 尚可* <br> *- 好的* <br> *- 卓越的* <br> *- 印象中最好*
    - 确保您在让参与者对体验进行评分后立即询问为什么参与者会以这种方式对其进行评分。
- 我们为什么要测量它？
    - 该分数与 SUS 高度相关， 我们的目标是 [提高系统可用性](https://about.gitlab.com/company/strategy/#2-build-on-our-open-core-strength).
    - 了解参与者给出评级的原因很重要，尤其是在评级较低的情况下。当参与者数量也很少时，这在可用性测试中尤为重要。

## 可用性测试如何与类别成熟度记分卡（CM 记分卡）相关联
在您进行 [类别成熟度计分卡](https://about.gitlab.com/handbook/engineering/ux/category-maturity-scorecards/#intro-and-goal) 之前进行可用性测试. 可用性测试有助于确定用户在使用 极狐GitLab 时遇到的大多数问题、这些问题的原因以及它们的影响，因此我们知道需要改进的地方。

如果您在没有事先进行可用性测试的情况下运行 CM 记分卡，您可能会发现用户遇到的一些可用性问题。然而，与类别成熟度记分卡相关的努力和严谨客观地衡量产品的当前成熟度并不能证明跳过可用性测试是合理的。
此外，在可用性测试期间，您有机会直接与参与者互动并深入了解他们的行为和问题。 类别成熟度记分卡流程不允许此类交互，因为它旨在捕获不偏不倚的指标和真实的的用户情绪。



## 经常问的问题

**为什么我不应该在用户测试中询问参与者是否成功完成了任务？**
这是参与者自己认为的一种判断，可能正确也可能不正确。如果参与者表示他们成功完成了任务，您仍然需要根据您对成功的定义来检查他们是否真的完成了任务。重要的是只从用户那里获取必要的数据，并考虑到您需要用实际行为仔细检查他们的反应，我们建议首先将其排除在外。

**为什么我不应该使用 UserTesting.com 的本地任务度量_难度_来评估效率？这不一样吗？**
UserTesting.com 的任务度量_难度_类似，但它使用的评分量表与 Single Ease Question 不同。目前，没有选项可以将 UserTesting.com 中的比例标签改成与我们的一致。 



