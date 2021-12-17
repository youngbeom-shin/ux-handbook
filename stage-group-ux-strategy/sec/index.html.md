---
layout: handbook-page-toc
title: "Secure & Protect UX"
description: "We’re designing an experience that enables contributors to commit their most secure work and to protect what they have in production."
---


### Overview
We’re designing an experience that enables contributors to commit their most secure work and to protect what they have in production. This is done by merging security into the DevOps process, giving development teams more ownership, commonly referred to as DevSecOps. The experience brings cross-functional stakeholders together to make better, faster, and more security-oriented decisions. We are doing this by focusing the experience on automation, education, empowerment, and shifting security to the left.

**Automation** referrs to convention over configuration that helps draw a clear path for the user to produce meaningful results. When it comes to web security, no application will ever be 100% secure. That’s why we are focused on integrating automation into every step of the user’s journey, taking the guesswork out of configuration to open up more time on what’s important: resolving known vulnerabilities and identifying attacks or threats.

**Education** for our users so they understand security basics and are aware of security needs in their applications. We want our users to know where vulnerabilities or threats have been detected, visualize the implications, present resources to understand the problem, and provide the tools to facilitate informed decisions about next steps.

**Empowerment** for all users to resolve security issues is essential as cross-functional departments share ownership of security. Our tools strive for an experience where the developer is responsible and the security team is accountable for the organization's security.

**Shifting left** is taking things like QA and other processes typically found later in the ops cycle and moving them to development. Resulting in security problems being addressed earlier and more often.

### Customer
Organizations of all sizes benefit from our tools and the experience of bringing teams together. We provide customers value with workflow efficiency, informed team decision-making, lower risk of security breaches, and attaining compliance requirements. We focus on all aspects of the product — starting with the customer experience. When deciding to use our tools, organizations are often considering the following:

* What languages does the tool support?
* What tests do we need to cover?
* What tests does the tool cover?
* Can it be automated?
* How long will setup take?
* What does setup involve?
* How easy is it to use?
* What technologies do you need to use? (ex. Docker, Kubernetes)
* How lightweight is the tool?
* How does it integrate with our tools?
* How does it integrate with GitLab's product?
* What customer support is offered?
* What are the upcoming features? (we are selling contracted services vs monthly)

### Jobs to be Done
We use the [Jobs to be Done (JTBDs) framework](/handbook/engineering/ux/jobs-to-be-done/) to keep us focused on user goals and to make sure we're supporting users on what they value. See a breakdown of the Secure and Protect Jobs to be Done [here](/handbook/engineering/ux/stage-group-ux-strategy/sec/jtbd/index.html).

