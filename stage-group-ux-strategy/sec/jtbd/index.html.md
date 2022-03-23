---
layout: handbook-page-toc
title: Secure and Protect - JTBD
description: The Jobs-to-be-Done that the Secure and Protect Group is striving to address.
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Overview

The goal of this page is to document, share and iterate on the Jobs to be Done (JTBD) and their corresponding job statements for the Secure and Protect stages. 

These Jobs reflect how the UX team frames the Secure and Protect experience. Combined, these Jobs aim to provide a unified view and a shared understanding of the user experience.

This page is a living document; as our understanding of our users deepens and as changes to the product direction take place, we will update our JTBDs.

## Goals common to all stages

Utilize JTBDs to:

- Understand our users' underlying motivations
- Validate identified problem areas within the stage-group
- Create a common language across teams for better collaboration when working on improving the experience for Secure and Protect
- Create a transparent view for our stakeholders into the current and future state of the product.

## How we use JTBDs in Secure and Protect

We utilize the JTBDs framework in the following ways:
- We generate realistic scenarios for [Category Maturity Scorecard](https://about.gitlab.com/handbook/engineering/ux/category-maturity-scorecards/) studies according to these Jobs.
- We use them for prioritizing upcoming work and creating a product roadmap (see example: [2021 UX Goals for Threat Insights](https://gitlab.com/gitlab-org/gitlab/-/issues/294062)).
- We reference Job Statements in Design issues, to state the user goal which the solution aims to resolve.
- We use them as a compass to align ourselves on a common direction for how Secure and Protect is aiming to help our users.
- We use them to identify collaboration opportunities between categories.

## Guiding principles we use in the creation of our JTBDs

### Break down silos, and stay user-centric
We want to use the JTBDs framework as a way of gaining a shared perspective on what the Secure and Protect user experience is, rather than thinking about it in a siloed, Category-focused, way. The user doesn’t care about our organizational structure, and so our grouping of Job Statements shouldn’t reflect that (i.e. you won’t see SAST/DAST/etc. Job Statements in our list). Striving to break free from [Conway’s Law](https://en.wikipedia.org/wiki/Conway%27s_law), we decided to instead group Job Statements primarily around broad user goals (i.e. Big Jobs), and then have each Category team interpret them as it fits their domain.

### Mutually Exclusive and Collectively Exhaustive
We aspire to create a single set of JTBDs for the entire stage, such that that set is mutually exclusive and collectively exhaustive. This means that there should be no overlap between Jobs, and that together all Jobs should exhaust the user goals that Secure and Protect should address.

### Validate JTBDs with Research
It is important to form hypothetical Jobs to explicitly call out what goals we believe our users have. However hypothetical Job Statements are not actionable yet. They should be validated (or invalidated) through user research.

## JTBD

### Job Hierarchy Diagram
The Job hierarchy diagram represents the relationship between Jobs in a visual way. It focuses solely on Jobs, rather than on full Job Statements, to make the structure more easily digestible.

Note that most, but not all, Jobs fit under the Aspirational Job of “Safeguarding my applications from exploits”. Additional Jobs appear as satellites, supporting this core mission.

[View Job Hierarchy Diagram in Mural](https://app.mural.co/t/gitlab2474/m/gitlab2474/1605789082819/395043ec677f981ce24743be8770829f9caa8770)

### Job Statements

<%= partial("direction/secure/secure-jtbd-list", locals: { stage_key: "Secure and Protect" }) %>

