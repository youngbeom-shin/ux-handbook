---
layout: handbook-page-toc
title: "Kano Model and Feature Prioritization Survey"
description: "Kano model provides a simple and powerful way how to think about the features that we plan to build."
---


## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Kano model

The Kano model is a theory that ties product development with user satisfaction.
It was developed in Japan in the 1980s by Professor Noriaki Kano.
<!-- TODO: Mention that Kano model theory originated in the same atmosphere as other theories that influenced DevOps movement -->
The Kano model classifies product features into five categories based on how developing them impacts user satisfaction:

- **Must-be**: Features that are crucial for the initial adoption but won't lead to high satisfaction, no matter how much you invest in them.
- **Performance**: (a.k.a. One-dimensional) Not having these is a problem and satisfaction grows with growing investment.
- **Attractive**: These are nice-to-have features, but if you implement them well, satisfaction will skyrocket.
- **Indifferent**: Investing in these features will not increase or decrease user satisfaction.
- **Reverse**: Not having these features is actually better than having them.

<!--TODO: Change the list to a diagram -->

Once you know which categories your features fall into, you can prioritize the most important ones for development.
In theory, features from the Must-be category should be prioritized first, followed by Performance and then Attractive.
In practice, there might be good reasons to follow a different order of the categories or to prioritize features individually based on their score for multiple categories.

<!-- TODO: Explain that it is a model – a simplification -->

