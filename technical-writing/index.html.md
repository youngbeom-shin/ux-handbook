---
layout: handbook-page-toc
title: "Technical Writing Team"
description: "The Technical Writing team continuously develops the GitLab product documentation to meet users' and administrators' needs."
---


## About Us

The primary goal of the Technical Writing team is to continuously develop the GitLab
product documentation to meet the evolving needs of all users and administrators.

Documentation educates readers about features and best practices,
and enables them to efficiently configure, use, and troubleshoot GitLab. To this end, the
team also manages the [docs.gitlab.com](https://docs.gitlab.com) site and related process and tooling.

Our team comprises:

- A [Senior Technical Writing Manager](/job-families/engineering/technical-writing-manager/#senior-manager-technical-writing).
- Two [Technical Writing Managers](/job-families/engineering/technical-writing-manager/).
- A group of [Technical Writers](/job-families/engineering/technical-writer/).

Technical Writers partner with anyone in the GitLab community who is concerned with
documentation, especially developers, who are typically the first to update docs for the
GitLab features that they code.

If you're interested in updating or creating GitLab product documentation, see our [Technical Writing Fundamentals course](fundamentals/), which includes:
- Guidelines for technical writing.
- GitLab style conventions.
- Information about internal testing.
- Instructions for content types.

Use the private-to-GitLab [#docs](https://gitlab.slack.com/messages/C16HYA2P5)
Slack channel to contact the Technical Writing team. To contact the entire team
in a GitLab issue or MR, use `@gl-docsteam`.

## Training 

GitLab provides [Technical Writing Fundamentals](/handbook/engineering/ux/technical-writing/fundamentals/), a course that introduces basic technical writing concepts that we follow at GitLab. 


## Projects

Technical Writers:

- Act as maintainers of documentation for many [engineering projects](../../projects/).
- Act as authors or reviewers of the documentation in collaboration with others in the GitLab community.
- Are [assigned](#assignments) to specific DevOps stage groups.

For more information on documentation at GitLab, see:

- The [Documentation](../../../documentation/) section of the Handbook.
- [GitLab Documentation guidelines](https://docs.gitlab.com/ee/development/documentation/) in the contributor documentation.
- [Technical Writing Workflow](/handbook/engineering/ux/technical-writing/workflow/)

## Slack channels

The Technical Writing team manages team-specific and general documentation-related Slack channels:

- `#docs`: For generic GitLab documentation discussion.
- `#docs-comments`: For automated messages from [Disqus comments](https://docs.gitlab.com/ee/development/documentation/structure.html#disqus).
- `#docs-processes`: For discussion relating to the [Style Guide group](#style-guide-group) and documentation processes.
- `#docs-tooling`: For discussion relating to the [Test Automation Commitee](#test-automation-committee),
  documentation tooling, and the `gitlab-docs` project.
- `#docs-site-changes`: For automated messages from [`gitlab-docs`](https://gitlab.com/gitlab-org/gitlab-docs) project.
- `#tw-team`: For Technical Writing team chat.
- `#tw-social`: For Technical Writing team social chat!

## Responsibilities

The Technical Writing team is broadly responsible for both developing product documentation content and helping others while they develop content, along with other tasks.

### Prioritization

When evaluating work to meet our stakeholders' needs, we prioritize in the following order:

1. Feature work (including documenting new features, and providing guidance on UI text)
1. OKR-related work
1. Backlog issues (including docs technical debt and implementing content topic design)
1. All other tasks

### Content

- Documentation content, including:
  - Developing new content to meet the needs of the community.
  - Reviewing and collaborating on documentation plans, reviewing doc merge requests or recently merged docs, and ensuring that content meets style and language standards.
  - Reorganizing, revamping, and authoring improved content to ensure completeness and a smooth user experience.
- UI content
  - Collaborating with Product Designers on and review of various forms of UI text, such as microcopy, links from the UI to documentation, error messages, and UI element labels.

### Publishing

[Documentation site](https://docs.gitlab.com/) (docs.gitlab.com) including
maintaining and enhancing the documentation site’s:

- Architecture
- Design
- Automation
- Versioning
- Search
- SEO
- Feedback methods
- Analytics

### Processes

Documentation process, including:

- Ensuring that processes are in place and being followed to keep the GitLab docs up to date.
- Following and optimizing documentation workflows with Product and Engineering, Documentation Team workflows, and the division of work.
- Triaging doc-related issues.
- Refining the [Documentation Style Guide](https://docs.gitlab.com/ee/development/documentation/styleguide/index.html) and continuously improving content about GitLab documentation and its contribution process.
- Making it easier for anyone to contribute to the documentation while efficiently handling community contributions to docs.

#### Style Guide

The [Documentation Style Guide](https://docs.gitlab.com/ee/development/documentation/styleguide/)
provides style recommendations for the product documentation and release posts.

Any Technical Writer (or other contributor) can make suggestions for
documentation style updates or additions by creating an issue or merge request with the
`~tw-style` label, and then assigning the issue or MR to the Style Guide DRI.

Use the following searches to track completed style-related issues:

- [GitLab project style issues](https://gitlab.com/gitlab-org/gitlab/-/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=tw-style)
- [GitLab project style MRs](https://gitlab.com/gitlab-org/gitlab/-/merge_requests?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=tw-style)
- [Technical Writing project style issues](https://gitlab.com/gitlab-org/technical-writing/-/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=tw-style)

#### Testing

The Technical Writing team develops and maintains toolkits to test GitLab's documentation (and other technical content) for problems. These toolkits include (but aren't limited) to:

- Text content and writing style: markdownlint, Vale
- Text formatting: Markdownlint, yamllint
- Link validity: nanoc
- File permissions and naming: `lint-doc.sh`

Any contributor can suggest changes to our linting rules or tooling by creating an issue or merge request with the [`~tw-testing`](https://gitlab.com/gitlab-org/gitlab/-/issues?label_name[]=tw-testing) label, and then assigning the issue or MR to a technical writer.

### Collaboration

Collaboration, including:

- Working on documentation efforts with Product, Support, Marketing, Engineering, Community Marketing, other GitLab teams, and the wider GitLab community.
- Ensuring that relevant documentation is easily accessible from within the product.
- Acting as reviewers of the monthly [release post](../../../marketing/blog/release-posts/).

### Assignments

Technical Writers (TWs) are assigned to and collaborate with other teams and
groups as described on the [DevOps stages](#designated-technical-writers),
[Development Guidelines](#assignments-to-development-guidelines), and
[other subjects](#assignments-to-other-projects-and-subjects) sections below.

#### Assignments to DevOps Stages and Groups
{: #designated-technical-writers}

The designated Technical Writer is the go-to person for their assigned
[stage groups](../../../product/product-categories/). They collaborate with
other team members to plan new documentation, edit existing documentation,
review any proposed changes to documentation, suggest changes to the microcopy
exposed to users, and generally partner with subject matter experts (SMEs) in
all situations where documentation is required.

The backup writer is assigned to cover merge request reviews and
urgent matters for the designated tech writer when they are out
(vacations, sickness, and any other temporary leave). They can
also naturally pair to work together on complex issues when needed.

**Note:** If you've been directed here from metadata in a documentation page
that has `none` as the stage, refer to the
[Assignments to other projects and subjects](#assignments-to-other-projects-and-subjects)
section, referencing the group shown in metadata with the listed Subjects in the table.

Not sure who's responsible for a feature? Review feature assignments by [stage](https://about.gitlab.com/features/) or [group](/handbook/product/product-categories/features/).
{: .alert .alert-info}

<%= partial("includes/stages/tech-writing") %>

<!--
  To update the table above:

  - For tech writer's name per stage, change data/stages.yml and includes/stages/tech-writing.html.haml
  - To turn off a stage, set tw: false in data/stages.yml

Reference: https://gitlab.com/gitlab-com/www-gitlab-com/merge_requests/24952
-->

Technical Writers are encouraged to review and improve documentation of other
stages but they aren't required to. When contributing to docs they don't own,
they must respect the assigned TW's ownership and ensure to request their review
and approval when adding significant changes to their docs.

#### Assignments to other projects and subjects

For collaboration in other projects and subjects:

| Subject | Assigned Technical Writer/DRI | Backup/Team members |
|---------|-------------------------------|---------------------|
| [Development guidelines](#assignments-to-development-guidelines) | [Marcia Ramos] | |
| [Style Guide](#style-guide) | [Suzanne Selhorn] | [Susan Tacker] |
| [Testing/Vale/markdownlint](#testing) | [Craig Norris], [Diana Logan] | n/a |
| [Documentation guidelines](https://docs.gitlab.com/ee/development/documentation/) | [Craig Norris] | [Diana Logan] |
| [Documentation handbook](/handbook/documentation/) | [Diana Logan] | [Craig Norris] |
| [Technical Writing handbook](/handbook/engineering/ux/technical-writing/) | [Susan Tacker] | [Craig Norris], [Diana Logan] |
| [Get started administering Gitlab](https://docs.gitlab.com/ee/administration/get_started.html) (TAM onboarding)| [Lyn Landon] | [Kati Paizee] |

[Amy Qualls]: https://gitlab.com/aqualls
[Axil]: https://gitlab.com/axil
[Craig Norris]: https://gitlab.com/cnorris
[Diana Logan]: https://gitlab.com/dianalogan
[Evan Read]: https://gitlab.com/eread
[Kati Paizee]: https://gitlab.com/kpaizee
[Lyn Landon]: https://gitlab.com/llandon
[Marcel Amirault]: https://gitlab.com/marcel.amirault
[Marcia Ramos]: https://gitlab.com/marcia
[Marcin Sędłak-Jakubowski]: https://gitlab.com/msedlakjakubowski
[Marcin Sedlak-Jakubowski]: https://gitlab.com/msedlakjakubowski
[Mike Jang]: https://gitlab.com/mjang1
[Nick Gaskill]: https://gitlab.com/ngaskill
[Russell Dickenson]: https://gitlab.com/rdickenson
[Susan Tacker]: https://gitlab.com/susantacker
[Suzanne Selhorn]: https://gitlab.com/sselhorn

#### Assignments to Development Guidelines

As GitLab grows, it's important to keep high-quality documentation, and ensure that the
guidelines for contributors are consistent and aligned throughout the organization.
Development Guidelines consist of:

- GitLab's [Development Guidelines](https://docs.gitlab.com/ee/development/):
  The processes and technical information needed for contributing to GitLab. Use
  the [Development Guidelines review process](https://docs.gitlab.com/ee/development/#development-guidelines-review)
  for any changes or updates to documentation in the `/development` directory.
- [GitLab Design System ("Pajamas")](https://design.gitlab.com/): The entire content of
  [`contents`](https://gitlab.com/gitlab-org/gitlab-services/design.gitlab.com/-/tree/main/contents)
  must be reviewed and approved by the TW assigned to Dev Guidelines.
- [GitLab UI](https://gitlab.com/gitlab-org/gitlab-ui/): Documentation in this
  project doesn't require TW review. The TW for Dev Guidelines will help in
  creating and maintaining minimum requirements for this documentation through
  specific guidelines and templates, and assist the team on request.

The Technical Writer assigned to Development Guidelines is [Marcia Ramos]. For regular merge request reviews:

- If you are submitting [broader changes](https://docs.gitlab.com/ee/development/#broader-changes)
to development guidelines, ask the Technical Writer assigned to Development Guidelines to review your merge request.
- If you are submitting [group-specific development guidelines](https://docs.gitlab.com/ee/development/#specific-changes),
ask the Technical Writer assigned to your group to review them instead.
- For [minor fixes and typos](https://docs.gitlab.com/ee/development/#wording-style-or-link-changes),
any GitLab Maintainer can review and merge your merge request.


<!-- References:
- All Dev Guidelines: https://gitlab.com/gitlab-org/technical-writing/issues/108
- Pajamas: https://gitlab.com/gitlab-org/technical-writing/issues/93
- GitLab UI: https://gitlab.com/gitlab-org/gitlab-ui/issues/598, https://gitlab.com/gitlab-org/gitlab-ui/issues/624
-->

#### Backup Technical Writers

Each Technical Writer has an assigned *backup Technical Writer* that’s listed in
the [DevOps Stages and Groups assignment table](#assignments).

Although the usual role of a backup Technical Writer is to provide coverage for
primary writers who may be out of the office, the backup can also be a resource for
a stage/group's normal Technical Writer. For example, depending on their
bandwidth, the backup may be able to help with coverage if the primary Technical
Writer gets too busy (for example, if the primary writer also has
[release post duty](/handbook/marketing/blog/release-posts/managers/)).

Technical Writers should ensure that their out-of-office messaging reflects
their backup, and should communicate with their PMs and developers to introduce
their backup Technical Writer.

Whenever you’re communicating with a backup Technical Writer to ask for an
issue's status or their assistance with a technical writing issue, please be
aware that they may require additional context, and that your request will need
to be incorporated into the list of stage/group and feature priorities for
*their* primary responsibility.

If neither the primary or backup Technical Writer are available to help, you can
post in the [#docs](https://gitlab.slack.com/archives/C16HYA2P5) channel to
ask for general assistance for your issue.

#### Regularly scheduled tasks

Along with Technical Writers' normally assigned work, there are recurring tasks
that need to be regularly completed:

- **Release Post Technical Writing Lead:** The Technical Writing Lead
  [reviews the content](/handbook/marketing/blog/release-posts/#tw-lead)
  for the release post published at the end of each milestone. See the
  [Release Post Scheduling](/handbook/marketing/blog/release-posts/managers/)
  Handbook page for the most updated list of each milestone's assigned writer.
  The Technical Writing Lead also
  [creates the monthly version for the docs site](/handbook/engineering/ux/technical-writing/workflow/#monthly-documentation-releases).
- **Docs project maintenance tasks:** Each month, one Technical Writer is assigned
  to complete maintenance tasks for the documentation site and its content. This
  involves [creating a new issue](https://gitlab.com/gitlab-org/technical-writing/-/issues/new)
  in the `technical-writing` repository to track maintenance work (using
  the `tw-monthly-tasks` template). If additional work beyond what's described
  in the maintenance issue is required, the Technical Writer will create merge
  requests and additional issues as needed.

Current schedule of regular Technical Writing team tasks:

| Month    | Release Post                      | Maintenance tasks          |
|----------|-----------------------------------|----------------------------|
| Jan 2021 | 13.8 - [Marcia Ramos]             | [Suzanne Selhorn]          |
| Feb 2021 | 13.9 - [Russell Dickenson]        | [Nick Gaskill]             |
| Mar 2021 | 13.10 - [Mike Jang]               | [Marcel Amirault]          |
| Apr 2021 | 13.11 - [Russell Dickenson]       | [Evan Read]                |
| May 2021 | 13.12 - [Suzanne Selhorn]         | [Axil]                     |
| Jun 2021 | 14.0 - [Amy Qualls]               | [Marcin Sędłak-Jakubowski] |
| Jul 2021 | 14.1 - [Marcel Amirault]          | [Marcia Ramos]             |
| Aug 2021 | 14.2 - [Evan Read]                | [Russell Dickenson]        |
| Sep 2021 | 14.3 - [Kati Paizee]              | [Amy Qualls]               |
| Oct 2021 | 14.4 - [Nick Gaskill]             | [Suzanne Selhorn]          |
| Nov 2021 | 14.5 - [Axil]                     | [Nick Gaskill]             |
| Dec 2021 | 14.6 - [Marcin Sędłak-Jakubowski] | [Marcel Amirault]          |

**Note:** Be sure to keep the Release Post column in sync with the [Release Post Scheduling](/handbook/marketing/blog/release-posts/managers/) page.

### Hiring Technical Writers

See how to participate in the [hiring process for Technical Writers](hiring/).

### Onboarding Technical Writers

While the Technical Writer is onboarding, they will be assigned to
shadow groups and then start contributing as trainees, as described
below. Veteran Technical Writers will coach them through the process.

#### Group shadowing

For the first release cycle that begins after the new member start
date, they will shadow (read) their buddy's work in their most active
Stage Group, plus one other stage group/writer decided with the
tech writing manager and the team. Veteran Technical Writers will
proactively share relevant issues, merge requests, and communications
with their shadows by using a `#tw-onboarding-<groupname>`
Slack channel, creating it if it doesn't already exist, and answering questions.

#### Group trainees

For the second release cycle that begins after the new member's start
date, unless the tech writing manager extends the shadowing phase,
they will act as a trainee on one or more groups as assigned by the manager.
The intent is to take on the group as its Technical Writer as of the
next release. The veteran Technical Writer who is assigned to that Group
will assign substantial parts of the work to the new member for this group,
which accounts to roughly half of the groups's reviews of MRs with docs, UI text,
and release post content; a small but substantial documentation
authoring project; a few minor doc improvement projects/fixes.

#### Group coaching

For the third release cycle, the onboarding tech writer assumes the
full role of Technical Writer for their assigned group, except that
they will not yet have [merge rights](#merge-rights). The former TW assigned to the group is now the coach,
who will review all their work (including reviews they perform of other authors)
before merging it or approving it for another maintainer to merge.
They may share the burden of these reviews with other Technical Writers.

### Reviews

Technical Writers are assigned merge requests to review that contain documentation changes
authored by GitLab team members and community contributors.
The reviews are assigned by subject matter according to the [Technical Writer assignments](#assignments)
to [stage groups](../../product/product-categories/#devops-stages) or other specialties.

#### Review principles

The following principles guide Technical Writers when conducting technical writing reviews:

- A technical writing review aims to confirm that the content:
  - Is clear, grammatically correct, discoverable, navigable, and written with the perspective of the user (or other intended audience) in mind.
  - Follows the [Documentation Style Guide](https://docs.gitlab.com/ee/development/documentation/styleguide/).
    and Pajamas Design System content guidance on:
    - [Voice and tone](https://design.gitlab.com/content/voice-tone).
    - [Terminology](https://design.gitlab.com/content/terminology).
    - [Punctuation](https://design.gitlab.com/content/punctuation).
  - Avoids redundancy, bad file locations, typos, and broken links.
- While Technical Writers apply any subject-matter expertise they possess, a technical writing
  review focuses on tone, style, and narrative flow.
- A technical writing review confirms that an authoritative source has checked for technical accuracy.
  The Technical Writer may serve as that authoritative source if they have the required knowledge or
  can efficiently perform any necessary verification.
- Because every writer can benefit from an editorial review, content changes (except, at the Technical Writer's discretion, very small changes)
  submitted by Technical Writers should go to another Technical Writer for review before merge. When in doubt, ask for a review.
  Because [velocity](/handbook/engineering/#the-importance-of-velocity) is important, Technical
  Writers can request a post-merge review from another Technical Writer in exceptional circumstances.
- To mirror development best practices and to encourage proper reviews, Technical Writers don't merge documentation changes for which they're the original author.
- The use of suggestions and the self-application of suggestions is between the the Technical Writer and their reviewer. Technical Writers should be clear when communicating with reviewers, and work collaboratively.

#### Selecting a reviewer

Technical Writers have the following options when selecting a reviewer for their merge requests.
They can select:

- A writer based on the [GitLab Review Workload Dashboard](https://gitlab-org.gitlab.io/gitlab-roulette/).
  Filter the list to show only Technical Writers and sort by **Assign events last 7 days**.
- Their [Technical Writer backup](/handbook/engineering/ux/technical-writing/#designated-technical-writers).
- A Technical Writer in [their timezone](/company/team/).
- A random Technical Writer.

No option is preferred over others, and all are suited to different situations.

### Merge rights

The Technical Writing team is given merge rights (through
[Maintainer access](/handbook/engineering/workflow/code-review/#how-to-become-a-project-maintainer))
to GitLab projects as part of their role. Not all developers get Maintainer access. Technical
writers should use this privilege responsibly.

As Maintainers, Technical Writers should limit what they merge to:

- Documentation, typically in Markdown-formatted files.
- UI text, error messages, and link-related fixes, with the approvals of appropriate engineer(s).
- Documentation-related tooling and configuration such as linters, and changes
  to the [`gitlab-docs`](https://gitlab.com/gitlab-org/gitlab-docs) project. Engineers in the
  [Editor team](/handbook/engineering/development/dev/create-editor/) are
  available for code review and merges.

In addition, Technical Writers should:

- Never merge an MR with a failed pipeline, unless the failures are unrelated to the changes. If in
  doubt, ask an engineer.
- Ensure that MRs are complete before merging, with appropriate labels and milestones.
- Ensure that the DRI or nominated backup (for [the stage](#assignments) or
  other documentation has reviewed
  and approved the MR.

## Documentation process

See:

- [Technical writing workflow](workflow/) in the handbook.
- [Documentation workflows](https://docs.gitlab.com/ee/development/documentation/workflow.html) in the contributor documentation.
- [Setting up a local environment](setup/) in the handbook.

## Community contribution opportunities

While we welcome [improvements to documentation](/community/contribute/documentation/)
from the community, we also encourage people to contribute to the development of our product
documentation website, at https://docs.gitlab.com.

If you'd like to help us further improve our documentation site, here are some resources:

- [List of available issues](https://gitlab.com/gitlab-org/gitlab-docs/-/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=Accepting%20merge%20requests)
- [Gitlab Docs repo](https://gitlab.com/gitlab-org/gitlab-docs)
- [Gitlab Docs README file](https://gitlab.com/gitlab-org/gitlab-docs/-/blob/master/README.md):
  The things you need to know to get started.
