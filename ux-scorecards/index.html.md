---
layout: handbook-page-toc
title: "UX Scorecards"
description: "The UX Scorecard is a process similar to a heuristic evaluation that helps identify usability issues and score a given experience."
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Intro and goal

The UX Scorecard is a way for us to identify and score the usability of an experience in our product based on a set of heuristics. We use UX Scorecards to gain an understanding of how a user interacts with our product and to quickly spot opportunities for improvement. 

UX Scorecards should be done on every important workflow and should be repeated from time to time so that we can continuously monitor our progress in making experiences better for our users. 

As UX practitioners, we must think strategically about fixing usability challenges within the GitLab product in order to give our users a quality experience. Creating a UX Scorecard with associated recommendations enables us to identify, scope, and track the effort of addressing usability concerns within a specific workflow. When it's complete, we have the information required to collaborate with Product Managers on grouping fixes into meaningful iterations and prioritizing UX-related issues.

## About the process

The UX Scorecard process is meant to balance flexibility and consistency. There are several ways you can create your Scorecard, listed from lightest to heaviest. Select an appropriate approach based on the time you have, the priority of the workflow to users, or whether or not this is a first Scorecard or an update.

When doing a Scorecard, you have several options:
- Conduct a [heuristic](https://www.nngroup.com/articles/ten-usability-heuristics/) evaluation. This can be done in half a day, especially when you are working on a Scorecard for a task that has previously been scored.
- Do a "light" usability test and observe 3-5 internal or external users. This can be done in about a day.
- Run a more in-depth usability test using 5-7 external users. Plan ahead, as it can take a couple of weeks to recruit participants and run the study. This approach is ideal for evaluating the primary job of the stage group that has not been scored in the past.

In every case,
- define the [JTBD](/handbook/engineering/ux/jobs-to-be-done/) prior to conducting the Scorecard. 
- use our [heuristics](/handbook/engineering/ux/heuristics/) to calculate a score.
- observation of users is preferred over a purely heuristic evaluation as it will remove subjectivity. 

This is a process intended to help inform the design process and maintain a high bar of quality.

- All of the UX Scorecards can be found in this [epic](https://gitlab.com/groups/gitlab-org/-/epics/1714).

### How UX Scorecards relate to Category Maturity Scorecards

- **When to create a UX Scorecard:** 
     - To quickly identify and prioritize usability issues and opportunities for improvement within an experience. 
     - When joining a new product area to become familiar with the workflows and to evaluate the experience from a fresh perspective.
     - In conjunction with usability testing workflows.
     - In order to evaluate the onboarding experience of your workflows.
     
- **When to create a [Category Maturity Scorecard](/handbook/engineering/ux/category-maturity-scorecards):** 
     - When more rigorous testing is required within a category in relation to a set of business requirements and/or features that are needed for the category to move up. This is a summative process (not for identifying usability concerns) that allows us to gather metrics and data that will help us understand how changes to the product impact the user experience over time. We grade the maturity of our product using this process.

## Setup

Below is a recommended step by step process for completing a UX Scorecard. Note that every scorecard is not the same. Product Designers are welcome to adapt the steps to their needs as long as they are as objective as possible and the spirit and outcome remains the same.

1. Create an (or locate the existing) epic that will contain all UX Scorecards for that stage group.  
    > Example: “UX Scorecard - Create:Source Code”
1. If not already done, add the stage group epic to the [UX Scorecards -- All Evaluations](https://gitlab.com/groups/gitlab-org/-/epics/1714) epic.  
1. Work with your Product Manager to identify the top jobs (in frequency or importance) for users of your stage group. Ideally, you will base this task list on user research (analytics or qualitative findings).
1. Select one of the top jobs to complete a UX Scorecard.
1. [Create an experience scoring issue](https://gitlab.com/gitlab-org/gitlab-design/issues/new?issuable_template=UX%20Scorecard%20Part%201), using the template “WIP: UX Scorecard Part 1”, and add it to the stage group epic. 

    This issue should have the **UX Scorecard** label. If it's related to an OKR, also apply the **OKR** label for easier tracking.
1. [Create a recommendations issue](https://gitlab.com/gitlab-org/gitlab-design/issues/new?issuable_template=UX%20Scorecard%20Part%202), using the template “WIP: UX Scorecard Part 2”, to be done after the experience scoring.
1. Follow the instructions in the templates to complete the scorecard and use the [Grading Rubric](https://about.gitlab.com/handbook/engineering/ux/heuristics/#scoring).
1. Once you have completed the evaluation and provided your recommendations, remove the "WIP:" prefix from the issue title.

If you'd like to view or edit the templates, you can find them here: 

* [Part 1 - UX Scorecard  ](https://gitlab.com/gitlab-org/gitlab-design/blob/master/.gitlab/issue_templates/UX%20Scorecard%20Part%201.md) 
* [Part 2 - Recommendations](https://gitlab.com/gitlab-org/gitlab-design/blob/master/.gitlab/issue_templates/UX%20Scorecard%20Part%202.md)

## Evaluating the onboarding experience

The onboarding experience of your product category can make a big difference in the adoption of GitLab stages. You can use a UX Scorecard to assess the UX of your onboarding experience and identify areas for improvement.

Onboarding can refer to many different scenarios, and this can impact the experience:
* a SaaS or self-managed user
* a brand new GitLab admin setting up a SaaS or self-managed account/instance
* a brand new GitLab user joining a company or team
* a trial user
* an existing user of GitLab joining a company or team
* an existing user of GitLab trying a feature in a new stage or category
* A GitLab feature, a set of features, or a complete DevOps stage
For example, an existing user of GitLab joining a new team might require some help on unfamiliar features, or getting oriented to the groups and projects on the team. While a brand new user would require more help getting oriented with the application itself.

### Steps to Evaluate Onboarding UX

* Think about the most important tasks/scenarios related to your JTBD.
* Identify the scenarios in which a user would do this task for the first time.
* Conduct a UX scorecard or usability test on those tasks/scenarios, incorporating each scenario.
* Focus your evaluation on the onboarding [heuristics and rubric](https://about.gitlab.com/handbook/engineering/ux/heuristics/) to rate the onboarding experience.
* Document the onboarding score and date (location TBD).

If you have a recent UX scorecard or a recent usability test with recordings, you can update these rather than starting over. For example, if you recently did a usability test on creating MRs, you can re-watch the sessions with the onboarding heuristics in mind to infer an initial score for the onboarding experience. However, it is highly recommended that at some point you intentionally evaluate the onboarding experience.