We also carry out [UX Scorecard evaluations](/handbook/engineering/ux/ux-scorecards/) for our JTBDs. See UX Scorecards for Secure and Protect, as well as for other stages, [here](https://gitlab.com/groups/gitlab-org/-/epics/1714).

### Team
* [Justin Mandell](https://gitlab.com/jmandell) - Product Design Manager
* [Andy Volpe](https://gitlab.com/andyvolpe) - Senior Product Designer
* [Annabel Dunstone Gray](https://gitlab.com/annabeldunstone) - Senior Product Designer
* [Becka Lippert](https://gitlab.com/beckalippert) - Product Designer
* [Camellia Yang](https://gitlab.com/cam.x) - Senior Product Designer
* [Michael Fangman](https://gitlab.com/mfangman) - Product Designer

#### Team structure
We've divided our stage into dedicated experience groups to align with a similar [split](/handbook/product/categories/#sec-section) undertaken by our engineering and PM counterparts.

**Security Testing**

| Group            | Features                                                     | Designer(s)           |
| ---------------- | ------------------------------------------------------------ | --------------------- |
| Static Analysis  | SAST, Secret Detection, Code Quality                         | Becka Lippert         |
| Dynamic Analysis | DAST                      | Annabel Dunstone Gray (interim), Michael Fangman         |
| Dynamic Analysis | Fuzz Testing                                                 | Camellia Yang         |

**Compliance & Auditing**

| Group                       | Features                                                     | Designer(s)         |
| --------------------------- | ------------------------------------------------------------ | ------------------- |
| Composition Analysis        | Dependency Scanning, Container Scanning, License Compliance  | Secure & Protect UX Team (shared) |

**Threat Insights**

| Group                       | Features                                                     | Designer(s)         |
| --------------------------- | ------------------------------------------------------------ | ------------------- |
| Vulnerability Management    | Vulnerability Management                                     | Andy Volpe          |

**Protect**

| Group                   | Features                                               | Designer(s)                         |
| ----------------------- | ------------------------------------------------------ | ----------------------------------- |
| Container Security Group | Container Network Security, Container Host Security, Security Orchestration, and Container Scanning | Annabel Dunstone Gray     

The Secure & Protect UX teams work closely together and have shared coverage in the following areas:

- Security Dashboards
- Security Reports 
- Security Widgets in the Merge Request
- Status, Metrics and Reporting
- Security Configuration

This segmentation gives us a better opportunity to:
- Grow our expertise and knowledge within our subgroup while sharing relevant information with the rest of the team.
- Evolve and maintain relationships with our dedicated engineering team and PMs.
- Serve as the known main point of contact.
- Deeply understand our users' needs by initiating and/or leading research activities specific to our experience group.
- Focus on iterating and progressing our experiences from MVC to Lovable.

Read more about how we've created these dedicated experience groups [here.](https://gitlab.com/gitlab-org/gitlab-design/issues/458)

#### UX pages
* [Secure UX](/handbook/engineering/ux/stage-group-ux-strategy/secure/)
* [Protect UX](/handbook/engineering/ux/stage-group-ux-strategy/protect/)

### How we work
We follow the [GitLab workflow](/handbook/engineering/workflow/#product-development-timeline) with [additional dates](/handbook/engineering/ux/stage-group-ux-strategy/sec/) and actions that directly tie to our work.

### Team meetings
* Secure and Protect UX (Secure & Protect Team Check-in w/ Configure & Monitor Team) weekly meeting on Tuesdays at 8:00am PST (See below for more details)
* Product Design and Secure PMs (Secure & Protect UX) bi-weekly on Wednesdays at 8:00am PST (We kick off the discussion for the plan of the upcoming milestone)
* Product Design does a bi-weekly refinement session on Tuesdays at 7:30am PST 
* Pre milestone Planning Session Monthly on the second Monday at 9:00am PST (We finalize the plan for the upcoming milestone)

Our weekly meeting is to discuss topics relevant to Secure design, UX, and research and to check-in with each other as a team. Design reviews/feedback are also suggested to begin with our company values of asynchronous communication first. Some example topics could include:
- Updates on in-flight and planned research
- Updates on design issues
- Issues that might be at risk or have blockers
- Recently discovered insights while conducting researching
- Updates to our UX Scorecards
- Updates on changes to UX workflows and processes
- Updates on pilot initiatives we are working on
- Strategy iterations

Some topics are better suited for a dedicated meeting, and should be created on an as-needed basis:
- Milestone planning and refinement
- Design critiques
- Research report readouts
- Syncing on troublesome issues

##### Labels we use
We use `devops::stage_name` and `UX` labels to indicate issues that need UX effort. We work on user flows that often span multiple categories so we review each of these issues prior to the start of a milestone to determine the design assignee or assignees.

* `UX` + `devops::stage_name`: It is a shared UX effort and the engineering effort has not been determined.
* `UX` + `devops::stage_name`+`Category::name`: There is a DRI for UX (can be shared) and clear engineering collaboration.
* `UX` + `devops::stage_name`+ `UX debt`: Used for follow-up issues when a proposed design was de-scoped or not implemented as planned.

See our [UX Workflow](/handbook/engineering/ux/ux-department-workflow/#how-we-use-labels) page for more on how we use labels.

##### Problem and solution validation issues
When working on a `workflow::problem validation` or `workflow:solution validation` issue requiring implementation in the next 2 releases, ensure there is a placeholder implementation issue. This issue must be attached to the epic, and have a tentative milestone.

#### Planning and refinement
We use a [team planning board](https://gitlab.com/groups/gitlab-org/-/boards/2131151?milestone_title=13.11&) as tool to help us monitor our velocity allowing us to more efficiently communicate our time to our counterparts.

At the start of each Milestone, we create a Team Milestone Planning Issue (using the [template below](#team-milestone-planning-issue-template)) to initiate a team discussion around which Issues will need to be worked on in the next, upcoming, milestone (not the milestone that has just begun). We do this to ensure that each Group has:
* Product Designer coverage
* To allow for a greater awareness of the work each Group is doing
* To increase the potential for cross-group collaboration, and
* To increase knowledge across Groups

**`M-1, 17th` (1 month before start of milestone)**
* Product Design Manager (PDM): Create a Planning Issue for the milestone from the team's Planning Issue Template.
* PDM: Assign Issue to entire team
* Team: Discuss the needs for the NEXT milestone's design work with your Product Managers (PM)
* Product Designers (PD) will fill in their expected Group, Flex and TOTAL Capacity in the Product Designer's Available Capacity table

**`M-1, 24th` (~3 weeks before start of milestone)**
* Each PM and Product Designer (PD) counterpart will work together for a week to add content to their Group's UX Needs table
* Each PD will add any OKR or Extra issues they expect to work on during the upcoming milestone to the OKR/Extra UX Needs table

**`M-1, 1st` (~2 weeks before start of milestone)**
* Now that all of the Group's UX Needs tables have been filled in, it's time to discuss if anyone needs additional Product Designer assistance (i.e. An Issue(s) has a priority that is deemed to be higher than another Group's prioritized list or a PM that doesn't have a PD counterpart has work that needs to get done).

**`M-1, 8th` (~1 weeks before start of milestone)**
* Add a new comment for a round table team check-in Thumbs up/down to ensure everyone is covered and happy with the outcome.

**`M, 17th` (Start of milestone)**
* PDM: closes Planning Issue

<!--
* By month `M-1, 4th` (at least 14 days before milestone `m` begins):
     * PM updates planning boards to propose issues that may be included in the next release (released 22nd of next month).
     * Product Designers hold a UX Planning session to review the issues, make assignments, and discuss capacity. UX proposes additional issues to include in the milestone.
     * Each issue is followed with a discussion (comment) to inform our capacity or request additional information.
* By month `M-1, 13th` (at least 5 days before milestone `m` begins):
     * PM finalizes the Release scope. In-scope issues are marked with milestone `m`; label `deliverable` applied.
     * PM updates the Kickoff document with relevant items to be included.
* By month `M-1, 17th` (at least 1 day before milestone `m` begins):
     * Group Kickoffs calls recorded and uploaded by PM.
* On month `M-1, 18th` (or next business day, milestone `m` begins): Kick off! 📣
     * Company Kickoff call live streamed by PM.
     * Development on milestone `m` begins
-->

#### Team Milestone Planning Issue Template

<!-- 
How Does This Work?
	1.	(M1, 22nd) At the start of each Milestone a new Secure Design Planning Issue will be created to discuss the needs for the NEXT Milestone's design work. 
	2.	(M1, 1st) Each Product Mgr (PM) and Product Designer (PD) counterpart will work together for a week to add content to their Group's UX Needs table below.
	3.	(M1, 8th) Group tables have been filled in; it's time to discuss if anyone needs additional Product Designer assistance (i.e. An Issue(s) has a priority that is deemed to be higher than another Group's prioritized list or a PM that doesn't have a PD counterpart has work that needs to get done).
	4.	(M1, 15th) Add a new comment for a round table team check-in Thumbs up/down to ensure everyone is covered and happy with the outcome.
	5.	(M, 22nd) Close the issue and do the work :)
--> 

    ### Secure & Protect Planning Boards
    | Group | Planning Board |
    | --- | --- |
    | Composition Analysis | <!-- link to your groups planning board --> |
    | Container Security | <!-- link to your groups planning board --> |
    | Dynamic Analysis:DAST | <!-- link to your groups planning board --> |
    | Dynamic Analysis:Fuzz | <!-- link to your groups planning board --> |
    | SAST | <!-- link to your groups planning board --> |
    | Vulnerability Management | <!-- link to your groups planning board --> |

    ### Product Designer's Available Capacity
    <!-- Group Capacity is the number of weight points you are able to contribute to your group work this milestone.
    Flex Capacity is any extra weight points you'll hold in reserve to accommodate any OKR, UX Dept or any other extracorricular work that you expect will pop-up during this milestone  -->
    | Designer | Group Capacity | Flex Capacity | TOTAL Capacity |
    | ------ | ------ | ------ | ------ |
    | Andy     |   |   |   |
    | Annabel  |   |   |   |
    | Becka    |   |   |   |
    | Camellia |   |   |   |
    | Michael  |   |   |   |

    ### Composition Analysis UX Needs
    | Priority | Issue/Epic | State | 💯 Need / 💪 Nice to have | Designer | Ready for Build By | ≅ Weight |
    | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
    | 1 | <!-- link goes here  --> | <!-- Ready for design --> | <!-- 💯  --> | <!-- designer name  --> | <!-- Milestone --> | <!-- approx weight --> |
    | 2 | <!--  link goes here  --> | <!-- Needs solution validation --> | <!-- 💪  --> | <!-- designer name  --> | <!-- Milestone  --> | <!-- approx weight --> |

    ### Container Security UX Needs
    | Priority | Issue/Epic | State | 💯 Need / 💪 Nice to have | Designer | Ready for Build By | ≅ Weight |
    | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
    | 1 | <!-- link goes here  --> | <!-- Ready for design --> | <!-- 💯  --> | <!-- designer name  --> | <!-- Milestone --> | <!-- approx weight --> |
    | 2 | <!--  link goes here  --> | <!-- Needs solution validation --> | <!-- 💪  --> | <!-- designer name  --> | <!-- Milestone  --> | <!-- approx weight --> |

    ### Dynamic Analysis:DAST/Fuzz UX Needs
    | Priority | Issue/Epic | State | 💯 Need / 💪 Nice to have | Designer | Ready for Build By | ≅ Weight |
    | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
    | 1 | <!-- link goes here  --> | <!-- Ready for design --> | <!-- 💯  --> | <!-- designer name  --> | <!-- Milestone --> | <!-- approx weight --> |
    | 2 | <!--  link goes here  --> | <!-- Needs solution validation --> | <!-- 💪  --> | <!-- designer name  --> | <!-- Milestone  --> | <!-- approx weight --> |

    ### SAST UX Needs
    | Priority | Issue/Epic | State | 💯 Need / 💪 Nice to have | Designer | Ready for Build By | ≅ Weight |
    | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
    | 1 | <!-- link goes here  --> | <!-- Ready for design --> | <!-- 💯  --> | <!-- designer name  --> | <!-- Milestone --> | <!-- approx weight --> |
    | 2 | <!--  link goes here  --> | <!-- Needs solution validation --> | <!-- 💪  --> | <!-- designer name  --> | <!-- Milestone  --> | <!-- approx weight --> |

    ### Vulnerability Management UX Needs
    | Priority | Issue/Epic | State | 💯 Need / 💪 Nice to have | Designer | Ready for Build By | ≅ Weight |
    | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
    | 1 | <!-- link goes here  --> | <!-- Ready for design --> | <!-- 💯  --> | <!-- designer name  --> | <!-- Milestone --> | <!-- approx weight --> |
    | 2 | <!--  link goes here  --> | <!-- Needs solution validation --> | <!-- 💪  --> | <!-- designer name  --> | <!-- Milestone  --> | <!-- approx weight --> |

    ### OKR/Extra UX Needs
    | Priority | Issue/Epic | State | 💯 Need / 💪 Nice to have | Designer | Ready for Build By | ≅ Weight |
    | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
    | 1 | <!-- link goes here  --> | <!-- Ready for design --> | <!-- 💯  --> | <!-- designer name  --> | <!-- Milestone --> | <!-- approx weight --> |
    | 2 | <!--  link goes here  --> | <!-- Needs solution validation --> | <!-- 💪  --> | <!-- designer name  --> | <!-- Milestone  --> | <!-- approx weight --> |

    <!-- Assign the entire team PMs and PDs -->
    <!-- Set the Milestone (current Milestone) -->
    <!-- Set the Due Date for the end of the current Milestone -->

    /label ~"section::sec" ~"Planning Issue"


##### Understanding capacity
Part of our milestone planning activities include factoring in the amount of effort required for each assigned issue. We use the following scale:

| Size     | Weight | Description                                                  |
| -------- | ------ | ------------------------------------------------------------ |
| Trivial  | 1      | Mostly small to medium UI changes, smaller UX improvements, without unanswered questions. UX may need to stay involved with the issue but might not have to do work. |
| Small    | 2      | Simple UI or UX change where we understand all of the requirements, but may need to find solutions to known questions/problems. |
| Medium   | 3      | A medium change (lots of UI or UX changes/improvements required). Multiple pages are involved, we're starting to design/redesign small flows. Some unknown questions may arise during the work. |
| Large    | 5      | A complicated change where other team members will need to be involved. Spans across multiple pages, we're working on medium-sized flows. There are significant open questions that need to be answered. |
| Huge     | 8      | A complex change that spans across large flows and may require input from other designers. This is the largest flow design/redesign that we would take on in a single milestone. |
| Gigantic | 13     | A significant change that spans across multiple flows and that would require significant input from others (teams, team members, user feedback) and there are many unknown unknowns. It's unlikely we would commit to this in a milestone, and the preference would be to further clarify requirements and/or break in to smaller issues. |

### Our strategy
The Secure and Protect UX teams are working together to [uncover customers core needs](https://gitlab.com/groups/gitlab-org/-/epics/1611), what our users’ workflows looks like, and defining how we can make our users tasks easier. Our strategy involves the following actions:

* [UX Scorecards and recommendations](/handbook/engineering/ux/ux-scorecards/) (quarterly)
* Internal understanding: stakeholder interviews (annually)
* Iterating on Secure product [foundation's document](https://gitlab.com/gitlab-org/gitlab-design/issues/333) (ongoing)
* Iterating on Protect product [foundation's document](https://gitlab.com/gitlab-org/gitlab-design/issues/547) (ongoing)
* Performing heuristic evaluations on at least 3 competitors, based competitors the 3 user type is using (annually, ongoing)
* We talk to our customer (ongoing)
* We talk to our users (ongoing)
* We outline current user workflows and improve them (upcoming, ongoing)

Additionally, we value the following:
* Testing our features with usefulness and usability studies
* Drinking our own wine and partnering closely with our internal Security and Compliance teams for feedback and feature adoption
* Partnering with our sales and account team to connect directly with customers and learn why customers did (or didn’t) choose our product
* Collaborating with stakeholders on proof of concept discoveries to better understand future consideration
* Collaborating between the Secure and Protect teams to make sure we’re offering a consistent and cohesive security workflow so that our customers can apply reactive findings into proactive measures and make sure their applications are protected throughout the entire application lifecycle
* Prioritizing issues that are likely to increase our number of active users

The source of truth lives with shipped features, therefore we:
* Make data-driven decisions quickly and thoughtfully
* Optimize to deliver our solutions as soon as possible
* Learn, iterate, test, and repeat

### Follow our work
Our [Secure and Protect UX YouTube channel](https://www.youtube.com/playlist?list=PL05JrBw4t0KrFCe5BgUkzFrZifjforQOz) includes UX Scorecard walkthroughs, UX reviews, group feedback sessions, team meetings, and more.


