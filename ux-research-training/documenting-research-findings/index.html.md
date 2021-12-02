---
layout: handbook-page-toc
title: "Documenting research findings"
description: "The UX Research team uses Dovetail to document all the user insights discovered through GitLab’s UX research program"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

### Documenting research findings
The UX Research team uses [Dovetail](/handbook/engineering/ux/dovetail/) to document all the user insights discovered through GitLab’s UX research program. User insights can be gathered through methods such as user interviews, usability testing, surveys, card sorts, tree tests, customer conversations, and more.

#### Why do we document research in Dovetail?
The UX Research team has [always faced challenges](https://about.gitlab.com/blog/2019/07/10/building-a-ux-research-insights-repository/) in finding the best way to create research reports that are easy to digest and access. When using methods such as PDFs, Google docs, and even GitLab CE issues themselves, it was difficult to track and share study findings. Additionally, since we are often asked to readily recall information we've learned in prior studies, it can be tedious to read through old reports, look through pages of interview notes, or rewatch video recordings to find the information we need. This problem compounds, since we are continuously producing research reports and the wealth of information grows infinitely.

The goal of Dovetail is to make research findings searchable, concise, and easy to reference.

Dovetail helps you identify patterns and themes that emerge across your research data and turn those into insight statements. You can analyze and synthesize research findings by [tagging and highlighting raw data](/handbook/engineering/ux/dovetail/#highlight-and-tag-content). Tag highlights with the feature/area of GitLab to which the highlight relates (for example, ‘Merge Requests’) and the persona (for example, ‘Sasha: Software Developer’) who made the comment, if possible. The next step is to [create insight statements](https://dovetailapp.com/help/the-basics/insights/) for your study and support them with the evidence you gathered in the tags, highlights, and charts. After you've created your insight statements, you can use Dovetail's ["presentation mode"](https://dovetailapp.com/help/the-basics/insights/#view-insights-as-a-presentation) feature to share your findings with your team and any other stakeholders. The last step is to provide a link to the Dovetail project directly in the original UX Research issue. Check out this [project](https://dovetailapp.com/projects/838a723f-d93b-48c1-9ade-8b2bd692152c/readme) (internal link only) as a great example of these steps.

#### What is an insight? 
When we conduct research studies, we have a set of [goals and objectives](/handbook/engineering/ux/ux-research-training/defining-goals-objectives-and-hypotheses/) that guide us as we investigate the research question. Whether we're evaluating the usability of a feature, conducting exploratory interviews, or gathering quantitative data, the research study will likely result in a list of observations, patterns, and behaviors related to a user's experience. The raw data from the study are the research findings.

A list of findings, alone, is often not enough to fully communicate how users conceptualize a topic or why they experienced a certain struggle. Through [analysis and synthesis](/handbook/engineering/ux/ux-research-training/defining-goals-objectives-and-hypotheses/) of the data gathered in a research study, we are able to distill *insights* that connect the dots between related concerns and provide an additional layer of understanding. 

There are two types of insights: [Actionable and Informative](/handbook/engineering/ux/ux-research-training/research-insights/).

  - Actionable insights are findings that require an action to be taken to resolve them. These can include UI changes, feature additions, and even conducting additional research.  All of these insights require the person conducting the research to create a GitLab issue that documents the actionable insight along with a proposed path for a solution.
  - Informative insights are findings that provide additional insights into topics, but for which no action needs to be taken as there is nothing to resolve. Informative insights are created only in Dovetail.

These synthesized research findings evolve into a cohesive collection of insights that enables stakeholders to make informed decisions. We support each insight with evidence that can be referenced during discussions, typically in the form of video clips, interview quotes, or statistical data.

#### So, how does it work?
At the end of each research study, the study's moderator is responsible for documenting the research in Dovetail. The first step is to create a new project in Dovetail, under the folder that corresponds to your product stage (e.g. Manage). The project homepage should provide a link back to the original UX Research issue. If you'd like to provide more context, you can describe the research methodology used in the study and any background information you may have about the research participants.

#### Creating useful insights
It's important to remember that insights often need context, since people may read them in isolation and misinterpret them. As you work on reporting on your study, it's important to keep the audience in mind and think about what you'd like them to learn from the study.

For example, you may find it useful to document all insights (big or small) from studies conducted on the GitLab interface to provide an explanation for why the interface has changed over time. This creates a record of why previous design decisions were not ideal, which can be helpful for discussions with newer team members. On the other hand, for design evaluations or tests with prototypes, it may be more relevant to focus on documenting the insights that answer the overarching research questions, since these studies often result in additional design iterations before implementation.

In either case, adding a brief "context" section at the top of the project description and providing a link to the relevant design artifact can help the reader better understand the background of the study.

#### Leveraging Dovetail insights
Searching through Dovetail is a great way to get acquainted with GitLab users and learn about studies that have already been conducted. You can search and filter through insights, highlights, tags, and charts to find the research that is relevant to any stage, feature, and type of research.

Another approach is to look through the [GitLab workspace homepage](https://dovetailapp.com/home/) in Dovetail if you'd like to see a higher-level overview of research being conducted across the stages (internal access only).

Whether you're looking to better understand a user persona, learn about use cases for features, gather context for solving a problem, or plan a future research study, Dovetail has something for you.

