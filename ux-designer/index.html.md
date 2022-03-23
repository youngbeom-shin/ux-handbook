---
layout: handbook-page-toc
title: Product Designer Workflow
description: "Here are some guidelines to help Product Designers manage their work at GitLab"
---

#### On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Planning and managing capacity

Product Designers are responsible for work assignments in their stage group and at the UX department level. These include supporting community contributions to their stage group, contributing to the [Pajamas Design System](https://design.gitlab.com/), reviewing other designers work, and more (see [Priorities](#priorities)). Product Designers are responsible for working with their stage peers and managers, as needed, to manage their capacity and complete their work on target and on time. Here are some guidelines to help Product Designers manage their work:

**Product Designers**

- Make sure discipline peers are aware of UX team assignments, such as UX OKRs, and what you'll need from them to succeed.
- Account for time off (both yours and others) as best you can during milestone planning.
- Let your manager know right away, if you believe you're not trending to complete your work. The sooner your manager knows, the higher the likelihood they can resolve the issue and manage expectations.
- Optionally, use UX issue weights to better learn your capacity and facilitate conversations with your Product Manager.

**Product Design Managers**

- If requested by Product Designers, help them set a baseline capacity for stage- and UX-team-assigned work each milestone. Product Designers can use this information to balance work and manage expectations.
- Quantify strategy work with clear time-to-complete (TTC) expectations, measurable goals, and deadlines.
- Resolve team questions, concerns, and blockers quickly.
- Make sure cross-functional partners are aware of UX OKRs and their associated dependencies.

### Priorities

You're encouraged to prioritize your work in the following order, but the actual prioritization depends on various aspects, such as your stage group's workflow.

1. Merge request (MR) reviews, including community contributions. See [MR Reviews guidelines](#mr-reviews).
1. Other designers' feedback requests. These can be in issues, MRs, Figma, the [`#ux-coworking`](https://gitlab.slack.com/app_redirect?channel=ux_coworking) Slack channel, or elsewhere. See related sections [Design Reviews](#design-reviews) and [Investigate possible dependencies](#investigate-possible-dependencies).
1. Issues in the current release milestone and labeled `Deliverable`.
1. Issues assigned to you labeled `workflow::problem validation`, `workflow::solution validation`, or `workflow::design`.
1. [UX OKRs](/company/okrs/).
1. Issues in the next release milestone.
1. Issues in the current release milestone and labeled `Stretch`.
1. Issues labeled `Pajamas`, `pajamas::create`, `pajamas::build`, `pajamas::style`, or `pajamas::integrate`.
1. Issues labeled [`Accepting merge requests`](https://gitlab.com/groups/gitlab-org/-/issues?state=opened&label_name%5B%5D=Accepting+merge+requests&label_name%5B%5D=UX)
1. Issues in future milestones, after the next release milestone. For example, in the milestones [Next 2-3 months](https://gitlab.com/groups/gitlab-org/-/issues?state=opened&milestone_title=Next+2-3+months&label_name%5B%5D=UX), [Next 3-6 months](https://gitlab.com/groups/gitlab-org/-/issues?state=opened&milestone_title=Next+3-6+months&label_name%5B%5D=UX), or [Backlog](https://gitlab.com/groups/gitlab-org/-/issues?state=opened&milestone_title=Backlog&label_name%5B%5D=UX).
1. Popular issues with no milestone (number of comments or upvotes).
1. [Other issues labeled `UX`](https://gitlab.com/groups/gitlab-org/-/issues?state=opened&label_name%5B%5D=UX)

### UX Issue Weights

Issue weights are optional, but weighting issues can be useful for planning. They enable Product Designers to understand their capacity, evaluate impact of time off, facilitate trade-off conversations with Product Managers, and help the Product Design Manager identify teams that need more UX support.

When weighting issues, we aim for [velocity over predictibility](/handbook/engineering/#velocity-over-predictability). This means that we don't need to be accurate at first, we just need to get better. This paragraph has a [useful explanation of estimation](/handbook/engineering/development/growth/product-intelligence/#estimation) at GitLab.

#### How to Use UX Issue Weighting

1. Review upcoming issues and think about how you would break down the work.
2. Use the chart below to assign an issue weight. If you don't know enough about the issue to add a weight, you can work with the Product Manager to get more clarity.
1. Record your issue weight. There are a few ways to do this, so check with your team to see what they prefer:
    - Use Google docs to list issues and corresponding weights
    - Create a linked issue for the UX work and add a weight to the issue. This issue will be closed after UX work is finished, so that the issue weight won't count toward the engineering team's issue weights.
    - Use the [design-weight labels](https://gitlab.com/gitlab-org/gitlab/-/labels?utf8=%E2%9C%93&subscribed=&search=design-weight).
1. When planning an iteration or a milestone, communicate your capacity and the total issue weights you have assigned to yourself. You can use the template below if you like.
1. After you finish a milestone, do a review. Were your weights accurate? Were you over or under in estimating your capacity? Use this mini-retrospective to improve your planning.


**Additional Notes:**

- Most other UX issues, including research and Pajamas related issues could be weighted, if desired.
- When determining capacity, take into account visual reviews, meetings, and other responsibilities which aren't typically weighted.
- Really small issues where the weight would be less than 1, don't need to be weighted.
- A weight of 8 or 13 indicates that the issue is probably too large.
- If unplanned work is added during a milestone, the Product Designer can add a weight and discuss trade-offs with their Product Manager.


> Milestone Capacity Template:
>
> - **Total weights completed last milestone:** 10
> - **Average capacity (average of weights completed last 3 months):** 10
> - **Estimated capacity for current milestone:** 7 (use your average capacity and subtract planned time off)
> - **Total current weights:** 10


#### UX Weight Definitions

| Weight | Design Tasks | User Research Tasks |
| ------ | ------------ | ------------------- |
| 1 | Mostly small UI changes leading to small incremental UX improvements. No users’ workflow involved in these changes. Requirements are clear and there are no unanswered questions. <i>For example: A copy experiment or changing a button styling.</i> | Synthesizing previous research findings and generating recommendations based on them. |
| 2 | Simple UI or UX change where we understand all of the requirements but may need to find solutions to known questions/problems. These changes should blend in with an actual user workflow. <i>For example: [Simplify Sign in / Register process the in trial flow](https://gitlab.com/gitlab-org/growth/product/-/issues/1471)</i>. | Running a first click test or other type of unmoderated research study |
| 3 | A well-understood change but the scope of work is bigger. Several pages are involved and/or we're starting to design/redesign small flows or connect existing flows between each other. Designers may conduct extensive background research (previous issues, support tickets, review past user research, review analytics, etc). Some unknown questions may arise during the work. <i>For example: [Update the CustomersDot checkout page to allow subscription and billing information input](https://gitlab.com/gitlab-org/growth/team-tasks/-/issues/96), [Experiment with adding a contact sales option in app](https://gitlab.com/gitlab-org/gitlab/-/issues/197235)</i>. | A moderated, narrowly scoped research study with specific questions to answer, such as a usability review of a single page |
| 5 | A complex change where input from group members is needed as early as possible. Spans across multiple pages, and we're working on medium-sized flows that potentially connect with another area of the product There are significant open questions that need to be answered. The product designer may need to do some research on their own or in collaboration with a researcher, but this isn't always the case. Possible research activities might be to find and/or validate a Job To Be Done, conduct user testing or card-sorting, or do a survey. <i>For example: UX Scorecard, [How can we improve the dismiss action in upgrade moments](https://gitlab.com/gitlab-org/gitlab/-/issues/213344)</i>. | A research study evaluating the usability of an end-to-end flow or multiple related features, or a usability study with a minor exploratory component |
| 8 | Complicated changes introducing a new user flow that connects with other large flows and may require input from other designers, product managers, or engineers from the same or another stage group. This is the largest flow design/redesign that we would take on in a single milestone. This requires research where the designer may or may not be working with a researcher to plan and conduct exploratory interviews or user testing sessions. <i>For example: [Onboard new signs up through an onboarding issue board](https://gitlab.com/gitlab-org/growth/product/-/issues/107)</i>. | An exploratory study investigating broad-based behaviors related to a single stage, including one or more distinct user groups |
| 13 | Highly significant changes impacting multiple user flows, a large new feature, and/or a complete redesign. This issue could significantly impact product strategy and would require critical input from others (the wider GitLab community, e-group, customers), and there are many unknowns. This necessitates research where the designer could team up with a researcher and other designers to gather input data, plan and conduct exploratory interviews, lead user testing sessions… It's unlikely we would commit to complete this issue in a milestone, and the preference would be to further clarify requirements and/or break it into smaller issues planned in several milestones. <i>For example: [An improved free trial sign-up experience for GitLab.com SaaS users](https://gitlab.com/groups/gitlab-org/-/epics/377)</i>. | An exploratory study investigating broad-based behaviors across multiple stages and multiple types of users, potentially involving team members from the different stages. |

## Working on issues

This section provides an overview of how we work with issues. But it's very important for you to communicate with your PM and EMs early and often about how you should work together. Many teams have different flavors of this process as they have adapted to the needs of that product and that team.

### Triaging UX issues

Every Product Designer at GitLab is empowered to triage issues with "~UX", ["~UX debt"](/handbook/engineering/workflow/#ux-debt) and ["~UI polish"](/handbook/engineering/workflow/#ui-polish) labels, or should be included for feedback by the responsible PM and EM instead. Use [Priority labels](/handbook/engineering/quality/issue-triage/index.html#priority) to propose the time in which the issue should be solved and [Severity labels](/handbook/engineering/quality/issue-triage/index.html#severity) to communicate its impact on users. Always work to align and communicate with your PM and EMs on the labels assigned.

### Scheduling issues in a milestone

All issues in a milestone labeled [`Deliverable`](https://gitlab.com/groups/gitlab-org/-/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name%5B%5D=UX&label_name%5B%5D=Deliverable) that need UX will be assigned to a Product Designer by the kickoff. Issues labeled [`Stretch`](https://gitlab.com/groups/gitlab-org/-/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name%5B%5D=Stretch&label_name%5B%5D=UX) may or may not be assigned to a Product Designer by the kickoff. Learn more about how we use Workflow labels in the [GitLab Docs](https://docs.gitlab.com/ee/development/contributing/issue_workflow.html).

#### Communicating scheduled UX issues to the stage group

Consider adding a `User Experience` section to your team's planning issues ([example 1](https://gitlab.com/gitlab-org/ci-cd/release-group/release/-/issues/53#user-experience-roller_coaster), [example 2](https://gitlab.com/gitlab-org/ci-cd/release-group/release/-/issues/59#research-sleuth_or_spy)), which can include issues related to active design items for that given milestone such as research projects, UX debt, UI polish, or Pajamas components. Learn more about [planning and capacity](/handbook/engineering/ux/ux-designer/#planning-and-managing-capacity) for product designers.

Having design problems added to the planning issue help make design efforts discoverable for the rest of the team and encourages cross-functional collaboration during `workflow::problem validation`, `workflow::design` and `workflow::solution validation`.

Other key benefits of making `User Experience` an official part of group's milestone planning include:

- Advocating for the value of UX within the stage group by making it part of the monthly team planning discussions.
- Using the planning issue with the Product Manager during the milestone kickoff recording.
- Communicating the current design and research efforts at a regular cadence to customers and counterparts outside the stage group area.
- Communicating the Product Designer's agreed capacity to the rest of the team.
- Reinforcing the desire for counterpart collaboration as early as possible within the design phase.

### Product design process

### Define the opportunity

- Work with your PM to [validate](/handbook/product-development-flow/#validation-goals--outcomes) _who_ you're designing for, _what_ you're designing, and _why_ you're designing it.
- Help your PM express the who/what/why as a user story. For example, "As a (who), I want (what), so I can (why/value)." If you’re asked to implement a non-evidence-based how, then ask the PM to refocus on the who/what/why, so everyone can work together to find the best how.
- Help your PM to define [MVC](/handbook/product/product-principles/#the-minimal-viable-change-mvc) success criteria, prioritizing MVC “must-haves” and non-MVC “should-haves” and “could-haves.” (Note that this success criteria is subject to change based on new learning from the iterative design process and customer feedback.)

### Before you design

#### Generate ideas

Part of the role of product designers is to lead and facilitate idea generation within our teams. We are all very busy working with PMs to drive forward our product roadmaps and solve known UX problems, but remember there are also undiscovered problems out there that are definitely worth solving. Here are a few activities and resources to inspire you!

- Run a sync (such as a [ThinkBig!](/handbook/engineering/ux/thinkbig/) session), async, or combination workshop to generate ideas. Define a scope and invite  participants from product, engineering, ux research, and other areas for best results.
- Reach out to [sales](/handbook/sales/), [customer success](/handbook/customer-success/) or [marketing](/handbook/marketing/corporate-marketing/) counterparts for a new perspective. You can also invite these counterparts as optional attendees to your regular meetings.
- Prioritize a round of [problem validation research](/handbook/engineering/ux/ux-research-training/problem-validation-and-methods/) together with Product Managers and UX research. Talk to customers about their experiences building software in a very open-ended way, see what keeps them up at night, what slows them down, and what impedes their productivity.
- Discover unknown pain points:
    - [Dovetail](/handbook/engineering/ux/dovetail/) is used to analyze data, collaborate on insights, and as our current research repository.
    - [Chorus.ai](https://www.chorus.ai/) is a tool used by sales reps that records and transcribes sales calls. You can search calls by keyword to narrow in on what you listen to.
    - [Zendesk](https://gitlab.zendesk.com/agent/) is also a source of information around existing problems, although it can be a bit harder to parse through the tickets, as they aren't necessarily categorized in a way that is optimal for UX.

[Access instructions for Dovetail, Zendesk and Chorus.ai](/handbook/engineering/ux/ux-research-training/ux-research-resources/#how-to-find-existing-research)

- The [community forum](https://forum.gitlab.com/c/questions-and-answers/) is a support option for free users.

#### Understand the space

- Investigate whether there is existing UX Research in the [UX Research Archive](https://gitlab.com/gitlab-org/uxr_insights), [Dovetail](https://dovetailapp.com/), or other data that could help inform your decisions and measure results. If there isn't existing UX Research, contact your [UX Researcher](/handbook/engineering/ux/ux-research-training/how-uxr-team-operates/) to conduct (or guide you and your Product Manager in conducting) research for the problem.
- Consider conducting competitive analysis to inform your work. Look for terminology, functionality, and UX conventions that can help refine success criteria. Only stray from industry conventions with strategic intent, such as capitalizing on [disruptive innovation](https://www.economist.com/the-economist-explains/2015/01/25/what-disruptive-innovation-means) opportunities. We want users to migrate from other tools to ours, and they’re more likely to be successful and satisfied when our products use conventions that are familiar based on other tools they've used.
- Consider creating user flows or journey maps to help ensure you've considered the entire workflow and also to help communicate that workflow to your team.

#### Investigate possible dependencies

It is our responsibility as Product Designers to research how our work can impact other parts of the product and the work that other Product Designers are doing.

- Proactively reach out to other Product Designers (using Slack, Weekly UX Sessions, etc.) to get background information on the product area you are about to start working on and to learn how your product area depends and interacts with others.
- Identify the [DRI](/handbook/people-group/directly-responsible-individuals/) for the product area you're about to start working on, and involve them in your design process from the beginning. If you are unsure who the DRI is, visit the [Product Categories Handbook page](/handbook/product/categories/).
- Check the [Product Kickoff Review](https://about.gitlab.com/direction/kickoff/) to see the list of issues that are currently planned for next release in other stages.

### Ideate and iterate

Iterative design at GitLab combines the two industry-standard definitions of "[incremental design](https://medium.com/@saadiam/incremental-design-12a260f024ae)" and "[design iteration](https://en.wikipedia.org/wiki/Iterative_design)." Put simply, iterative design is the process of breaking down design solutions into the smallest change possible that improves the user's outcome. It's getting things quickly into the product to get feedback early and guide refinement.

When applying iterative design, you should consider the longer-term strategy or vision and work with your Product Manager to plan successive releases until it's realized.

- Share design ideas in the lowest fidelity that still communicates your idea. To keep the cost of change low, only increase fidelity as design confidence grows and implementation requires.
- Ask for feedback from your PM throughout the design process to help refine your understanding of the problem and solution criteria.
- Engage engineering peers early and often. Their insight into technical costs and feasibility is essential to determining viable designs and MVCs. Also, invite design feedback, especially if you’re solving for a development workflow they’re familiar with.
- Ask for feedback from other Product Designers in [Design Reviews](#design-reviews) to help improve your work. At minimum, you'll get objective feedback and new ideas that lead to better solutions. You might also get context you didn’t know you were missing, such as GitLab-specific or industry-standard design conventions.
- Collaborate with your group's Technical Writer when the work involves substantial UI text, such as user-assistance or links back to documentation. For details on how to collaborate, see the [UI text Planning and authoring](/handbook/engineering/ux/technical-writing/workflow/#ui-text) section of the Technical Writing handbook. Additionally, involve your technical writer in the [review process](#technical-writer-ui-text-reviews) for smaller copy changes, such as UI elements labels.
- For a significant UX change, like a new workflow or feature, include your Product Design Manager in feedback sessions, as they might have input into the overall direction of the design or knowledge about initiatives on other teams that might impact your own work.
- If the team does not have a high level of confidence in a direction, there are multiple design solutions, or the direction is a significant risk, [validate](/handbook/product-development-flow/#validation-phase-4-solution-validation) your proposed solution with customers/users by leveraging [ux research methods](/handbook/engineering/ux/ux-research-training/solution-validation-and-methods/). If the team has a high level of confidence in a direction or design solution and the risk is low, it's fine to gather feedback from customers only after releasing the MVC.
- Think through how your design will look and function at multiple viewports, devices, and user preferences. **Note:** It is not required to design for [dark mode](https://docs.gitlab.com/ee/user/profile/preferences.html#dark-mode) while it is an [alpha](https://about.gitlab.com/handbook/product/gitlab-the-product/#alpha) feature. Improving dark mode is on the [UX Foundation direction page](/direction/ecosystem/foundations/) as an item that will be worked on later. Until [Pajamas](https://design.gitlab.com/) components are integrated in the product and the underlying design strategy is in place to support dark mode, we cannot guarantee that bugs and debt will not be introduced to this mode. It is at the discretion of the individual stage group to determine which, if any, dark mode patches are created when working on deliverables.

#### GitLab Design Talks: Iteration

<!-- blank line -->
<iframe height="315" width="560" src="https://www.youtube.com/embed/0lhjzU-QZ2w?start=286&amp;end=359"></iframe>Think big, ship small, move fast with iteration

<blockquote>
"Our relationship with uncertainty: When we conduct research and design we have some level of certainty about how effective it’s going to be, but it isn’t until we ship it and get it in the hands of many users that we truly understand how effective the thing is that we designed."
</blockquote>

<!-- blank line -->
<iframe height="315" width="560" src="https://www.youtube.com/embed/VrXQiik3Q9U?start=244&amp;end=334"></iframe>A new designer's take on iteration

<blockquote>
"Breaking things down creates psychological safety for me as a designer."
</blockquote>

### Design Reviews

Sharing work and gathering feedback can happen at any time within the design process. We do this most frequently by sharing mocks and having open discussions in issues.

Design Reviews are a dedicated space for Product Designers to give and receive specific and sometimes in-depth feedback on ideas and possible solutions. Other benefits include:

- Discover what others are working on.
- Identify any overlapping work.
- Help surface opportunities for where group work should overlap.
- Encourage the practice of sharing ones work.

We [default to asynchronous](/handbook/values/#bias-towards-asynchronous-communication) design reviews so everyone can participate. Asynchronous Design Reviews are very similiar to their synchronous equivalent: designers share their work and provide context so their peers can offer valuable and constructive feedback. Product Design Managers are encouraged to coordinate Design Reviews on a regular candence with their teams.

In practice, this is what it means for designers:

1. Identify one issue where you have many open questions or the one you're most excited to work on.
1. Decide what the best format is to give others a glimpse into the work you need feedback on: It could be anything from an issue, a short text blurb, screenshots, a Figma file, or a short, up-to 5-minute walkthrough recording of the problem you are trying to solve.
1. Remember to share the customer problem, known constraints, and what kind of feedback you need. Be specific about what you want feedback on and also what you do not want feedback on, and where you want the feedback to be provided. Read more about [employing multimodal communication](/handbook/communication/#multimodal-communication).
1. Post your item with a short description to the [`#ux-coworking`](https://gitlab.slack.com/app_redirect?channel=ux_coworking) Slack channel and any other channel where you'd like to get feedback (e.g. your Groups channel, etc.). Be sure to provide a link to the item requiring review as well as a link to the location where feedback should be left. Capturing feedback in issues will ensure you can refer back to it later, whereas Slack messages will eventually disappear.
  1. If you're recording a video it's recommended to default to using Zoom as your recording tool and then uploading the video to our [GitLab Unfiltered](https://www.youtube.com/channel/UCMtZ0sc1HHNtGGWZFDRTh5A) YouTube channel. Set the visibility to "Public" (unless your video contains confidential information), and add it to the "UX" playlist (and any other relevant playlists). For more information, see our [YouTube uses and access](/handbook/marketing/marketing-operations/youtube/) page.
  1. If you're using any other tool to record your video, it should also be uploaded to our [GitLab Unfiltered](https://www.youtube.com/channel/UCMtZ0sc1HHNtGGWZFDRTh5A) YouTube channel. Set the visibility to "Public" (unless your video contains confidential information), and add it to the "UX" playlist (and any other relevant playlists). For more information, see our [YouTube uses and access](/handbook/marketing/marketing-operations/youtube/) page. 
1. Comment on your feature issue with a link to the video and links to all references made ([example](https://gitlab.com/gitlab-org/gitlab/-/issues/217355#note_435285696)), such as related issues, epics, or Figma files. Also add those reference links to the video's description, so that everyone can follow and participate ([example](https://www.loom.com/share/f99878181fe7429d8c0a9d94bfd8b943)).
1. You can also open an issue dedicated to capturing feedback ([example](https://gitlab.com/gitlab-org/gitlab/-/issues/241511)), and attach all references and information needed for review within the issue description. This will allow the threads to focus solely on providing and discussing feedback. Attach this issue as related to the main feature issue.
1. Don't forget to mention any specific Product Designers and counterparts you think your work may relate to.

**Examples**
- [Add a new list iteration - feedback request](https://gitlab.com/gitlab-org/gitlab/-/issues/284610)
- [Swimlane boards loading states - Skeleton loaders feedback request](https://gitlab.com/gitlab-org/gitlab/-/issues/277240)
- [Right issuable sidebar patterns feedback request](https://gitlab.com/gitlab-org/gitlab/-/issues/270117)
- [Geo: Maintenance mode design](https://gitlab.com/gitlab-org/gitlab/-/issues/201757)

### Partnering with Technical Writers

Any additions or changes to UI text require review by the group's Technical Writer, though you may have already discussed plans and ideas during the Product Design phase.
This includes button or menu labels, error messages, user-assistance microcopy, and any other text that may be surfaced in the UI.

- Ensure the issue and MR have the [UI text](https://gitlab.com/gitlab-org/gitlab/-/issues?label_name%5B%5D=UI+text) label.
- Message the [Technical Writer for the group](/handbook/engineering/ux/technical-writing/#designated-technical-writers) in the MR to request a review, including any specific files or lines they should review, and how to preview or understand the location/context of the text from the user's perspective.

### Partnering with UX Researchers

UX Researchers work closely with Product Managers and Product Designers to ensure research projects are focused and provide answers to design questions.

- Ensure you follow the [process to request research](/handbook/engineering/ux/ux-research-training/how-uxr-team-operates/#how-to-request-research) (even if you are conducting the research yourself)
- Ensure you follow the process to [document research findings](/handbook/engineering/ux/ux-research-training/documenting-research-findings/)


### Refine MVC

- UX issues have a tendency to expand in scope. Work with your PM and developers to revisit which aspects of the design are “must-haves” versus those that can be pushed until later. Document non-MVC concepts and research in new issues, marking the new issues as related to the original issue. If you’re ever unsure how to split apart large issues, work with your Product Design Manager.
- If developers need to begin before you have validated your designs, and a planning pivot to another validated UX issue or perhaps dev debt issues is not an option, then look for high confidence and low risk changes devs can start work on while you validate the remainder of the solution. To mitigate these scenarios, PMs and UXers should work together to [get 1-2 months ahead](/handbook/product-development-flow/#validation-track), so that the Build track always has well-validated product opportunities ready to start.
- Developers should be able to build a working feature within one release. If a feature is too large to build within one release, work with your PM and Engineering team to determine the best way to split the feature into smaller segments.

For iteration inspiration watch our Product Designers discuss [iteration at GitLab](https://youtu.be/0lhjzU-QZ2w).

### Present an MVC solution

- After you've validated your solution with users, propose just one solution. Proposing multiple alternative solutions for others to pick undermines your position as a UX expert and leads to design by committee. If you have a good reason to propose multiple alternative solutions, make sure to explain why.
- When sharing asynchronously in an issue, make sure your audience has the context necessary to understand your proposal and how they can help. Is it clear who will use the solution and what it will enable them to accomplish? Do you need feedback or assistance from stakeholders? If so, on what specifically? Or, are you looking for approval? To make reviewing easier, have you highlighted things that changed since the last review?
    - Consider using the [collapsed content sections](https://about.gitlab.com/handbook/markdown-guide/#collapse) to include information that would support points being made without distracting the reader from the main point. This is demonstrated in [this issue comment around using analytics about file sizes](https://about.gitlab.com/handbook/markdown-guide/#collapse).
- `@mention` your Product Design Manager on the issue for feedback. Product Design Managers have a broader view of work that's happening across the product, enabling them to provide feedback that is helpful for maintaining strategic alignment, a consistent level of quality, and functional consistency.
- Frame design discussions around the customer and the problem being solved, not the UI or functionality itself. When presenting, start with the current state and how it fails to meet user needs, and then walk through the proposed solution from the user’s point of view. As the discussion unfolds, continually tie everything back to the user’s experience and needs.
- Anticipate questions that others might have, and try to answer them in your proposal comments. You don’t have to explain everything, but try to communicate a bit of your rationale every time you propose something. This is particularly important when proposing changes or challenging the status quo, because it reduces the feedback loop and time spent on unnecessary discussions. It also builds the UX Department’s credibility, because we deal with a lot of seemingly subjective issues.
    - Consider using the [questions as headings](https://gitlab.com/gitlab-org/gitlab/-/issues/118442#note_276666054) in framing your proposal
- Keep the SSOT updated with what’s already agreed upon so that everyone can know where to look. This includes images or links to your design work.
- If you’re working with design files, follow the instructions in the [GitLab Design project contribution guidelines][gitlab-design-project-contribution-guidelines] and regularly commit them.
- If you are proposing a solution that will introduce a new UX paradigm, or change an existing one, please consider the following:
    1. Will this pattern be inconsistent with other areas of the application?
    1. Will other areas of the application need to be updated to match?
    1. Does this new pattern significantly improve the user experience?
    1. If you decide that it is worth changing/updating the pattern, follow the steps outlined in our [component lifecycle documentation](https://design.gitlab.com/get-started/lifecycle).

### Deliver

- Once your work is complete and all feedback is addressed, make sure that the issue description, the SSOT, is updated with a section called "Solution". This is where you should direct people when they have questions about what should be done and how.
- When sharing design work, utilize both Figma's collaboration tools and [GitLab's design management features](https://about.gitlab.com/direction/plan/design_management/). In the following table, you’ll find a few common scenarios along with the recommended tool. Use this as a starting point, and when in doubt, make the best decision that moves the design forward.

| **Scenario** | **Figma** | **Design Management** |
| -------- | ----- | ----------------- |
| Co-designing within a shared file | √ |  |
| Providing, or seeking feedback while a design is still in progress, and not ready for MVC | √ |  |
| Seeking feedback on a design with a larger audience |  | √ |
| When feedback directly impacts an issue |  | √ |
| Presenting design options or variations so the team can choose a direction |  | √ |
| Sharing a prototype | √ |  |
| Adding a to-do for a designer as it relates to in-progress design | √ |  |
| Adding a to-do for a designer as it relates to an issue |  | √ |
| Identifying visual regressions |  | √ |
| Detailed redlines or specs | √ |  |

- If the solution needs to be broken out into smaller issues for implementation, apply the `workflow::planning breakdown` label and stay involved by walking PM and Engineering through the proposed solution and participating in the conversation to break down the issue.
- If the solution needs to be scheduled by PM and/or EM, apply the `workflow::scheduling` label and mention the [responsible product manager](/handbook/product/categories/#devops-stages) to [schedule it](/handbook/engineering/workflow/#scheduling-issues). It is also the Product Designer's responsibility to communicate with the assigned engineer to ensure they understand the solution.
- If the issue is meant for implementation in the current milestone, review the solution with the assigned engineer(s) and/or engineering manager. If they are comfortable with the solution, you can apply the `workflow::ready for development` label.
- There are times that a Product Manager might request that an issue is moved to the Build phase before the Product Designer feels that the experience meets UX Department standards. In that case, the Product Designer should create follow-on issues and/or apply the `UX debt` label to indicate that the product doesn't meet UX requirements and will require immediate iteration.

### Follow through

- Encourage Engineers to scope down features into multiple merge requests for an easier, more efficient review process.
- When breaking down features into multiple merge requests, consider how the UX of the application will be affected. If merging only a portion of the total changes will negatively impact the overall experience, consider using a feature branch or feature flag to ensure that the full UX scope ships together.
- When breaking solutions into smaller parts, make sure to share the end design goal, so that the entire team has context. Giving everyone the full picture helps developers write code aimed at achieving that goal in the future.
- Keep the issue description updated with the agreed-on scope, even if doesn’t impact your work. This is everyone’s responsibility. The issue description must be the Single Source Of Truth (SSOT), not the discussion or individual comments.
- Not all issues are scheduled immediately, which means changes are likely needed when the issue is prioritized. The Product Designer responsible for a particular stage group should be aware of open issues within their product area and work to prioritize them accordingly with their respective Product Managers, even if they are not the original designer who worked on the issue.
    - To stay up to date with issues in your product area, subscribe to the label that matches your stage group.
    - Review issues within your stage group label regularly.
    - Actively contribute to planning meetings to ensure all open issues are being discussed and prioritized.
- When working on an issue, keep the SSOT in the description updated until the issue is closed. This applies to both text and mockups. Previous content (by a PM, for example) should be removed or archived into a separate section in the description. If the developer working on the issue ever has any questions on what they should implement, they can ask the designer to update the issue description with the design.
- For obvious changes, make the SSOT description update directly. [You don't need to wait for consensus](/handbook/values/#collaboration). Use your judgement.
- When the issue is actively being worked on, make sure you are assigned and subscribed to the issue. Continue to follow both the issue and related merge request(s), addressing any additional UX issues that come up.

### MR reviews

Almost all merge requests (MRs) change the UX in one way or another, but we only require UX reviews for MRs that include **user-facing changes**. Per the [approval guidelines](https://docs.gitlab.com/ee/development/code_review.html#approval-guidelines)), “user-facing changes include both visual changes (regardless of how minor), and changes to the rendered DOM which impact how a screen reader may announce the content.”

- Follow the [Code Review guidelines](https://docs.gitlab.com/ee/development/code_review.html). Exceptions to those guidelines are noted below.
- UX review requests in MRs are high priority. Respond to them in accordance with our [first-response Service-Level Objective](/handbook/engineering/workflow/code-review/#first-response-slo), not only when the request comes from within your stage group, but also when it's a community contribution or another stage group asks for your quick input.
- Test locally, and do not rely on screenshots.
- Be thorough. There should be as little back and forth as possible.
- If you are asked to review an MR for an issue you were not assigned to, remind the author who the assigned designer is and assign to original designer for review.
- When reviewing an MR, please use the following order of importance:
    - Functionality first: Does it work? Are there [accessiblity](https://design.gitlab.com/accessibility/best-practices) issues?
    - Edge cases: Are there any unexpected edge cases?
    - Visual consistency: Does it conform to our Design System and workflows in other product areas?
- Remember to stick to the issue. Create issues for further updates to avoid scope creep.
- Once you have completed the review process, use the **Approve** button to indicate you have completed your review. You can unassign yourself from the MR.

Product Designers should feel empowered to adapt the process to fit their situation, as long as they feel confident that UI changes are getting sufficient attention to avoid inflicting UX bugs or UX pain for customers. Some common scenarios include:

- Finding a UX problem but the team decides to merge the code anyway. When this happens, create a new issue to fix the problem and label it with `UX Debt` per this section on [UX labels](/handbook/engineering/ux/ux-department-workflow/#how-we-use-labels).
- Doing visual reviews on staging instead of (or in addition to) locally. Examples are larger changes that span more than one MR or workflows that don't test well locally. In this case, product designers can work with the frontend team to figure out the right timing for the review. In certain cases, it can be fine to merge MRs prior to a full visual review, as long as the functionality remains behind a feature flag and a plan is in place for the visual review to occur in staging. Keep in mind that this can result in more new issues and MRs, if the product designer finds things that need to be fixed.

### Follow-up after design is complete

For changes that affect Pajamas, such as introducing a new UI component, refining an existing component, or adding significant clarity to the usage of a component, you should take the following additional steps:

- For changes that affect the user interface: [Create a **UX Pattern** issue](https://gitlab.com/gitlab-org/gitlab-design/issues/new?issuable_template=UX%20Pattern) in GitLab Design and follow its checklist to record the new standard.
- For other changes: Create an issue and/or MR in the [Design System](https://gitlab.com/gitlab-org/gitlab-services/design.gitlab.com) to update the documentation.
- As applicable, create issue(s) to update areas of the application that are affected by this pattern.
- Add an agenda item to the next UX weekly call to inform everyone of those changes.
- If the change/addition is a significant one, consider adding it to the Company Call to inform the company of the changes.

## Approach to communication

As design can be subjective, discussion can heat up. Sometimes team members won't agree on the best approach. Always try to be [direct](/handbook/values/#directness) but [kind](/handbook/values/#kindness). Try to give your best reasoning for your choices, and evaluate everyone's ideas and suggestions. Come up with a solution instead of discussing endlessly. If you think additional perspective is needed, mention a fellow Product Designer in the issue, or take it a step further and suggest that we perform some [solution validation](/handbook/engineering/ux/ux-research/#solution-validation) to let the data guide our design direction. Finally, remember that at GitLab we can [disagree, commit, and disagree](/handbook/values/#disagree-commit-and-disagree).

## Design tools

### Figma

Our primary design tool is [Figma](https://www.figma.com/). As a product designer or product design manager in the UX department, you will have a Professional Figma license and access to the GitLab team in Figma. You don’t need to do anything on your end, other than accept the invite sent to your GitLab email account during onboarding.

Anyone else in GitLab can access your files when you either share the file URL or invite them directly via email, but we ask that you only give them “can view” permissions. Anyone with “can edit” permissions is considered a paid seat and must have approval. A user with “can view“ permission will still be able to comment on and inspect design files.

GitLab has a public Figma profile where anyone can duplicate or remix files we have published. You can view our profile under the Community tab of the GitLab team section, or navigate to https://www.figma.com/@GitLab.

Do not create additional teams. An editor is billed for each team they are on, and we’ve only allocated resources for one team.

#### Access and permissions

Figma has four levels of access, also called Permissions, for Professional teams. Permissions can be set at a team, project, and file level.

1. **Editors** - Only GitLab product designers and product design managers in the UX department are editors. Editors have “can edit” access to projects and files, unless otherwise changed.
1. **Viewers** - Viewers on the GitLab team have “can view” access to any project or file, unless otherwise changed.
1. **Admins** - An admin has access to Team Settings, and the Admin Dashboard, including billing.
1. **Owners** - Anyone who creates a team, project, or file will be the default owner of it.

[View complete permission details](https://help.figma.com/hc/en-us/articles/360039970673-Viewer-Editor-and-Admin-team-permissions)

[ux-guide]: https://docs.gitlab.com/ee/development/ux_guide/
[gitlab-design-project-contribution-guidelines]: https://gitlab.com/gitlab-org/gitlab-design/blob/master/CONTRIBUTING.md
[twitter-sheet]: https://docs.google.com/spreadsheets/d/1GDAUNujD1-eRYxAj4FIYbCyy8ltCwwIWqVTd9-gf4wA/edit
[product-dev-flow]: /handbook/product-development-flow/
