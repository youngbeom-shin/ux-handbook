---
layout: handbook-page-toc
title: "Release Management UX"
description: "The Release Management UX team focuses on creating delightful experiences for all functionality related to Continuous Delivery and Release Automation."
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Overview

The [Release Management group](/handbook/product/categories/#release-management-group) is focused on all the functionality with respect to Continuous Delivery and Release Automation.

- [Release Orchestration Product Direction](/direction/release/release_orchestration/) (viable)
- [Release Evidence Product Direction](/direction/release/release_evidence/) (minimal)
- [Secrets Management Product Direction](/direction/release/secrets_management/) (minimal)
- [Pages Product Direction](/direction/release/pages/) (complete)

### Learn more

- For of our UX Vision and Strategy, take a look at the [Release UX Strategy](/handbook/engineering/ux/stage-group-ux-strategy/release/).
- For the product vision and mission, take a look at the [Release:Release Management Group](/handbook/engineering/development/ops/release/release-management/) page.
- For an understanding of what the Ops stage ecapsulates, take a look at the [product vision](/direction/ops/#release).

You can also reach out to the Release Management Slack channel `#g_release-management`.

## UX Vision Map - What's next

We are working on adding depth and enriching the Release Management features to support our vision of allowing users to plan and orchestrate releases from wherever they want API, YAML, and UI. Our next big items are:

- 3-year vision mockups ([gitlab&3825](https://gitlab.com/groups/gitlab-org/-/epics/3825))
- GitLab Runbooks ([gitlab&4218](https://gitlab.com/groups/gitlab-org/-/epics/4218))
- Advanced Deploy Freeze ([gitlab&2884](https://gitlab.com/groups/gitlab-org/-/epics/2884))
- Measure DORA 4 Metrics in GitLab ([gitlab&4358](https://gitlab.com/groups/gitlab-org/-/epics/4358))
- Releases <> Group Milestones ([gitlab&4362](https://gitlab.com/groups/gitlab-org/-/epics/4362))
    - Associate group milestones to releases ([gitlab#121476](https://gitlab.com/gitlab-org/gitlab/-/issues/121476))
- Share production environments across projects ([gitlab&4276](https://gitlab.com/groups/gitlab-org/-/epics/4276))
- Fetch & Configure Secrets ([gitlab&2875](https://gitlab.com/groups/gitlab-org/-/epics/2875))
    - Define Vault credentials in UI ([gitlab#218677](https://gitlab.com/gitlab-org/gitlab/-/issues/218677))
- Split secrets from CI/CD Variables ([gitlab#217355](https://gitlab.com/gitlab-org/gitlab/-/issues/217355))

We are also continuously investigating how to improve the overall user experience of GitLab Releases through the following initiatives:

- Usability of Releases ([gitlab&2355](https://gitlab.com/groups/gitlab-org/-/epics/2355))
- Improving Environments ([gitlab&3293](https://gitlab.com/groups/gitlab-org/-/epics/3293))
- Release Management UX Debt & UI Polish ([gitlab&3416](https://gitlab.com/groups/gitlab-org/-/epics/3416))

## Our customer

The product vision for Release Management has become more focused on providing advanced administration capabilities for release coordination and deployment tracking in GitLab. This is to build on the data asset we have at GitLab that starts from users purchasing GitLab to build product fast in a continuously integrated way. We will expand this journey by helping them coordinate and deploy at scale.

Today, mono-repository projects deploying with Kubernetes are most able to take advantage of our offering. We are targeting customers needing to coordinate across many teams and groups to successfully deploy. Regulated industries are top benefactors of our offering.

### Competitive analysis

See all [Release Management competitive analysis](https://gitlab.com/groups/gitlab-org/-/epics/2622).

## Our Jobs To Be Done (JTBD)

See all [Release Stage Jobs To Be Done](/handbook/engineering/development/ops/release/jtbd/).

## How we work

- We use the [**UX Planning epic**](https://gitlab.com/groups/gitlab-org/-/epics/2439) to collect issues that need UX review. Because these issues are in the `workflow:design`, they don't need to have a milestone assigned and are mostly assigned to `Backlog`. UX and PM will discuss the scope and priority of these in our 1:1s, ThinkBig! sessions, and other sync and async methods. Once a design proposal is added to the issue description (SSOT), we remove it from the epic and move it to the next step as per the [engineering workflow stages](/handbook/engineering/development/ops/release/release-management/#workflow-stages).
- We work in a continuous Kanban manner while still aligning with Milestones. See the [Release Management planning workflow](/handbook/engineering/development/ops/release/release-management/planning.html).
- We **label** our issues with `UX`, `devops::release` and `group::release-management`.
- PM will assign UX-ready issues to a particular milestone as per engineering capacity and delivery priority.
- PM will scope and label issues `workflow:ready for design` before moving them to `workflow:design`.
- We support engineering issues that are being worked on a particular milestone by reviewing MRs labeled `UX`, creating follow-up issues, and updating the SSOT as the scope of delivery changes.
  - See [all Release P1s labeled UX](https://gitlab.com/groups/gitlab-org/-/boards/1488065?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=cicd%3A%3Aactive&label_name[]=group%3A%3Arelease%20management&label_name[]=Release%3A%3AP1&label_name[]=UX).

### UX Definition of Done (DoD)

> This is a pilot process we kicked off in 12.10 -- [release-management#21](https://gitlab.com/gitlab-org/ci-cd/release-management-group/release-management/-/issues/21). Iterated on [release-management#40](https://gitlab.com/gitlab-org/ci-cd/release-management-group/release-management/-/issues/40#note_430976408).

Together with the product manager, the product designer applies the DoD to epics in order to better break down design work and give counterparts better insight into which steps in the design workflow need to be completed before the MVC can move to the development phase.

```
### UX Definition of Done

- [ ] Problem has been validated
- [ ] Problem is ready to enter ~"workflow::ready for design" 
- [ ] User stories and acceptance criteria for MVC have been created
  - Reminder: consider edge cases for each user story
- [ ] Cross-team dependencies have been identified, if applicable
- [ ] Prototypes or mock for each user story have been created
- [ ] Solution has been validated
- [ ] Pajamas
    - [ ] UI Component design have been identified
    - [ ] Pajamas issue is created (new workflow)
- [ ] If changes involve copy, ~"Technical Writing" and ~"UI text" labels have been added
- [ ] SSOT of MVC has been updated and labeled ~"workflow::ready for development"

```

[See how other designers in CI/CD use the UX DoD](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/ci-cd/#definition-of-done-for-ux-pilot)

### UX and engineering collaboration

We collaborate closely with the engineering team to ideate, refine, review, and iterate on the design of Release Management features. The Product Designer's responsibilities include:

- Provide [guidance and facilitate design discussions](/handbook/engineering/ux/ux-designer/#product-design-process) before issues are ready for development.
- Review MRs locally using by following the [code review guidelines](https://docs.gitlab.com/ee/development/code_review.html) and [ux review guidelines](/handbook/engineering/ux/pajamas-design-system/design-review/). If reviewing an MR locally is not possible, communicate early and often with the engineer to provide a concise description, screenshots/videos for the MR.
- Unblock the engineering team by ensuring changes that impact the user experience but are not validated by the Product Designer in the development phase are tracked as `UX debt`.

Watch on Unfiltered: [Frontend/UX MR Review Process. What can we improve going forward?](https://www.youtube.com/watch?v=aqRolFLULzE)

## Performance indicators

### UX Debt

**Chart** ([Sisense↗](https://app.periscopedata.com/app/gitlab/641753/UX-Debt?widget=8474988&udv=0))

<embed width="100%" height="350" src="<%= signed_periscope_url(dashboard: 641753, chart: 8474996, embed: 'v2') %>">

**Chart** ([Sisense↗](https://app.periscopedata.com/app/gitlab/641753/UX-Debt?widget=8474991&udv=0))

<embed width="100%" height="350" src="<%= signed_periscope_url(dashboard: 641753, chart: 8474998, embed: 'v2') %>">

- [Learn more about UX Debt](/handbook/engineering/ux/performance-indicators/#ux-debt) in the UX Department Performance Indicators page.
- [Release Managament UX Debt issues](https://gitlab.com/gitlab-org/gitlab/-/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=UX%20debt&label_name[]=group%3A%3Arelease%20management)

## Follow our work

Our [Release (CD) UX YouTube channel](https://www.youtube.com/playlist?list=PL05JrBw4t0KoyqCjN4f79w0dYZusHLx15) includes UX Scorecard walkthroughs, UX reviews, group feedback sessions, team meetings, and more.
