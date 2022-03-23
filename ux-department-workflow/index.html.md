---
layout: handbook-page-toc
title: "UX Department Workflow"
description: "Our UX department includes designers, researchers, and technical writers from all around the world. Everyone brings their own unique cultures, experiences, and strengths"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Meet The UX Department

Our UX department is made up of designers, researchers, and technical writers from all around the world. Each of them brings their own unique cultures, experiences, and strengths to GitLab. You can learn about each member of UX by visiting our [team page](/company/team/?department=ux-department).

## UX Weekly Call

The UX Department gets together once a week to share and discuss a variety of topics including workflow shortcuts or processes, designs for feedback, UX articles, and conferences. Attendance is optional but participation is encouraged. Each call is recorded and added to the archive.

## Product development timeline

The product development timeline that the UX department follows is described in the [engineering workflow](/handbook/engineering/workflow/#product-development-timeline) section of the handbook.

## Working with PMs

Every Product Designer is aligned with a PM. The UXer is responsible for the same features their PM oversees. The Product Designer meets with their PMs and other engineers every month to discuss scheduling and prioritization. Once the milestone has been set, the UXer assigns themselves to the issues in their area that need UX. UXers should immediately engage in and facilitate a conversation with the PM and engineers involved with the issue. Communicate early and often.

Understanding which PM is responsible for which area of the product is essential. An excellent resource for this is the [Product stages, groups, and categories](/handbook/product/categories/#devops-stages) section of the handbook. The [Product section](/handbook/product/) of the handbook will give you a deep dive into how Product at GitLab thinks and works.

## Milestone Planning

Product Designers meet with their PMs and other Engineering managers to discuss the priorities for the upcoming milestone. The purpose of this is to ensure that all understand the requirements and to assess whether or not there is the capacity to complete all the issues proposed. While we follow the [product development timeline](/handbook/engineering/workflow/#product-development-timeline), it is recommended that you work with your PM and Engineering counterparts to discuss upcoming issues in your stages' roadmap prior to them being marked as a deliverable for a particular milestone. There will be occasions where priorities shift, and changes must be made to milestone deliverables. We should remain flexible and understanding of these situations while doing our best to make sure these exceptions do not become the rule.

## Milestone Kickoff

Before working on the next release, we have a company kickoff call to explain what we expect to ship in the next release. This call is led by the product team and highlights significant improvements and features.

The UX Department is currently investigating a way to perform a UX Team kickoff asynchronously. Kickoff has been postponed until we find a viable solution.

## Community Contributions

We want to make it as easy as possible for GitLab users to become GitLab contributors. The UX team should offer support, guidance, and resources to any community member interested in contributing code and/or UX improvements.

Issues for which we accept contributions from community contributors are labeled as [`Accepting merge requests`][accepting-mrs].
We want to encourage our community to contribute at any stage of an issue we are interested in.
If an `Accepting merge requests` issue has an additional [`UX ready`][accepting-mrs-ux-ready] label, this issue points to changes that:

* We already agreed on,
* Are well-defined from UX perspective,
* Are likely to get accepted by a maintainer.

As a member of the UX Department, make sure to alert the UX Manager if you are asked to work on one of the issues but don’t have the capacity. The UX manager is responsible for encouraging the community member to suggest a solution, share a design proposal, and keep the conversation going.

For full details on contributing in general, see the [contributing doc](https://docs.gitlab.com/ee/development/contributing/issue_workflow.html#label-for-community-contributors).

[accepting-mrs]: https://gitlab.com/groups/gitlab-org/-/issues?state=opened&label_name[]=Accepting+merge+requests&assignee_id=0&sort=weight
[accepting-mrs-ux-ready]: https://gitlab.com/groups/gitlab-org/-/issues?state=opened&label_name[]=Accepting+merge+requests&label_name[]=UX+ready&assignee_id=0&sort=weight

## Product Designer Workflow

Once assigned to an issue, there is general workflow Product Designers follow.

Read about [__Product Designer workflows__](/handbook/engineering/ux/ux-designer/)

## UX Research Workflow

There is a general workflow UX Researchers follow.

Read about [__UX Researcher workflows__](/handbook/engineering/ux/ux-research/)

## How we use labels

GitLab uses labels to categorize, prioritize, and track work. The following is a breakdown of the labels most directly related to the UX workflow. An overview of all the label types and uses can be found in the [contributing doc](https://gitlab.com/gitlab-org/gitlab-foss/blob/master/doc/development/contributing/issue_workflow.md).

* [**UX** label](https://gitlab.com/groups/gitlab-org/-/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=UX): Indicates that UX work is required on this issue. These issues can be new features, ideas for improvement or anything else where UX should contribute their expertise.
- [**Inclusion** label](https://gitlab.com/groups/gitlab-org/-/labels?utf8=✓&subscribed=&search=Inclusion): A change to GitLab that promotes inclusion as it relates to our [diversity](https://about.gitlab.com/handbook/values/#diversity) value.
- [**Inclusive design** label](https://gitlab.com/groups/gitlab-org/-/labels?utf8=✓&subscribed=&search=Inclusive+design): Considering, exploring, and evaluating the different ways someone would access, interact with, or contribute to content that results in a more accessible experience.
- **Accessibility and scoped accessibility labels** are used to identify issues with accessibility impact. The scoped labels should be added after an accessibility audit has validated the impact and used in combination with [priority](https://about.gitlab.com/handbook/engineering/quality/issue-triage/#priority) and [severity](https://about.gitlab.com/handbook/engineering/quality/issue-triage/#severity) labels to [triage](https://about.gitlab.com/handbook/engineering/quality/issue-triage/) an issue.
  - [**Accessibility** label](https://gitlab.com/groups/gitlab-org/-/labels?utf8=✓&subscribed=&search=%22Accessibility%22): Issues that directly relate to creating an accessible experience. This can be positive, negative, or just an observation.
  - `accessibility::critical`: Prevents some or all users from performing critical tasks with no possible workaround.
  - `accessibility::high`: Prevents some users from performing critical tasks. A workaround may exist, but not without creating frustration and inefficiency.
  - `accessibility::medium`: Prevents some users from performing non-critical tasks, or where the user experience is seriously degraded for users with certain assistive technologies.
  - `accessibility::low`: The user experience is degraded for users with certain disabilities or using certain assistive technologies, but users can still accomplish tasks.
* **Scoped workflow labels** from the [Product Development Flow](/handbook/product-development-flow/#validation-phase-1-validation-backlog) should be used to indicate where an issue is in the development lifecycle. Issues can move between workflow labels as many times as necessary, and not all labels will be applicable to every issue. Issues that require UX would use one of these labels to indicate that the issue is:
    * waiting to be worked on in the current or future milestone (`workflow::validation backlog`)
    * being validated to ensure the problem being solved is well understood and a real problem (`workflow::problem validation`)
    * in a solution design phase, including learning how others have solved the problem, creating sketches, flows, wireframes, mockups and/or prototypes (`workflow::design`)
    * being validated to ensure the selected solution solves the problem and is easy to use (`workflow::solution validation`)
* **Pajamas component lifecycle labels** are scoped labels used for creating and updating [Pajamas](https://design.gitlab.com) components. Label usage guidelines can be found in the [Pajamas component lifecycle documentation](https://design.gitlab.com/get-started/lifecycle/).
* [**UX problem validation** label](https://gitlab.com/groups/gitlab-org/-/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=UX%20problem%20validation): Indicates that the issue requires UX work to validate that the problem is relevant to users. We use this label in addition to the Product Development Flow scoped labels, so that we can track validation efforts over time in our [UX Performance Indicators](/handbook/engineering/ux/performance-indicators/).
* [**UX solution validation** label](https://gitlab.com/groups/gitlab-org/-/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=UX%20solution%20validation): Indicates that the issue requires tasks to validate that the proposed solution is technically feasible and meets user needs. We use this label in addition to the Product Development Flow scoped labels, so that we can track validation efforts over time in our [UX Performance Indicators](/handbook/engineering/ux/performance-indicators/).
* [**UI polish** label](https://gitlab.com/groups/gitlab-org/-/issues?scope=all&state=opened&utf8=%E2%9C%93&label_name%5B%5D=UI+polish): Indicates the issue covers _only_ visual improvement(s) to the existing user interface.
* [**UX debt** label](https://gitlab.com/groups/gitlab-org/-/issues?scope=all&state=opened&utf8=%E2%9C%93&label_name%5B%5D=UX+debt): UX debt results from the intentional decision to deviate from the UX vision or MVC, which sacrifices the user experience. UX debt labeled issues are to be included in subsequent releases. Use this label to indicate that the UX released does not meet: 
   * UX and Pajamas specifications
   * Usability standards
   * Feature viability standards

   This label is applied to any follow-up issues that address a UX gap. It does not apply to the issue or merge request that created the UX debt. For example, if the agreed MVC design solution is not fully realized due to release pressures or implementation oversight, that's considered UX Debt. 
   
   If the design is implemented correctly but unforeseen UX issues are identified, it is *not* considered UX debt. 

   If in doubt about when to apply this label, use the following rule: If you can say "This UX problem did not originate from an issue or merge request.", then it's just UX, not UX Debt. In case your team makes the decision ship an MVC that contains UX Debt, it is recommended to create an issue to track it as soon as the change has been released.
   
   [**Learn more about UX Debt as a UX Department Performance Indicator**](/handbook/engineering/ux/performance-indicators/#ux-debt)
   
* [**System Usability Scale (SUS)** labels](https://gitlab.com/gitlab-org/gitlab/-/labels?subscribed=&search=sus): Indicates that the issue is related to usability problems surfaced in one of our SUS research efforts. More specifically, issues related to SUS that are prioritized can be labeled with the corresponding Fiscal Year and Quarter. For example: `SUS::FY22 Q2 - Incomplete`  

  [**Learn more about SUS score as a UX Department Performance Indicator**](/handbook/engineering/ux/performance-indicators/#perception-of-system-usability)

* [**Regression** label](https://gitlab.com/groups/gitlab-org/-/issues?scope=all&state=opened&utf8=%E2%9C%93&label_name%5B%5D=regression): Indicates a bug introduced in the latest release that broke correct behavior (see the [contribution guidelines](https://gitlab.com/gitlab-org/gitlab-ce/blob/master/CONTRIBUTING.md#regression-issues) for more info).
* [**UX scorecard** label](https://gitlab.com/groups/gitlab-org/-/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=UX%20scorecard): Indicates the primary issue or epic for the [UX Scorecard](/handbook/engineering/ux/ux-scorecards/). We use this label to help us easily find current work and track efforts over time.
* [**UX scorecard-rec** label](https://gitlab.com/groups/gitlab-org/-/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=UX%20scorecard-rec): Indicates this issue is a recommendation that was a result of a UX scorecard review. It's OK if the issue was created prior to the scorecard being done; it can still be pulled into the set of recommendations.

While labels are extremely useful for organizing and tracking our work, they are not meant to replace the expertise and judgement of team members, or to replace collaborative touchpoints between PM, UX, and Engineering. Do not rely on labels to communicate important information about an issue (for example, to hand off an issue to a developer). Designers, partnering with PMs and EMs, should determine the best approach for any given problem, and label issues accordingly.   

## Milestone Retro

After each release, we have a company retrospective call in which we discuss what went well, what went wrong, and what we can improve for the next release.

To understand the specific challenges faced by the UX Department, we hold an async UX retrospective after every milestone. This retro is carried out through a new Issue created for the recent release in the [ux-retrospectives](https://gitlab.com/gl-retrospectives/ux-retrospectives/issues) project. The goal is to evaluate what went well, what didn’t go well, and how we can improve.

## Epics and issues

We use epics and issues to organize, discuss, and execute our day-to-day work. Epics are used to define a larger vision and goal for a feature or area of the product. Issues within the epic drive the actions taken to achieve the desired results. In most cases, PM and the UX Manager are utilizing epics to plan and execute efforts over several milestones.

## UX Showcase

<%= data.ux_showcase.about %>

[ux-guide]: https://docs.gitlab.com/ee/development/ux_guide/
[ux-label]: https://gitlab.com/groups/gitlab-org/issues?scope=all&state=opened&utf8=%E2%9C%93&label_name%5B%5D=UX
[ux-ready-label]: https://gitlab.com/groups/gitlab-org/issues?scope=all&state=opened&utf8=%E2%9C%93&label_name%5B%5D=UX+ready
[gitlab-design-project-readme]: https://gitlab.com/gitlab-org/gitlab-design/blob/master/README.md
[twitter-sheet]: https://docs.google.com/spreadsheets/d/1GDAUNujD1-eRYxAj4FIYbCyy8ltCwwIWqVTd9-gf4wA/edit

## User Experience professional development

The field of User Experience is always changing and evolving. We want Product Designers, UX Researchers, and Technical Writers to have opportunities to stay current on trends and further develop and refine their skills as part of a well-rounded [career development plan](/handbook/people-group/learning-and-development/career-development/). To that end, we support participation in relevant and valuable training and conferences, per GitLab's policies.

Your manager will work with the UX Director to communicate and approve requests for professional development.

To attend training or a conference, follow these procedures:
1.  Familiarize yourself with GitLab's policies on [professional development expenses](/handbook/spending-company-money/#work-related-online-courses-and-professional-development-certifications) and [budget applications](/handbook/engineering/development/enablement/processes/budget_approval.html).
1.  Talk to your manager about the event you are interested in. Estimate the attendance and travel costs before this conversation. Your manager can give guidance as to how likely your proposal is to be approved.
1.  Create a proposal (even for events under $500). This is the [template](https://docs.google.com/document/d/1AiwGVEXIXpl8jml8pkUlRYYquGnxeUyNNl_W09Rx1Lo/edit?usp=sharing).
1.  Name your proposal something that makes it easy to identify and save it to this [folder](https://drive.google.com/drive/folders/1VCNuwpJK0KjX2_ibtU2G_FFlF2mLB-7W).
1.  Send your manager a link to your proposal.
1.  If the cost exceeds $500, your manager will communicate with the UX Director and Finance department as needed, to obtain the approval you need.
    1. NOTE: If your conference exceeds the max budget, you will need to wait until the following year to be reimbursed for additional conferences. If it does not exceed the max budget, please follow this process again and work with your manager for approval.
1.  Don't book your ticket or travel until you have approval.

### Helpful information

* Consider using the [visiting grant](/handbook/incentives/#visiting-grant) to offset your travel budget.
  * NOTE: Visiting Grants can only be used for travel expenses
* Costs over $500 will need to be approved by your manager and finance. This is an annual limit, not a per event limit. There are no specific amounts or caps, but consider GitLab's policy regarding spending company money as if it were your own.
  * NOTE: It's possible that you can utilize the L&D budget to address additional expenses that weren't covered by the above reimbursements. This should be done on a case-by-case basis at the discretion of your manager and director.
