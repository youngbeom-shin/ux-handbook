---
layout: handbook-page-toc
title: "Technical Writing workflows"
description: "This document explains the workflows of the Technical Writing team."
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

This document explains the workflows of the Technical Writing team.

These processes work in conjunction with the:

- [Product development flow](/handbook/product-development-flow/).
- [Product designer workflow](/handbook/engineering/ux/ux-designer).
- [Engineering workflow](/handbook/engineering/workflow/).
- Broader information about contributing to GitLab found in
  [PROCESS.md](https://gitlab.com/gitlab-org/gitlab/blob/master/PROCESS.md).

## Documentation authoring and review

The process for creating and maintaining GitLab product documentation depends
on whether the documentation is:

- [A new feature or feature enhancement](#for-a-product-change).

  Delivered for a specific milestone and associated with specific code changes.
  This documentation has the highest priority.

- [Changes outside a specific milestone](https://docs.gitlab.com/ee/development/documentation/workflow.html).

  Usually not associated with a specific code change, is of lower priority, and
  is open to all GitLab contributors. The process for these changes are
  documented in GitLab's documentation.

Documentation isn't usually required when a *backstage feature* is added or
changed, and doesn't directly affect the way that any user or administrator
interacts with GitLab.

### For a product change

Documentation is required for any new or changed feature, and is:

- Created or updated as part of feature development, and is almost always in
  the same merge request as the feature code. Including documentation in the
  same merge request as the code eliminates the possibility that code and
  documentation get out-of-sync.
- Required with the delivery of a feature for a specific milestone as part of
  GitLab's [definition of done](https://docs.gitlab.com/ee/development/contributing/merge_request_workflow.html#definition-of-done).
- Often linked from the release post.

#### Roles and responsibilities

Documentation for specific milestones involves the:

- Developer of a feature or enhancement.
- Product Manager for the group delivering the new feature or feature
  enhancement.
- Technical Writer assigned to the group.

Each role is described below.

##### Developers

Developers are the primary author of documentation for a feature or feature
enhancement. They are responsible for:

- Developing initial content required for a feature.
- Liaising with their Product Manager to understand what documentation must be
  delivered, and when.
- Requesting technical reviews from other developers within their group.
- Requesting documentation reviews from the Technical Writer
  [assigned to the DevOps stage group](../#assignments)
  that is delivering the new feature or feature enhancements.

The first merge request where a feature can be tested should include the
documentation, even if the feature is behind a feature flag.

The author of this MR, either a frontend or backend developer, should write the documentation.

**Note:** Community Contributors can ask for additional help from GitLab team
members.
{: .note}

###### Authoring

Because the documentation is an essential part of the product, if a `~feature`
issue also contains the `~documentation` label, you must ship the new or
updated documentation with the code of the feature.

Technical Writers are happy to help, as requested and planned on an
issue-by-issue basis.

For feature issues requiring documentation, follow the process below unless
otherwise agreed with the Product Manager and Technical Writer for a given
issue:

- Include any new and edited documentation, either in:
  - The merge request introducing the code.
  - A separate merge request raised around the same time.
- Use the [documentation requirements](#documentation-requirements) developed
  by the Product Manager in the issue and discuss any further documentation
  plans or ideas as needed.

  If the new or changed documentation requires extensive collaboration or
  conversation, a separate, linked issue can be used for the planning process.

- Use the [Documentation guidelines](https://docs.gitlab.com/ee/development/documentation/index.html),
  and other resources linked from there, including:
  - Documentation [Structure and template](https://docs.gitlab.com/ee/development/documentation/structure.html) page.
  - [Style Guide](https://docs.gitlab.com/ee/development/documentation/styleguide.html).
  - [Markdown Guide](https://docs.gitlab.com/ee/user/markdown.html).
- Contact the Technical Writer for the relevant
  [DevOps stage](../#assignments)
  in your issue or merge request, or within `#docs` on GitLab Slack, if you:
  - Need any help to choose the correct place for documentation.
  - Want to discuss a documentation idea or outline.
  - Want to request any other help.
- If you are working on documentation in a separate merge request, ensure the
  documentation is merged as close as possible to the code merge.
- If the feature has a feature flag, [follow the policy for documenting feature-flagged issues](https://docs.gitlab.com/ee/development/documentation/feature_flags.html).

###### Reviews and merging

Prior to merging, documentation changes committed by the developer must be
reviewed by:

- The code reviewer for the merge request. This is known as a technical review.
- Optionally, others involved in the work such as other developers or the
  Product Manager.
- The Technical Writer for the DevOps stage group, except in exceptional
  circumstances where a [post-merge review](https://docs.gitlab.com/ee/development/documentation/workflow.html#post-merge-reviews)
  can be requested.
- A maintainer of the project.

##### Product Managers

Product Managers are responsible for the
[documentation requirements](#documentation-requirements) for a feature or
feature enhancement. They can also:

- Liaise with the Technical Writer for discussion and collaboration.
- Review documentation themselves.

For issues requiring any new or updated documentation, the Product Manager
must:

- Add the ~documentation label.
- Confirm or add the [documentation requirements](#documentation-requirements).
- Ensure the issue contains:
  - Any new or updated feature name.
  - Overview, description, and use cases when applicable (as required by the
    [documentation structure and template](https://docs.gitlab.com/ee/development/documentation/structure.html).

Everyone is encouraged to draft the documentation requirements in the issue.
However, a Product Manager will:

- When the issue is assigned a release milestone, review and update the
  Documentation details.
- By the kickoff, finalize the documentation details.

##### Technical Writers

Technical Writers are responsible for:

- Participating in issue discussions and reviewing MRs for the upcoming
  milestone.
- Reviewing documentation requirements in issues when called upon.
- Answering questions, and helping and providing advice throughout the
  authoring and editing process.
- Reviewing all significant new and updated documentation content, whether
  before merge or after it is merged, in accordance with [review principles](/handbook/engineering/ux/technical-writing/#review-principles).
- Assisting the developer and Product Manager with feature documentation
  delivery.
- Ensuring that issues and MRs are labeled appropriately, and that doc content:
  - Has the correct [metadata](https://docs.gitlab.com/ee/development/documentation/index.html#metadata).
  - Has an entry in the repo's CODEOWNERS file, if one exists (typically
    [CODEOWNERS](https://gitlab.com/gitlab-org/gitlab/-/blob/master/.gitlab/CODEOWNERS)
    in `gitlab-org/gitlab` repo). The entry can be a path if all its files are
    owned by the same group; otherwise include references to individual files.

###### Planning

The Technical Writer:

- Reviews their group's `~feature` issues that are part of the next milestone
  to get a sense of the scope of content likely to be authored.
- Recommends the `~documentation` label on issues from that list which don't
  have it but should, or inquires with the PM to determine if documentation is
  truly required.
- For `~direction` issues from that list, reads the full issue and reviews its
  Documentation requirements section. Addresses any recommendations or
  questions with the PMs and others collaborating on the issue in order to
  refine or expand the Documentation requirements.

###### Collaboration

By default, the developer will work on documentation changes independently, but
the developer, Product Manager, or Technical Writer can propose a broader
collaboration for any given issue.

Additionally, Technical Writers are available for questions at any time.

###### Review

Technical Writers:

- Provide non-blocking reviews of all documentation changes, before or after
  the change is merged. Identified issues that would block or slow a change's
  release are to be handled in linked, follow-on MRs.
- Follow technical writing [review principles](/handbook/engineering/ux/technical-writing/#review-principles).

#### When documentation is required

Documentation [is required](https://docs.gitlab.com/ee/development/contributing/merge_request_workflow.html#definition-of-done)
for a milestone when:

- A new or enhanced feature is shipped that impacts the user or administrator
  experience.
- There are changes to the user interface or API.
- A process, workflow, or previously documented feature is changed.
- A feature is deprecated or removed.

**Note:** Documentation refactoring unrelated to a feature change is covered by
the [process for changes not related to a specific milestone](https://docs.gitlab.com/ee/development/documentation/workflow.html),
which allows for time-sensitive documentation updates to be prioritized.
{: .note}

#### Documentation requirements

Requirements for the documentation of a feature should be included as part of
the issue for planning that feature in a **Documentation** section within the
issue description. Issues created using the
[**Feature Proposal** template](https://gitlab.com/gitlab-org/gitlab/-/raw/master/.gitlab/issue_templates/Feature%20proposal%20-%20detailed.md)
have this section by default.

Anyone can add these details, but the Product Manager who assigns the issue to
a specific release milestone will ensure these details are present and
finalized by the time of that milestone's kickoff.

Developers, Technical Writers, and others may help further refine this plan at
any time on request.

The following details should be included:

- What concepts and procedures should the documentation guide and enable the
  user to understand or accomplish?
- To this end, what new page(s) are needed, if any? What pages or subsections
  need updates? Consider changes and additions to user, admin, and API
  documentation.
- For any guide or instruction set, should it help address a single use case,
  or be flexible to address a certain range of use cases?
- Do we need to update a previously recommended workflow? Should we link the
  new feature from various relevant locations? Consider all ways documentation
  should be affected.
- Are there any key terms or task descriptions that should be included so that
  the documentation is found in relevant searches?
- Include suggested titles of any pages or subsection headings, if applicable.
- List any documentation that should be cross-linked, if applicable.

#### Including documentation with code

Currently, the Technical Writing team strongly encourages including
documentation in the same merge request as the code that it relates to, but
this isn't strictly mandatory. It's still common for documentation to be added
in an MR separate from the feature MR.

Engineering teams may elect to adopt a workflow where it is **mandatory** that
documentation is included in the code MR, as part of their
[definition of done](https://docs.gitlab.com/ee/development/contributing/merge_request_workflow.html#definition-of-done).
When a team adopts this workflow, that team's engineers must include their
documentation in the **same** MR as their feature code, at all times.

##### Downsides of separate documentation MRs

A workflow that has documentation separated into its own MR has many downsides.

If the documentation merges **before** the feature:

- GitLab.com users might try to use the feature before it's released, driving
  support tickets.
- If the feature is delayed, the documentation might not be pulled/reverted in
  time and could be accidentally included in the self-managed package for that
  release.

If the documentation merges **after** the feature:

- The feature might be included in the self-managed package, but without any
  documentation if the documentation MR misses the cutoff.
- A feature might show up in the GitLab.com user interface before any
  documentation exists for it. Users surprised by this feature will search for
  documentation and won't find it, possibly driving support tickets.

Having two separate MRs means:

- Two different people might be responsible for merging one feature, which
  isn't workable with an asynchronous work style. The feature might merge while
  the Technical Writer is asleep, creating a potentially lengthy delay between
  the two merges.
- If the documentation MR is assigned to the same maintainer as responsible for
  the feature code MR, they will have to review and juggle two MRs instead of
  dealing with just one.

Documentation quality might be lower, because:

- Having documentation in a separate MR will mean far fewer people will see and
  verify them, increasing the likelihood that issues will be missed.
- In a *split* workflow, engineers might only create the documentation MR after
  the feature MR is ready, or almost ready. This gives the Technical Writer
  little time to learn about the feature in order to do a good review. It also
  increases pressure on them to review and merge faster than desired, letting
  problems slip in due to haste.

##### Benefits of always including documentation with code

Including documentation with code (and doing it early in the development
process) has many benefits:

- There are no timing issues connected to releases:
  - If a feature slips to the next release, the documentation slips too.
  - If the feature *just* makes it into a release, the documentation *just*
    make it in too.
  - If a feature makes it to GitLab.com early, the documentation will be ready
    for our early adopters.
- Only a single person will be responsible for merging the feature (the code
  maintainer).
- The Technical Writer will have more time to gain an understanding of the
  feature and will be better able to verify the content of the documentation in
  the Review App or GDK. They will also be able to offer advice for improving
  the user interface text or offer additional use cases.
- The documentation will have increased visibility:
  - Everyone involved in the merge request can review the documentation. This
    could include product managers, multiple engineers with deep domain
    knowledge, the code reviewers, and the maintainer. They will be more likely
    to catch issues with examples, and background or concepts that the
    Technical Writer may not be aware of.
  - Increasing visibility of the documentation also has the side effect of
    improving *other* engineers' documentation. By reviewing each other's MRs,
    each engineer's own documentation skills will improve.
- Thinking about the documentation early can help engineers generate better
  examples, as they will need to think about what examples a user will want,
  and will need to ensure the code they write implements that example properly.

##### Documentation with code as a workflow

In order to have documentation included with code as a mandatory workflow, some
changes might need to happen to a team's current workflow:

- The engineers must strive to include the documentation early in the
  development process, to give ample time for review, not just from the
  Technical Writer, but also the code reviewer and maintainer.
- Reviewers and maintainers must also review the documentation during code
  reviews, to ensure the described processes match the expected use of the
  feature, and that examples
  are correct. They *don't* need to worry about style, grammar, and so on.
- The Technical Writer must be assigned the MR directly and not only pinged.
  Thanks to the ability to have
  [multiple assignees for any MR](https://docs.gitlab.com/ee/user/project/merge_requests/getting_started.html#multiple-assignees),
  this can be done at any time, but must be before the code maintainer review.
  It's common to have both the documentation and code reviews happening at the
  same time, with the author, reviewer and Technical Writer discussing the
  documentation together.
- When the documentation is ready, the Technical Writer will click **Approve**
  and usually will no longer be involved in the MR. If the feature changes
  during code review and the documentation is updated, the Technical Writer
  must be reassigned the MR to verify the update.
- Maintainers are allowed to merge features with the documentation *as-is*,
  even if the Technical Writer hasn't given final approval yet. The
  **documenation reviews must not be blockers**. Therefore it's important to
  get the documentation included and assigned to the Technical Writers early.
  If the feature is merged before final documentation approval, the maintainer
  must create a [post-merge follow-up issue](https://docs.gitlab.com/ee/development/documentation/workflow.html#post-merge-reviews),
  and assign it to both the engineer and Technical Writer.

Maintainers are allowed to merge features with the documentation *as-is*, even
if the Technical Writer hasn't given final approval yet but the merge request
has all other required approvals.

You can visualize the parallel workflow for code and documentation reviews as:

```mermaid
graph TD
  A("Feature MR Created (Engineer)") --> |Assign| B("Code Review (reviewer)")
  B --> |"Approve / Reassign"| C("Code Review (maintainer)")
  C --> |Approve| F("Merge (maintainer)")
  A --> D("Docs Added (Engineer)")
  D --> |Assign| E("Docs Review (Tech Writer)")
  E --> |Approve| F
```

For complex features split over multiple merge requests:

- If a merge request is implementing components for a future feature, but the
  components aren't accessible to users yet, then no documentation should be
  included.
- If a merge request will expose a feature to users in any way, such as an
  enabled user interface element, an API endpoint, or anything similar, then
  that MR **must** have documentation. Note that this may mean multiple
  documentation additions could happen in the buildup to the implementation of
  a single large feature, for example API documentation and feature usage
  documentation.
- If it's unclear which engineer should add the feature documentation into
  their MR, the engineering manager should decide during planning, and tie the
  documentation to the last MR that must be merged before a feature is
  considered released. This is often, but not always, a frontend MR.

## UI text

### Planning and authoring

A Product Designer should consult with the Technical Writer for their stage group when planning to add
or change substantial text within the UI, such as a phrase of explanatory microcopy or a link to documentation.

The Technical Writer can offer an initial review of any ideas, plans, or actual text, and can be asked to
draft text when provided with information on the context and goals of the text. Context may include
detail on the scenarios in which the text would appear (for example, to all users viewing the feature
or only under certain conditions), and the information to convey, which typically answers
one or more of the questions:

- What does this do?
- How do I use it?
- Why should I care?

### MR Reviews

Once the merge request is created, all changes and additions to text in the UI *must* be reviewed by
the Technical Writer in accordance with [review principles](/handbook/engineering/ux/technical-writing/#review-principles).

These may include: labels (buttons, menus, column headers, UI sections) or any phrases that may be
displayed within the UI, such as user-assistance microcopy or error messages.

Additional information about composing and reviewing UI text:

- "[Copy That: Helping your Users Succeed with Effective Product Copy](https://www.youtube.com/watch?v=M_Q1RO0ky2c)", a talk by Sarah Day.

## Release posts

The Technical Writer for each [stage group](/handbook/product/categories/#devops-stages)
is a reviewer of their group's [feature blocks](/handbook/marketing/blog/release-posts/#content-reviews) (also known as release post items) authored by the Product Manager.

For each release, a single Technical Writer is also assigned as the [Technical Writing Lead](/handbook/marketing/blog/release-posts/#tw-lead) to perform
the [Structural Check](/handbook/marketing/blog/release-posts/#structural-check) and other duties.

## Monthly documentation releases

When a new GitLab version is released on the 22nd, we release version-specific published
documentation for the new version.

We complete the process as soon as possible after the GitLab version is announced. The result is:

- The [online published documentation](https://docs.gitlab.com) includes:
  - The three most recent minor releases of the current major version. For example 13.9, 13.8, and
    13.7.
  - The most recent minor releases of the last two major versions. For example 12.10, and 11.11.
- Documentation updates after the 22nd are for the next release. The versions drop down
  should have the current milestone with `-pre` appended to it, for example `13.10-pre`.

Each documentation release:

- Has a dedicated branch, named in the format `XX.yy`.
- Has a Docker image that contains a build of that branch.

For example:

- For [GitLab 13.9](https://docs.gitlab.com/13.9/index.html), the
  [stable branch](https://gitlab.com/gitlab-org/gitlab-docs/-/tree/13.9) and Docker image:
  [`registry.gitlab.com/gitlab-org/gitlab-docs:13.9`](https://gitlab.com/gitlab-org/gitlab-docs/container_registry/631635).
- For [GitLab 13.8](https://docs.gitlab.com/13.8/index.html), the
  [stable branch](https://gitlab.com/gitlab-org/gitlab-docs/-/tree/13.8) and Docker image:
  [`registry.gitlab.com/gitlab-org/gitlab-docs:13.8`](https://gitlab.com/gitlab-org/gitlab-docs/container_registry/631635).

### Recommended timeline

To minimize problems during the documentation release process, use the following timeline:

- Any time before the 17th of the month:

  [Add the charts version](#add-chart-version), so that the documentation is built using the
  [version of the charts project that maps to](https://docs.gitlab.com/charts/installation/version_mappings.html)
  the GitLab release. This step may have been completed already.

- Between the 17th and the 20th of the month:

  1. [Create a stable branch and Docker image](#create-stable-branch-and-docker-image-for-release) for
     the new version.
  1. [Create a release merge request](#create-release-merge-request) for the new version, which
     updates the version dropdown menu for the current documentation and adds the release to the
     Docker configuration. For example, the
     [release merge request for 13.9](https://gitlab.com/gitlab-org/gitlab-docs/-/merge_requests/1555).

     Try to create the MR close to the cutoff for `gitlab` project's stable branch for the release.
     If the `gitlab-docs` MR is too early or late, a mismatch between the `gitlab` project's
     documentation files and the `gitlab-docs` global navigation can cause failed MR pipelines that
     must be manually fixed. To check the status of the `gitlab` release, go to the `#releases`
     Slack channel and look for the `This is the candidate commit to be released on the 22nd.`
     message.

  1. [Update the three online versions](#update-dropdown-for-online-versions), so that they display the new release on their
     version dropdown menus.

- On the 22nd of the month:

  [Merge the release merge requests and run the necessary Docker image builds](#merge-merge-requests-and-run-docker-image-builds).

### Add chart version

To add a new charts version for the release:

1. Make sure you're in the root path of the `gitlab-docs` repository.
1. Open `content/_data/chart_versions.yaml` and add the new stable branch version using the
   [version mapping](https://docs.gitlab.com/charts/installation/version_mappings.html). Only the
   `major.minor` version is needed.
1. Create a new merge request and merge it.

**Note:** If you have time, add anticipated future mappings to `content/_data/chart_versions.yaml`. This saves
a step for the next GitLab release.
{: .note}

### Create stable branch and Docker image for release

To create a stable branch of the `gitlab-docs` project and a Docker image for the release:

1. Make sure you're in the root path of the `gitlab-docs` repository.
1. Run the Rake task to create the single version. For example, to create the 13.9 release branch
   and perform other tasks:

   ```shell
   ./bin/rake "release:single[13.9]"
   ```

   A branch for the release is created, a new `Dockerfile.13.9` is created, and `.gitlab-ci.yml`
   has branches variables updated into a new branch. These files are automatically committed.

1. Push the newly created branch, but **don't create a merge request**. After you push, the
   `image:docs-single` job creates a new Docker image tagged with the name of the branch you created
   earlier. You can see the Docker image in the `registry` environment at
   <https://gitlab.com/gitlab-org/gitlab-docs/-/environments/folders/registry>.

For example, see [the 13.9 release pipeline](https://gitlab.com/gitlab-org/gitlab-docs/-/pipelines/260288747).

If the pipeline fails, the new Docker image is not created and so not added to the registry.

Optionally, you can test locally by:

1. Building the image and running it. For example, for GitLab 13.9 documentation:

   ```shell
   docker build -t docs:13.9 -f Dockerfile.13.9 .
   docker run -it --rm -p 4000:4000 docs:13.9
   ```

1. Visiting `http://localhost:4000/13.9` to see if everything works correctly.

### Create release merge request

**Note:** An [epic is open](https://gitlab.com/groups/gitlab-org/-/epics/4361) to automate this step.
{: .note}

To create the release merge request for the release:

1. Make sure you're in the root path of the `gitlab-docs` repository.
1. Create a branch `release-X-Y`. For example:

   ```shell
   git checkout main
   git checkout -b release-13-9
   ```

1. Edit `content/_data/versions.yaml` and update the lists of versions to reflect the new release:

   - Add the latest version to the `online:` section.
   - Move the oldest version in `online:` to the `offline:` section. There should now be three
     versions in `online:`.

1. Edit `Dockerfile.main` by removing the oldest version, and then adding the newest version to the top of the list.

1. Commit and push to create the merge request. For example:

   ```shell
   git add content/_data/versions.yaml Dockerfile.main
   git commit -m "Release 13.9"
   git push origin release-13-9
   ```

1. Create the merge request and choose the `Release` description
   template. Set the merge request to _Draft_ status and do not merge it yet.

### Update dropdown for online versions

To update `content/_data/versions.yaml` for all online versions (stable branches `X.Y` of the
`gitlab-docs` project). For example:

- The merge request to [update the 13.9 version dropdown menu for the 13.9 release](https://gitlab.com/gitlab-org/gitlab-docs/-/merge_requests/1556).
- The merge request to [update the 13.8 version dropdown menu for the 13.9 release](https://gitlab.com/gitlab-org/gitlab-docs/-/merge_requests/1557).
- The merge request to [update the 13.7 version dropdown menu for the 13.9 release](https://gitlab.com/gitlab-org/gitlab-docs/-/merge_requests/1558).

1. Run the Rake task that creates all of the necessary merge requests to update the dropdowns. For
   example, for the 13.9 release:

   ```shell
   git checkout release-13-9
   ./bin/rake release:dropdowns
   ```

1. [Visit the merge requests page](https://gitlab.com/gitlab-org/gitlab-docs/-/merge_requests?label_name%5B%5D=release)
   to check that their pipelines pass. Set each merge request to _draft_ status.

Do not merge these merge requests yet.

### Merge merge requests and run Docker image builds

The merge requests for the dropdowns should now all be merged into their respective stable branches.
Each merge triggers a new pipeline for each stable branch. Wait for the stable branch pipelines to
complete, then:

1. Check the [pipelines page](https://gitlab.com/gitlab-org/gitlab-docs/pipelines)
   and make sure all stable branches have green pipelines.
1. After all the pipelines succeed:
   1. Merge all of the [dropdown merge requests](#update-dropdown-for-online-versions).
   1. Merge the [release merge request](#create-release-merge-request).
1. Finally, run the
   [`Build docker images weekly` pipeline](https://gitlab.com/gitlab-org/gitlab-docs/pipeline_schedules)
   that builds the `:latest` Docker image.

1. Go to the [CI/CD Schedules pipelines tab](https://gitlab.com/gitlab-org/gitlab-docs/-/pipeline_schedules) and view the latest **Build docker images weekly** job. Run the **image:docs-latest** job.

As the last step in the scheduled pipeline, the documentation site deploys with all new versions.

### Post-deployment checklist

Verify the documentation site has been deployed as expected.  Open site `docs.gitlab.com` in a
browser and confirm both the latest version and the correct `pre-` version are listed in the
documentation version dropdown.

For example, if you released the 14.1 documentation, the first dropdown entry should be `GitLab.com (14.2-pre)`, followed by `14.1`.

## Labels

When working with issues or merge requests, the Technical Writing team uses
[labels](https://docs.gitlab.com/ee/user/project/labels.html) to describe those
issues' and merge requests' attributes (including the types of work being done).

The information about labels as described in this section supplements the
contents of the [Issues workflow](https://gitlab.com/gitlab-org/gitlab/blob/master/doc/development/contributing/issue_workflow.md)
page. To view a usage description of each of the labels in this section, see
[Labels](https://gitlab.com/groups/gitlab-org/-/labels?utf8=%E2%9C%93&subscribed=&search=docs%3A%3A)
in the GitLab interface.

### Usage

Any issue or merge request for which a Technical Writer provides a measurable
amount of work on (including content creation and reviews) _must_ include the
`Technical Writing` label.

After adding the `Technical Writing` label, we want to classify the type of
effort we're contributing to the issue or merge request by adding an additional
label from the following list:

- [`documentation`](https://gitlab.com/groups/gitlab-org/-/labels?utf8=%E2%9C%93&subscribed=&search=documentation):
  Use this label if files in the `/doc` directory were added, changed, or
  removed.
- [`UI text`](https://gitlab.com/groups/gitlab-org/-/labels?utf8=%E2%9C%93&subscribed=&search=ui+text)
- [`global nav item`](https://gitlab.com/groups/gitlab-org/-/labels?utf8=%E2%9C%93&subscribed=&search=global+nav+item)
- [`release post item`](https://gitlab.com/groups/gitlab-org/-/labels?utf8=%E2%9C%93&subscribed=&search=release+post+item)
- [`tw-style`](https://gitlab.com/groups/gitlab-org/-/labels?utf8=%E2%9C%93&subscribed=&search=tw-)
- [`tw-testing`](https://gitlab.com/groups/gitlab-org/-/labels?utf8=%E2%9C%93&subscribed=&search=tw-)
- [`development guidelines`](https://gitlab.com/gitlab-org/gitlab/-/labels?utf8=%E2%9C%93&subscribed=&search=development+guidelines):
  See the [Developer documentation](https://docs.gitlab.com/ee/development/#development-guidelines-review)
  for information about updating pages in the `/developer` directory.
- [`docs-technical-debt`](https://gitlab.com/groups/gitlab-org/-/labels?utf8=%E2%9C%93&subscribed=&search=docs-technical-debt)
- `handbook`

Depending on the issue or merge request, you may include one or more of the
preceding labels with the issue or merge request, depending on its contents.
There may be occasions when _none_ of the preceding labels apply to the issue
or merge request; in that case, having only the `Technical Writing` label is
enough.

### Documentation-specific type labels

If an issue/merge request has both the `Technical Writing` and `documentation`
labels, Technical Writers should add one of the following
[scoped labels](https://gitlab.com/groups/gitlab-org/-/labels?utf8=✓&subscribed=&search=docs%3A%3A)
to the issue/merge request on which they work:

- `docs::feature`
- `docs::fix`
- `docs::improvement`
- `docs::non-content`

### Workflow labels

To better communicate the status of what's being worked on by the
Technical Writing team, the Technical Writers use the
[following labels](https://gitlab.com/groups/gitlab-org/-/labels?utf8=✓&subscribed=&search=tw%3A%3A)
to describe issues' statuses:

- `tw::doing`
- `tw::finished`

Note that these are *team* workflow labels. The Technical Writer who is doing
writing work will usually be the person adding the `tw::doing` label, and the
Technical Writer doing the review will usually be changing it to the
`tw::finished` label (although external content submissions could have the
same Technical Writer using both the `tw::doing` and `tw::finished` labels as
part of their content review).

The labels are used as follows:

1. An issue or MR is marked with the `Technical Writing` label, as usual.
1. When a Technical Writer starts working on the issue/MR, they add the
   `tw::doing` label. In this case, *work* is everything that's required to
   finish the content, from creation through review. If a writer involved in
   the process stops working on the unfinished issue/MR, they remove the
   `tw::doing` label (at least at the point of one work week of inactivity).
   Whenever work is restarted, the `tw::doing` label is restored.
1. When work is complete on the issue/MR, a Technical Writer (normally the
   reviewer) adds the `tw::finished` label.
1. The issue/MR makes its way to Closed or Merged in the usual manner.

Note that the `tw::finished` label is for indicating when a Technical Writer
is done with an issue/MR for which we're not doing the merge or closing the
issue. If the Technical Writing team is doing the merging/closing, the issue/MR
status overrides the scoped `tw` label status, and there's no need to use the
`tw::finished` label.

If a Technical Writer is presented with an open issue or MR with a
`tw::finished` label that has more work required for it, the writer should
re-add the `tw::doing` scoped label to the issue/MR, and then continue with
the normal workflow process.

### Weights (proposed)

The Agile concept of _weight_ allows tracking of the effort that it takes to complete work. Although GitLab has a **Weight** field for issues, the Technical Writing team is responsible for work that happens in both issues and merge requests. Other teams might also want to track their effort using the **Weight** field, so scoped labels allow writers to track effort without using the **Weight** field.

The following scoped labels allow the Technical Writing team to track effort in both issues and merge requests:

| Label           | Comparable effort |
|-----------------|-------------------|
| `tw-weight::1`  | Fix a single misspelling or add missing punctuation. Smallest amount of Technical Writing effort. |
| `tw-weight::3`  | Develop or revise a few sentences. |
| `tw-weight::5`  | Develop or revise a section of content. More than a paragraph, less than a page. |
| `tw-weight::8`  | Revise up to a full page with content provided to you, or develop approximately a half page from scratch. |
| `tw-weight::13` | Create an entirely new page for a feature or process, with no content provided in advance. Largest amount of technical writing effort. Split larger items into one or more issues or MRs.|

These labels are being tested by the team, and are not being used by all technical writers.

The technical writers using these labels assign a `tw-weight` label to any issue or MR on which they work, based on the amount of effort to complete the task (which includes reviews). "Comparable effort" above provides some amount of consistency of the weights. However, each technical writer gauges their own level of effort. For example, if two technical writers were given a merge request to complete, one of them might rate their effort as 3 points, while the other might rate it as 8 points of effort, perhaps due to their unfamiliarity with the topic.

Because weights are based on each technical writers' assessment, they are not and will not be used for direct comparisons between technical writers. Weights can be used, however, to ensure individual technical writers have healthy workloads, and represent a mechanism that can indicate when they're getting overloaded with work.

Weights should not include time or effort associated with creating the issue or MR, or when dealing with pipeline or platform issues. For example, dealing with unforeseen build issues shouldn't be a factor in sizing, and wouldn't increase a 3 to a 5.

The first technical writer that works on the task (either as a reviewer of developer-created content, or as a developer of content) logs their effort with a `tw-weight` label. The label isn't used to track the efforts of secondary technical writer reviewers.