**Resources:** For more information check [The Complete Guide to Kano Model](https://foldingburritos.com/kano-model/) by Daniel Zacarias or Wikipedia entry for [Kano model](https://en.wikipedia.org/wiki/Kano_model).
{: .note}

### Why use it?

Using the Kano model can help you to make more informed decisions when prioritizing features from your backlog and to better understand why these features do or don't resonate with your users.

### How to use it?

The Kano model is best formed from user data, especially when it is informing the prioritization of features.
To collect this data we recommend conducting a research study and use a standardized questionnaire ([more details bellow ⬇️](https://about.gitlab.com/handbook/engineering/ux/ux-research-training/kano-model/#standardized-questionnaire)) that was developed as a part of the Kano model theory.
Designing a survey for a Kano model study is rather simple from the research perspective, however it requires a lot of preparation by the product manager – especially describing the features and current state of the product area.
In the following paragraphs we will discuss details of organizing such a study.

## Features Prioritization Survey

<!-- TODO: Add a section about issues structure for such a project -->

Example project: [Survey for CI feature prioritization](https://gitlab.com/gitlab-org/ux-research/-/issues/1027)

Project summary: *The team was considering 12 new features to build that they thought would benefit our users.  Since building new features is costly and time consuming, the team wanted to understand how users felt about each of those features, along with a prioritization.  The goal was to end up with a clearer understanding of which 12 the team should build first.*

### Preparation

Well-formulated feature descriptions are crucial for the success of your study.
Participants must be able to accurately understand the features that you are asking about and the value of those features, so they can provide honest feedback.
It makes sense to begin creating the survey only after the features are documented.

#### Category description

We usually develop new features in the context of features that already exist.
For that reason, you should first walk the participant through the current experience(s) that contain the features being presented.

**Example of category description:**

> A continuous integration pipeline in GitLab is defined as a version-controlled file in the Git repository of a project. This file is called 'gitlab-ci.yml' and users configure CI pipelines by editing this file and pushing it to the repository. Pipelines consists of jobs and stages. Jobs define what the pipeline should do. Stages consist of one or multiple jobs and define the sequence in which jobs run. All jobs in a stage run in parallel, and if all of them succeed, the pipeline moves on to the next stage. Different types of conditions can be specified for pipelines like prerequisites, exceptions, and so on. You can edit the pipeline YAML file either by cloning the project locally or using an online text editor.

#### Feature descriptions

When creating feature descriptions, follow these guidelines:

1. Describe features, not MVCs
   - The findings should be relevant for a reasonably long time. In other words, you would likely not be able to develop it in 1 or 2 milestones.
1. Use simple and neutral language
   - No GitLab lingo like `sections`, `categories`
   - No sales pitching like `easy-to-use`, `better`, `more efficient`
1. Set the feature into the context of the system
   - Use consistent terminology, making sure your feature descriptions fit into the overall category description.
1. Aim for one paragraph of text for each of the descriptions
   - Less than 1 normal paragraph might be not enough. On the other hand, if the text is too long, participants will more likely skip it.
1. Include only new features
   - Including features that are already developed can set a benchmark; however, it is mostly not actionable and therefore useless in this context.
1. Enrich the descriptions with images or gifs

**Example of feature description:**

> A list of CI job code snippets that will display next to the online pipeline editor. You use these code snippets as the building blocks of your pipeline by copying the jobs YAML from this list and pasting it into your pipeline code. This will speed up creating new pipelines and reduce mistakes.

<details>
  <summary markdown="span">**More feature description examples**</summary>
  <figure class="video_container">
     <iframe src="https://docs.google.com/document/d/e/2PACX-1vQff1-XyGoZeWaAyHhANrPjIQ54WXX8Je06_DzIsUtMK6ZQ6IhzMrvM3PGdXJLzu_Q9Z0Jz_5W41FCm/pub?embedded=true"></iframe>
  </figure>
</details>

<!-- TODO: Create & add a feature descriptions doc template -->

<!-- TODO: Add a feature description structure recommendation – https://gitlab.com/gitlab-org/ux-research/-/blob/8abb8170124572620ff719760cf67fb8d8e7a79a/Survey%20about%20requirements%20for%20monitoring/Feature%20description%20guidelines.md#feature-description-structure -->

#### Tips & tricks

💡**Tip**: Preparing for the survey can take a lot of time and might be hard to track. Creating a separate issue (just like [this issue](https://gitlab.com/gitlab-org/ux-research/-/issues/1143)) to track this effort will lighten the main research issue and will make it clearer who is the DRI.
{: .alert .alert-gitlab-purple}

 💡 **Tip**: Preparing feature descriptions asynchronously can take a lot of time. If you feel like your team is not moving forward quickly enough, [pivot to synchronous communication](https://about.gitlab.com/company/culture/all-remote/asynchronous/#when-to-pivot-to-synchronous).
 {: .alert .alert-gitlab-purple}

### Survey

#### Standardized questionnaire

The standardized questionnaire for the Kano model consists of two questions that are asked for each of the features that you are interested in:

<table style="width:100%">
  <tr>
    <th>Functional question</th>
    <th>Dysfunctional question</th>
  </tr>
  <tr>
    <td>
      <p>How would you feel if you <b>had</b> this feature?</p>
      <ul>
        <li>I am delighted by it</li>
        <li>I expect it</li>
        <li>I am neutral</li>
        <li>I can tolerate it</li>
        <li>I am frustrated by it</li>
      </ul>
    </td>
    <td>
      <p>How would you feel if you <b>did not have</b> this feature?</p>
      <ul>
        <li>I am delighted by it</li>
        <li>I expect it</li>
        <li>I am neutral</li>
        <li>I can tolerate it</li>
        <li>I am frustrated by it</li>
      </ul>
    </td>
  </tr>
</table>

**Note**: In [!28](https://gitlab.com/gitlab-org/ux-research/-/merge_requests/28), we adjusted the answer options a bit, because during a pilot session the original ones turned out to be hard to understand. More details about this decision are in [this thread](https://gitlab.com/gitlab-org/ux-research/-/merge_requests/28#note_382934909).
{: .note}

The benefit of using the standardized questionnaire is that basically all of the research design is already done, and you can reuse it from previous studies.  Also, taking a consistent approach to this methodology reduces the risk of introducing errors to the process.

<details>
  <summary markdown="span">**Example of a research plan**</summary>
  <figure class="video_container">
     <iframe src="https://docs.google.com/document/d/e/2PACX-1vRi6Dq6sDBtkggW5oEnmkTsLGx6WRvKrs8EV4aXaAhIlEpOgykK2PJEEp8uj2UfEymbQgLJYBVavR1c/pub?embedded=true"></iframe>
  </figure>
</details>

<!-- TODO: Create & add a research plan template -->

#### Questionnaire structure

Use Qualtrics to create the questionnaire. Each feature with related questions should be presented on a separate block.

<!-- TODO: Add a diagram of survey structure -->

Example: [Survey](https://gitlab.eu.qualtrics.com/jfe/preview/SV_3VoczISwBuK8ab3?Q_CHL=preview&Q_SurveyVersionID=current) that we used in [#1027](https://gitlab.com/gitlab-org/ux-research/-/issues/1027)

<!-- TODO: Review and mention a survey block template -->

#### Data collection & Analysis

Using the provided questionnaire, you'll be able to collect the data, analyze it, and report out the findings using both quantitative and qualitative approaches.

##### The qualitative approach

This approach will provide you with a better understanding of the _why_ behind their prioritization.  Also, collecting and analyzing the qualitative data first could help you to spot problems in your feature descriptions that you can fix before sending them out to a lot of people.
We recommend conducting 5 to 10 moderated sessions and/or 20 to 30 unmoderated sessions where a participant's task is to go through the questionnaire and explain the reasoning behind their answers.

<!-- TODO: Add example UserTesting project -->
<!-- TODO: Add example Dovetail project -->
<!-- TODO: Add example of outcome -->
<!-- TODO: Ask Nels if you can embed video with him -->

##### The quantitative approach

We recommend collecting responses from 50 to 80 users in your target audience and analyze them using discrete analysis described in the article [The Complete Guide to Kano Model](https://foldingburritos.com/kano-model/) by Daniel Zacarias.
This approach will provide you with "the numbers" that can back up your prioritization decisions, but you'll still lack the understanding behind the prioritization.

<!-- TODO: Add example spreadsheet -->
<!-- TODO: Find out if you can publish a spreadsheet. If yes, anonymize it and embed to this page -->
For the analysis use this spreadsheet template: [Kano model: Survey for <category> feature prioritization](https://docs.google.com/spreadsheets/d/14D-ayhw15J9o7ixzFh7pda_SZQkhZTRsyJvHi_5JXbk/edit?usp=sharing)
<!-- TODO: Explain that this type of analysis is not statistically sound and that we have to come up with something better -->
<!-- TODO: Add example of outcome -->

Taking the quantitative and qualitative approach will result in a more complete story behind the data. In addition to prioritization, you'll also be able to explain _why_ participants scored the way they did, too.
Combine these two approaches to get the most of your Kano model study

#### Tips & tricks

💡 **Tip**: If the questionnaire isn't too long and you have some other questions you would like to ask, feel free to add one more block for these questions in the end.
{: .alert .alert-gitlab-purple}

## Resources
- Article [The Complete Guide to Kano Model](https://foldingburritos.com/kano-model/) by Daniel Zacarias
- Wikipedia entry for [Kano model](https://en.wikipedia.org/wiki/Kano_model)
- Article [Kano Model — Ways to use it and NOT use it](https://medium.com/design-ibm/kano-model-ways-to-use-it-and-not-use-it-1d205a9cf808) by Cary-Anne Olsen-Landis
- Video [Building a Winning UX Strategy Using the Kano Model](https://www.youtube.com/watch?v=Hr1rN3jibIk&feature=youtu.be) by Jared Spool

## Example research in GitLab
- [Monitoring feature prioritization](https://gitlab.com/gitlab-org/ux-research/-/merge_requests/28)
- [CI feature prioritization](https://gitlab.com/gitlab-org/ux-research/-/issues/1027)
- [Threat insights feature prioritization](https://gitlab.com/gitlab-org/ux-research/-/issues/1295)

<!-- TODO: Use GitLab terminology – category, group -->
