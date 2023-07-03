---
layout: handbook-page-toc
title: "Qualtrics Tips & Tricks"
description: "How to use Qualtrics at GitLab to run surveys"
---

## 创建一个问卷

1. 选择`空白问卷项目`
1. 为你的项目命名
1. 进入调查问题。在屏幕的右侧，你会发现:
    * [问题类型](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/question-types-guide/question-types-overview/) 和格式 (选择答案的数量，定位等).
    * [验证](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/validation/) (强制受访者回答问题或要求他们在离开页面前考虑回答这个问题).
    * Actions (如[分页符](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/add-page-break/)、[跳过逻辑](https://www.qualtrics.com/support/survey-platform/survey-module/question-options/skip-logic/)和[显示逻辑](https://www.qualtrics.com/support/survey-platform/survey-module/question-options/display-logic/)).
1. 更新你的问卷的 `Look & Feel` .
    * 请参考[Look & Feel 设置](#styling-look--feel-settings)获得指导。
1. 适当调整您的[问卷选项](https://www.qualtrics.com/support/survey-platform/survey-module/survey-options/survey-options-overview/)。
1. 在[工具](https://www.qualtrics.com/support/survey-platform/survey-module/survey-tools/survey-tools-overview/)菜单下，你会发现许多有用的功能，例如:
    * `协作` - 允许您与另一个Qualtrics用户分享您的调查，以便您可以协同编辑或分析结果。
    * `拼写检查` - 只支持英文(美国)。
    * `生成测试反馈` - 在将调查发送给实际参与者之前，为您的调查生成自动的虚拟回答，以查看数据集和报告将是什么样子。
    * `检查问卷的可访问性` - 确定您的问卷对使用屏幕阅读器的受访者来说是否是无障碍的，并接受改进您问卷的无障碍性的建议。
    * `分析问卷` - 对你的问卷打开[专家评审](https://www.qualtrics.com/support/survey-platform/survey-module/survey-checker/quality-iq-functionality/)建议。
    * `导入/导出问卷` - 导入/导出QSF，TXT或DOC文件。
1. 当你完成了你的问卷，`预览` 它，以确保一切都是按照你期望的方式工作。
1. 一旦你准备好启动你的调查，点击`发布`。

## 样式(外观和感官设置)

以下设置应应用于您的问卷:

1. 主题: 空
1. 排版: 现代
1. 通用
    * 进度条: 无文本
    * 进度条位置: 顶部
1. 样式
    * 主要的颜色: #554488
    * 次要的颜色: #554488
    * 字体: Arial   
    * 前景对比度: 中等
    * 问题间距: 紧凑
    * 问题文本: 14px bold
    * 答案文本: 14px
1. 动效
    * 页面过渡: 无
    * 额外的复选框: 取消勾选
1. Logo
    * GitLab First Look Logo (存储在 UX Research library)
    * 样式: Banner
    * 位置: 居左
    * 最大高度: 70px
    * 移动缩放: 66%
1. 背景
    * 背景类型: 颜色
    * 背景颜色: #ffffff
    * 前景的对比: 中等
    * 问题容器: 关闭

## 避免社交媒体的垃圾回复

在社交媒体上发布调查是快速扩大受众的好方法，可以减少研究的时间和成本。然而，请注意，在社交媒体上分享的**调查经常被机器人或假参与者**攻击，在短时间内提交数十或数百个回复，影响数据的完整性和整个研究。**这尤其会影响到有奖调查或在Twitter上分享的调查。**

一些机器人比其他机器人更复杂。例如，一些简单的机器人将“快速”完成调查或对开放式问题提供不合逻辑的回答;更复杂的机器人会故意花更多的时间来完成调查，甚至使用调查本身的语言来对开放式问题进行逻辑回答。没错，有些人为了得到调查奖励而竭尽全力。

不要担心，你可以做很多事情来防止或过滤掉大部分的这些回复。我们说“大多数这些回应”，因为在你的调查中避免垃圾邮件的唯一真正的方法是不要在社交媒体上分享它们，而是[发送带有单个链接的调查邀请的电子邮件](https://www.qualtrics.com/support/survey-platform/distributions-module/email-distribution/emails-overview/#UnderstandingTheIndividualLink)。你可以使用我们的 First look 面板，但只能使用一次。

### 在共享调查之前，防止垃圾邮件回复

在分享你的调查之前，请使用以下方法来防止机器人和虚假参与者。注意,尽管 Qualtrics 有[验证码的问题](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/question-types-guide/advanced/captcha-verification/)和[欺诈检测功能](https://www.qualtrics.com/support/survey-platform/survey-module/survey-checker/fraud-detection/)的帮助,但它们不足以阻止更复杂的机器人。

- 在调查的开始添加[验证码问题](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/question-types-guide/advanced/captcha-verification/)。
- 启用所有[欺诈检测功能](https://www.qualtrics.com/support/survey-platform/survey-module/survey-checker/fraud-detection/):防止多次提交，机器人检测，安全扫描监视器，和近似 ID。
- 添加一个“蜜罐”问题，一个对人类隐藏但对机器人“可见”的问题。有些机器人会回答这个问题，让你可以过滤掉他们或过滤掉他们的回答。
   1. 在你的调查中的某个地方添加一个**可选的**单选题（复选框）。问题和位置并不相关，因为它将被隐藏起来，不被人类发现。例如，"你是人类吗？" `[]是的`。
   1. [添加以下 JavaScript](https://www.qualtrics.com/support/survey-platform/survey-module/question-options/add-javascript/)到该问题，替换现有的`Qualtrics.SurveyEngine.addOnload` function:
      ```js
      Qualtrics.SurveyEngine.addOnload(function()
      {
          jQuery("#"+this.questionId).hide();
      });
      ```
   1. 预览调查表，检查页面加载时问题是否被隐藏。
- 添加一个**必选的**选择题，检查被调查者的注意力和逻辑。例如，直接说明他们应该选择哪个答案，或者问是哪一年。
- 在多项选择题中加入不合逻辑的选项。例如，在问题“您使用这些工具中的哪一个进行代码检查?”“添加像 `[]Tanuki Code` 这样不合逻辑的选项。
- 在调查的两个不同的点问同样的**必选**的问题。试着用简单的多项选择题，人们可以很容易地回答。例如，他们的职位或团队规模。
- 对于以上三种类型的问题，如果你想根据受访者的回答来筛选他们，请参阅[在调查流程中筛选应答者](https://www.qualtrics.com/support/survey-platform/survey-module/survey-flow/advanced-elements/screen-out-management/#ScreeningOutRespondentsInTheSurveyFlow)部分的**调查外的应答者分支部分**。在添加该部分中描述的调查流逻辑之后，然后您可以决定[标记这些响应](https://www.qualtrics.com/support/survey-platform/survey-module/survey-flow/advanced-elements/screen-out-management/#FlaggingScreenedOutResponses)，以供以后分析或[立即丢弃他们](https://www.qualtrics.com/support/survey-platform/survey-module/survey-flow/advanced-elements/screen-out-management/#DiscardingScreenedOutResponses)。

此外，如果你的调查被分享在多个社交媒体渠道上，您可以通过[通过查询字符串传递信息](https://www.qualtrics.com/support/survey-platform/survey-module/survey-flow/standard-elements/passing-information-through-query-strings/#PassingInformationIntoASurvey)跟踪参与者访问调查的来源。如果一个源的垃圾邮件似乎比其他源多，这可以帮助过滤响应。

### 关闭调查后，过滤掉垃圾回复

结束调查问卷后，现在是时候看看预防措施在多大程度上减轻了垃圾邮件的影响，以及我们仍然需要过滤掉哪些回复。[响应质量](https://www.qualtrics.com/support/survey-platform/data-and-analysis-module/data/response-quality-functionality/)功能根据[若干标准](https://www.qualtrics.com/support/survey-platform/survey-module/survey-checker/response-quality/)自动为您标记响应。

- 查看[响应质量](https://www.qualtrics.com/support/survey-platform/data-and-analysis-module/data/response-quality-functionality/#ViewingResponseQuality)报告和[过滤掉响应](https://www.qualtrics.com/support/survey-platform/data-and-analysis-module/data/response-quality-functionality/#FilteringResponsesbyIssue)。
- 如果适用的话，检查对开放式问题的不符合逻辑的回答。
- 檢查那些太快完成调查问卷的受访者。响应质量功能试图[标记 "超速 "响应](https://www.qualtrics.com/support/survey-platform/survey-module/survey-checker/response-quality/#Speeders)，但它只适用于至少有100个响应的调查。
- 检查重复的电子邮件地址（如果适用）。还要注意`@aol.com`、`@yahoo.com`和`@hotmail.com`等经常被用来发送垃圾邮件的电子邮件地址。

## 向GitLab First Look分发调查问卷 

**注意:这些说明只适用于UX研究人员和研究协调员。**

1. 选择 `联系人` (右上角菜单).
1. 选择 `列表` (最左边的菜单).
1. 选择 `GitLab First Look`
1. 选择 `列表选项`
1. 从下拉菜单中, 选择 `从列表中创建样本`. 
1. 给你的样本取一个名字。
1. 选择 你的样本量（你理想中的调查对象的人数）。
    * 明智的做法是先将你的调查发送给一小部分用户测试样本，以确保你能够收到你想要的回应。 
    * 当你将你的调查分发给更多的受众时，为了避免联系那些已经回答了你的调查作为测试样本的一部分的相同用户，请单击 `高级抽样标准`，确保抽样标准声明为。`以下都是真的`，将`联系活动`过滤器改为`调查`，将`选择调查`过滤器改为您已经分发的调查。
1. 点击 `添加取样标准`。
1. 确保抽样标准声明为:`以下所有都是正确的`
1. 选择 `嵌入式数据`，选择一个 `嵌入式数据字段`，选择一个 `操作者` 并输入/选择一个 `嵌入式数据值`。
    * 对于你创建的每个样本，你必须始终为 `阶段组`和 `研究类型` 添加抽样标准。当一个人注册 GitLab First Look 时，他们会指定他们希望收到关于什么的研究（阶段组），以及他们希望参加什么类型的研究。极为重要的是，当你与用户联系时，你只给他们发送与他们的偏好有关的电子邮件。
    * 请记住，`阶段组`和`研究类型`的嵌入式数据可以包含多个值（用户注册时很少会收到关于一个特定阶段组的邮件，或者想参加一种形式的研究）。因此，你的`操作者`将始终是`包含`。
    * 有关哪些嵌入式数据的更多信息，请参考[嵌入式数据](https://about.gitlab.com/handbook/engineering/ux/qualtrics/#embedded-data)部分。
1. 点击 `新条件` 来添加额外的采样标准
1. 一旦你完成输入你的取样标准，点击 `创建`
1. 会出现一个进度条，这表明 Qualtrics 正在建立你的样本
1. 一旦样本准备好，点击 `进入样本`（或者你可以导航到 `列表`，你的新样本将在 `所有列表`下可见。点击您的样本即可进入）
1. 你的样本中的联系人数量将显示在屏幕的左侧
    * [如果你的样本量低于预期，该怎么做？](https://about.gitlab.com/handbook/engineering/ux/qualtrics/#what-to-do-if-your-sample-size-is-lower-than-expected)
1. 如果你对样本中的联系人数量感到满意，你现在就可以向用户发送你的调查。要做到这一点，请进入 `项目`
1. 选择你想分发给用户的项目/调查表
1. 点击 `分布式`
1. 点击 `撰写邮件`
1. 在 `To`字段中，导航到`Group Library:UX Research`->`GitLab First Look`->`Samples`，选择你之前创建的样本。
1. 将 `From` 字段更新为。`firstlook@gitlab.com`
1. 将 `From Name` 更新为`GitLab First Look`
1. `回复邮件`可以是你自己的、个人的 GitLab 电子邮件地址，也可以是`firstlook@gitlab.com`。
    * 如果您打算在休假期间让调查继续进行，请使用`firstlook@gitlab.com`，因为这将自动转发给所有用户体验研究人员，他们可能会在您不在时协助解决任何用户疑问。
1. 将 `When` 字段更新为你想发送电子邮件的时间。
1. 输入你的 `主题行` 
    * 我们在活动中使用的标准主题是:“快，新的研究报告已经出来了”不过，如果你愿意，你可以试试这个。请确保您使用[主题行检查器](https://www.subjectline.com/)来评估您的主题行。
1. 删除出现在WYSIWYG文本区域的标准文本/链接。
1. 点击信息栏旁边的 `加载信息`
1. 导航到 `Group Library: UX Research` 并选择你想使用的模板。
1. 在模板加载后，从 `加载信息`下拉菜单中选择 `使用固定文本`选项。这可以阻止你对模板所做的任何修改被永久保存。
1. 适当地编辑信息文本。
    * 默认情况下，动作调用总是链接到您计划发送的当前项目/调查。正如在 `可用性测试` 和 `用户访谈` 的模板正文中发现的筛选调查文本链接一样。
1. 当你完成了电子邮件的构建，点击 `发送预览邮件` 并输入你的 GitLab 电子邮件地址。电子邮件的副本将被发送给你，供你审查。
1. 如果你对你的电子邮件感到满意，请点击 `发送`。

### 嵌入数据

**注意：这些说明只适用于用户体验研究人员和研究协调员。**

当用户注册到 GitLab First Look 时，我们会自动收集以下嵌入式数据。

1. `阶段组`

    * `1` - 管理
    * `2` - 计划
    * `3` - 创建
    * `4` - 验证
    * `5` - 包管理
    * `6` - 发布
    * `7` - 配置
    * `8` - 监控
    * `9` - 安全
    * `10` - 保护
    * `11` - 启用 & 增长

1. `研究类型` *(在2020年11月删除。这个问题的数据将存在于以前注册的用户，但不存在于新的小组成员。)*

    * `Beta测试`
    * `Cards sorts`
    * `设计评估`
    * `问卷`
    * `可用性测试`
    * `用户访谈`

1. `GitLab 用户` - 此人是否为GitLab用户。

    * `Yes` - 此人是GitLab用户。
    * `No` - 此人不是GitLab用户。

1. `岗位名称` - 此人的工作头衔是什么。

    * `后端工程师`
    * `设计师`
    * `DevOps 工程师`
    * `行政管理 (研发总监, CTO, CEO, 等等)`
    * `前端工程师`
    * `全栈工程师`
    * `基础架构工程师`
    * `运维工程师`
    * `渗透测试`
    * `产品经理`
    * `项目经理`
    * `质量保障工程师`
    * `研究员`
    * `安全分析员`
    * `安全专家`
    * `科学家`
    * `网站可靠性工程师`
    * `软件工程师/开发人员`
    * `学生`
    * `系统管理员/工程师`
    * `失业人员`
    * `其他`

1. `组织规模` - 有多少人在用户的组织内工作？(2019年8月新增)

    * `0-10 人`
    * `11-100 人`
    * `101-500 人`
    * `501-1000 人`
    * `1001-10,000 人`
    * `10,000+ 人`

1. `团队规模` - 有多少人在用户的团队中工作（2019年8月新增）

    * `0 - 只有我一个人！`
    * `1-5 人`
    * `6-10 人`
    * `11-20 人`
    * `21-30 人`
    * `30+ 人`

1. `SaaS (GitLab.com) 版本`

    * `免费版`
    * `高级版`
    * `旗舰版`
    * `不太清楚`

1. `Self managed 版本`

    * `Core`
    * `Starter`
    * `Premium`
    * `Ultimate`
    * `I don't know`

* 这个名单上有什么遗漏吗？请告诉Sarah，她会把它加进去的

* 当使用 `嵌入式数据值` 时，Qualtrics 不会在您开始键入时自动补全该值。搜索功能也可能是杂乱无章的。因此，请确保你完整地输入数值，就像上面显示的那样。

* 嵌入式数据字段过去是区分大小写的。对于绝大多数 Qualtrics 用户来说，嵌入式数据不再区分大小写，这意味着 `Test` 和 `test` 将被视为同一个字段。然而，Qualtrics 仍然建议将匹配案例作为最佳实践，因为有一小部分账户没有进行此更改。

* 并不是所有的嵌入式数据值都是在 GitLab 的 First Look 创建时创建的。因此，我们并不需要为每个用户提供完整的值。值得注意的是，用户的某些值可能会随着时间而改变。例如，有些人可能会换工作，这可能会影响他们的职位、组织和团队规模。因此，我们持有的关于用户的信息可能存在一些差异。我们计划通过定期要求 GitLab First Look 的成员检查并在必要时为他们更新我们的文件信息来降低这种风险。


### 如果你的样本量低于预期，该怎么做？

**注意：这些说明只适用于用户体验研究人员和研究协调员。**

可能有几个原因导致你的样本数低于预期。

1. GitLab First Look 的联系频率已经用完了。默认情况下，GitLab First Look 的成员每周收到的电子邮件不会超过一次，或者一个月收到四次以上。如果是这种情况，你将需要延迟发送你的调查(你可能只需要延迟一天发送你的调查-联系 UX 研究协调员确认)或在 GitLab First Look 之外寻找用户。
1. 没有足够的符合你的采样标准的 GitLab First Look 成员。
1. 你的取样标准有错误。

* 对于选项2和3，导航到你的样本，点击 `列表选项`，选择 `编辑样本` 来改变你的采样标准。

## 向 GitLab.com 的用户分发你的调查问卷

**注意：这些说明只适用于用户体验研究人员和研究协调员。**

在一些研究中，你希望根据一些标准来锁定特定的用户群体（例如，在过去30天内至少撰写了5个合并请求的用户）。如果可以生成一个符合特定标准的用户 ID 列表（通常来自[数据仓库](https://about.gitlab.com/handbook/business-ops/data-team/#-data-warehouse)），你可以使用该列表将这些用户的联系信息推送到 Qualtrics 中，并分发调查问卷。**注意，这只限于GitLab.com的用户，不包括自我管理的用户。**

1. 生成 GitLab.com 用户 ID 列表，并将其放入 Google Sheet 的第一列。第一列（A1）的第一个条目应该是 `id`，因为这证实了这是一个你想使用的 ID 列表。
1. 特定表格(或标签)的名称应该是你想要命名的Qualtrics邮件列表，例如，`05/20 - CI Pipeline Prototype Testing`。**名称不能包含以下字符:`< >`。这样做将导致在转移到 Qualtrics 时出现错误。**
1. 整个电子表格的文件名应该是`qualtrics_mailing_list.`，后面是你在上述步骤中使用的工作表/邮件列表的名称。所以保持我们之前的例子，`qualtrics_mailing_list.05/20 - CI Pipeline Prototype Testing`。
1. 一旦一切准备就绪，将文件移到 `QualtricsRequest` Google Drive 文件夹中。
1. 如果一切操作正确，在大约15分钟内，A1中的`id`条目应该变成`processing`。这意味着数据管道正在处理你的请求。
1. A1将显示 `已处理`。 你的邮件列表现在应该在 Qualtrics 中了。
1. 在文件名中加入 `processed_`，以便明确哪些文件已经完成，同时也使进程在未来尽可能快地执行。
1. 该名单将显示为*UX研究和产品*目录的共享名单。您可以从 Qualtrics 的*联系人*部分访问该名单本身，或者您可以在发送电子邮件的过程中选择该名单。
 
* 你在 Google Sheet 中指定的 GitLab.com 用户 ID 将作为嵌入式数据包含在 Qualtrics 邮件列表中。你可以用它来将你得到的任何回应与你的原始用户列表联系起来。

## 如何创建一个追踪链接

你可能想用几种方法来推广一项调查，并跟踪哪种方法表现最好（例如。GitLab 社交网站、UX 团队社交网站、博客文章或 gitlab.com 内部的 banner）。你可以通过使用查询字符串来做到这一点。阅读[文档](https://www.qualtrics.com/support/survey-platform/survey-module/survey-flow/standard-elements/passing-information-through-query-strings/)，或观看[短视频](https://share.getcloudapp.com/kpumEOvR)。

## 如何从我们的通讯录中删除联系人

用户体验研究协调员偶尔会收到从所有名单上删除联系人的请求。值得注意的是，每个列表都是独立的，所以从一个列表中删除联系人并不会自动从他们可能订阅的其他列表中删除。

UX研究协调员或其他具有 Qualtrics 管理员权限的团队成员必须在全球范围内删除联系人，以防止他们今后收到电子邮件。 

要从你的目录中删除一个联系人。

1. 登录您的Qualtrics账户
1. 点击右上角的 "联系人 "标签
1. 单击 "目录联系人
1. 搜索你想删除的联系人
1. 选择该联系人
1. 选择一个联系人后，选项应显示在页面的右侧
1. 点击扳手图标
1. 选择删除联系人




