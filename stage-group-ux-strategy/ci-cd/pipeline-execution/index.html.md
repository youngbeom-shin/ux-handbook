---
layout: handbook-page-toc
title: "Pipeline Execution UX"
description: "A documentation of the practices, objectives, achievements and plans of the Pipeline Execution UX team."
---

## Overview

The [Verify:Pipeline Execution Group](/handbook/engineering/development/ops/verify/pipeline-execution/) is focused on all the functionality with respect to Pipeline Execution, as part of GitLab Continuous Integration.
A key focus for the Pipeline Execution group is delivering features that achieve the outcome we track in our performance indicator.

- **Pipeline processing**: processes responsible for transitions of pipelines, stages and jobs.
- **Rails-Runner communication**: jobs queuing, API endpoints and their underlying functionalities related to operations performed by and for Runners.
- **Job artifacts**: storage and management of artifacts is the gateway for many CI/CD features.

## Pipeline Execution UX Plan

### Vision

The Pipeline Execution UX team is working on substantially improving the experience of the overall core areas within CI, including triggering a pipeline and analyzing its performance. Here are a few epics to support our plan:

- [3 Year Vision - Verify:Pipeline Execution](https://gitlab.com/groups/gitlab-org/-/epics/4793)
- [1 Year Focus - Verify:Pipeline Execution](https://gitlab.com/groups/gitlab-org/-/epics/4794)
- [3 Years Focus](https://gitlab.com/groups/gitlab-org/-/epics/4898)
- [MR Widget Improvements for CI](https://gitlab.com/groups/gitlab-org/-/epics/4926)
- [Improve GitLab CI/CD documentation](https://gitlab.com/groups/gitlab-org/-/epics/4899)

### Ongoing Initiatives

Currently we are working towards refining the merge trains related experience and exploring around providing users with an ability to monitor the performance of their running pipelines.

- [Merge Trains support for fast-forward merge](https://gitlab.com/groups/gitlab-org/-/epics/4911)
- [Job ignores previous stage if cancelled and retried](https://gitlab.com/gitlab-org/gitlab/-/issues/207988)
- [Design - Present information around running pipeline activities in GitLab CI](https://gitlab.com/gitlab-org/gitlab/-/issues/280773)


## Our Customers

Coming soon.

## Our Process

In the CI UX team, the planning happens on the milestone planning issue in collaboration with the Product Manager and the engineering team. 

Since the designs are always provided a few milestones in advance to the implementation milestone, we track the progress of design issues by using the labels `pd::doing` and `pd::finished`. These labels indicate if an issue is being worked on by the product designer and the final design proposal has been added to the issue, respectively.

Read about the process of Verify:Pipeline Execution team in detail [here](/handbook/engineering/development/ops/verify/pipeline-execution/#how-we-work).

## CI UX DoD objectives
A Definition of Done (DoD) serves as a tool for describing and tracking the expected deliverables, objectives, and the approval process. The DoD consists of a list applied by the Product Designer and Product Manager to issues or epics, in order align and track the entry and exit criteria for design work. This list should be flexible, making this process [efficient for their ways of working](https://about.gitlab.com/handbook/values/#efficiency-for-the-right-group).

##### Entry Criteria for `workflow::design`

- Problem is well understood and has gone through the `workflow::problem validation`, if necessary.
- Issue has a clear and well articulated problem background (why it is prioritised) description
- User stories and acceptance criteria have been created
- Edge cases were considered and described by PM and Product Designer
- `UX` and `pd::doing` labels are added to the issue
- Cross-team dependencies have been identified and documented, if applicable. Product Designer and Product manager from the concerned stage groups are notified

##### Criteria for UX DoD (exit criteria for "workflow::design")

- Prototypes for each applicable user story have been created
  - Empty state
  - Responsiveness
  - Edge cases
- Design proposal was ran and is aligned with engineering team to avoid non-feasible solutions and ensure the iteration in our development process.
- Incremental design approach was applied to split the design problem into small problems and deliverables and an MVC solution is identified (UX to work with Engineering). New issues are created for the follow up user stories
- If changes involve copy, `UI text` label has been added
- Pajamas: component creation or update have been identified
  - Pajamas issue is created. If a new component is proposed, consider notifying the UX team to avoid duplicate efforts and encourage collaboration
- Marked as ready for engineering evaluation per user story moved into `workflow::planning breakdown`
- Replace `pd::doing` with `pd::finished`

##### Entry Criteria for `workflow::ready for development`

- Scope has successfully exited `workflow::planning breakdown` 
- User stories have been weighed and broken down into feasible iterations (smaller solutions)

##### UX Weighting (optional)

UX weighting is an optional process and should be applied accordingly to team needs.

We add the weight to UX issues using the [storypoints system](https://www.nngroup.com/articles/ux-user-stories/):

|  | S | M | L | XL | XXL (subject for breaking down) | XXXL (subject for breaking down) |
| ------ | ------ | 
| Points | 1 | 2 | 3 | 5 | 8 | 13 |

-----

## UX Debt and UI Polish Issues

The ~UX Debt and ~UI Polish issues for CI are tracked in this epic: https://gitlab.com/groups/gitlab-org/-/epics/4667. Our goal is to work on a minimum of one of these issues each milestone.




