---
layout: default
title: "Sprint Backlog"
description: "AquaLink's documented initial sprint goals, evidence and dependencies"
permalink: /agile/sprint-backlog/
---

[← Agile hub]({{ '/agile/' | relative_url }})

## 1. What a sprint backlog shows

A sprint backlog takes selected work from the larger product backlog and gives the development team a short-term goal and a practical plan. The sprint backlog should make the tasks, current progress, ownership, dependencies and remaining work visible.

For AquaLink, Faith's portfolio identifies four initial iterations across July and early August 2026. These dates and goals are **team-reported** and were not cross-checked against the complete live Trello history.

## 2. Original sprint-backlog evidence

![AquaLink sprint backlog, screenshot 1](https://raw.githubusercontent.com/MologadiD/Portfolio/main/assets/img/sprint-backlog-1.png)

*Shared artefact: [Mologadi's sprint-backlog screenshot 1](https://github.com/MologadiD/Portfolio/blob/main/assets/img/sprint-backlog-1.png).*

![AquaLink sprint backlog, screenshot 2](https://raw.githubusercontent.com/MologadiD/Portfolio/main/assets/img/sprint-backlog-2.png)

*Shared artefact: [Mologadi's sprint-backlog screenshot 2](https://github.com/MologadiD/Portfolio/blob/main/assets/img/sprint-backlog-2.png).*

## 3. Initial sprint chronology

| Sprint | Dates in teammate's record | Reported sprint goal | Original sprint taskboard |
|---|---|---|---|
| **1** | 14–17 July 2026 | Investigate water-access problems, stakeholders, service requirements and project scope | [Sprint 1 image](https://github.com/FaithA965/FaithA965.github.io/blob/main/Taskboard_Sprint1.png) |
| **2** | 21–24 July 2026 | Define database entities, attributes, relationships and ERD | [Sprint 2 image](https://github.com/FaithA965/FaithA965.github.io/blob/main/Taskboard_Sprint2.png) |
| **3** | 28–30 July 2026 | Establish consistent styling, shared components and responsive layout | [Sprint 3 image](https://github.com/FaithA965/FaithA965.github.io/blob/main/Taskboard_Sprint3.png) |
| **4** | 4–7 August 2026 | Review architecture, ERD, entities, relationships and proposed changes | [Sprint 4 image](https://github.com/FaithA965/FaithA965.github.io/blob/main/Taskboard_Sprint4.png) |

*Source: [Faith's AquaLink sprint backlog](https://github.com/FaithA965/FaithA965.github.io/blob/main/agile.md#4-sprint-backlog).*

## 4. Relationship between the sprints

**Sprint 1: Understand the problem.** The research sprint aimed to identify what residents and suppliers needed, rather than immediately designing software around an assumed solution.

**Sprint 2: Represent the domain.** The database sprint considered the entities and relationships needed by the planned platform: households, boreholes, suppliers, service plans, payments, tanks, alerts and related information. This is particularly relevant to the allocated backend role.

**Sprint 3: Create a common visual language.** The team worked on shared styling and interface components. This was primarily a user-interface workstream; it should not be recorded as backend implementation.

**Sprint 4: Revisit the technical design.** The team reviewed the architecture and ERD against the requirements. Faith's log describes items being reviewed and the final team approval still being prepared by 7 August, so this portfolio **does not claim final approval was already obtained**.

## 5. Tracking planned versus completed work

A task listed under a sprint is a commitment or planned activity; its presence in a screenshot is not necessarily proof it was completed. Each task should eventually be traced to a status, responsible member and evidence of output. The [live project board](https://trello.com/b/5lxVBUSK/aqualink) is the preferred source for those details.

For backend work in Sprint 2 or 4, useful evidence would be an ERD revision, schema commit, design decision, issue, test or API contract. None is claimed as personally completed until it can be verified.

## 6. Personal reflection (STAR) — draft for review

<a id="personal-reflection"></a>

**Situation.** AquaLink's work had to move from understanding the community problem to defining technical requirements. The team divided the early work into short iterations so that each workstream would feed the next.

**Task.** In my Backend Developer role, the database-design and technical-review sprints were especially relevant. Their goals concerned the information model and system behaviours that planned backend functionality would depend on.

**Action.** The documented sprint structure separated research, data modelling, interface consistency and technical review. This sequence illustrates the importance of understanding dependencies before implementation. For example, a backend design decision about the relationship between a household and service plan needs to be consistent with what the product team intends to offer and what the UI will eventually display.

**Result and learning.** The chronology shows an organised progression through discovery, technical modelling and review, but the published screenshots alone do not establish the status of every individual assignment. My strongest takeaway is that sprint planning should balance ambition with the information actually available: unclear requirements and unresolved dependencies should be surfaced as work in their own right.

> **Personal check before submission:** Add the tasks you personally worked on, the dates of your own updates, the outcome, and any blocker you genuinely encountered. The above is a reflection draft on the shared process, not an invented personal sprint diary.

## References

- [Faith Adams — Sprint Backlog](https://github.com/FaithA965/FaithA965.github.io/blob/main/agile.md#4-sprint-backlog)
- [Mologadi Dikgale — Backlog screenshots](https://github.com/MologadiD/Portfolio/tree/main/assets/img)
- [AquaLink Trello Board](https://trello.com/b/5lxVBUSK/aqualink)
