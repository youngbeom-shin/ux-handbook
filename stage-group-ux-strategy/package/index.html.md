---
layout: markdown_page
title: "UX Vision: Package"
description: "The Package UX team supports anyone who uses GitLab to build, test, and deploy software or would like to use a variety of package and/or image registries to manage dependencies"
---


## Overview
The Package group works on the part of GitLab concerning the [Package stage](/handbook/product/categories/#package-stage), which integrates with GitLab's [CI/CD product](https://about.gitlab.com/direction/ops/). Our mission is to create a secure environment where both source code and dependencies can live by allowing you to publish, consume, and discover packages of a large variety of languages and platforms all in one place.

Package design prioritizes deliveirng value to our users as effectively as possible. While design is an adaptive counterpart to the team, the design process tends to fall into one of two categories:
1. **Large scale vision** - This design process is designed to create a large-scale vision and validate the direction with our users. From there, an epic is often created and broken down into small MVC iterations in coordination with the broader team.
1. **Small scale design** - This design process focuses more on meeting the immediate need of the team, delivering solutions to edge cases, refining validated experiences, etc. At the highest level, the design focuses on three broad areas:

    1.  Providing a seamless experience geared towards storing and accessing packages and container images for safer more reliable builds
    1.  Establishing a transparent, performant supply chain of dependencies to ensure everyone can contribute.
    1.  Building tools around security policies and vulnerability remediation all while limiting exposure to known vulnerabilities

### Our customer
Our customer is anyone who uses GitLab to build, test, and deploy software or would like to leverage a variety of package and/or image registries to manage their dependencies. This sort of customer can be in any size or specific industry. A different customer is a large organization that utilizes several programming languages across teams and they would like to centralize all of their external dependencies in one location, GitLab.

### Our user
We consider several different types of users in our experience design effort. Even when a user has the same title, their responsibilities may vary by organization size, department, org structure, and role. Below are some of the personas we serve:

* [Systems administrators](/handbook/marketing/strategic-marketing/roles-personas/#sidney-systems-administrator)
* [Software developers](/handbook/marketing/strategic-marketing/roles-personas/#sasha-software-developer)
* [Devops engineers](/handbook/marketing/strategic-marketing/roles-personas/#devon-devops-engineer)
* [Security analysts](/handbook/marketing/strategic-marketing/roles-personas/#sam-security-analyst) (future)

### Our team
Our team continues to grow. We currently have 2 members that contribute to Package UX efforts:

* [Rayana Verissimo](https://gitlab.com/rayana) - Product Design Manager
* TBD - Product Designer, Package

#### Our team meetings
Following in GitLab's tradition of async over sync, a majority of our communication is done through issues and merge requests. We do have a few regular synchronous meetings:

* Product Management and Design meet weekly to coordinate design efforts for Package.
* Front-end and Design meet weekly to coordinate UI improvement efforts.
* Designers around CI/CD meet every other week to coordinate efforts accross the platform.

### SSOT Design Files
In order to improve transparency, Package UX has created single sources of truth (SSOT) for the product categories included inside of the Package Group. Not all of the categories have corelating SSOT Figma Files.

| Category | SSOT Design File | Epic |
|---|---| --- |
| [Package Registry](https://about.gitlab.com/direction/package/#package-registry) | [Figma File](https://www.figma.com/file/AnBWA0HLLLRWUK6c8oePzv/Package-Registry-SSOT?node-id=1%3A1) | [&3693](https://gitlab.com/groups/gitlab-org/-/epics/3693) |
| [Container Registry](https://about.gitlab.com/direction/package/#container-registry) | [Figma File](https://www.figma.com/file/kZh5V0YEHoKqZZdqIPF92I/Container-Registry-SSOT?node-id=0%3A1) | [&2899](https://gitlab.com/groups/gitlab-org/-/epics/2899) |
| [Dependency Proxy](https://about.gitlab.com/direction/package/#dependency-proxy) | [Figma File](https://www.figma.com/file/5LlIZjcgDe9QNNRK2vZEyc/Dependency-Proxy-SSOT?node-id=0%3A1) | [&2920](https://gitlab.com/groups/gitlab-org/-/epics/2920) |
| [Dependency Firewall](https://about.gitlab.com/direction/package/#dependency-firewall) | tbd | [&5133](https://gitlab.com/groups/gitlab-org/-/epics/5133) |
| [Help Chart Registry](https://about.gitlab.com/direction/package/#helm-chart-registry) | tbd | [&2281](https://gitlab.com/groups/gitlab-org/-/epics/2281) |
| [Release Evidence](https://about.gitlab.com/direction/package/#release-evidence) | tbd | [&5135](https://gitlab.com/groups/gitlab-org/-/epics/5135) |
