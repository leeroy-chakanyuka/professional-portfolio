---
layout: default
title: "Sprint Backlog"
description: "AquaLink's documented initial sprint goals, evidence and dependencies"
permalink: /agile/sprint-backlog/
---

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

## 6. Extended project timeline from the later team logbook

Faith's four early sprint boards cover July and early August. Tony's [later dated logbook](https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/documents/AquaLink_Agile_Logbook.docx) covers the wider implementation cycle. The phases below summarise its dated workstreams; they **do not** claim to be the exact numbering of the logbook's referenced eleven-sprint roadmap.

| Period | Team-reported workstream | Important delivery boundary |
|---|---|---|
| 27–31 July | Requirements and user stories | Acceptance criteria and scope |
| 3–7 August | Visual foundations and shared components | Consistency across screens |
| 10–14 August | Architecture and data requirements | Entities and integration assumptions |
| 17–21 August | Administrator implementation | Dashboard and household/plan views |
| 24–28 August | Supplier operations | Tanks, refills and alerts |
| 31 August–4 September | Shared component logic | Navigation, styles and page consistency |
| 7–11 September | Integration of screen flows | Cross-page navigation |
| 14–18 September | Application review | Implementation against requirements |
| 21–25 September | Quality activities | Admin/Supplier screen tests |
| 28 September–2 October | Regression and responsiveness | Browser and layout checks |
| 5–9 October | Integration boundaries | UI completion versus services outstanding |
| 12–16 October | Documentation | Architecture and business model |
| 19–23 October | Demo preparation | Outstanding tasks and walkthrough |
| 26–29 October | Final review | Reprioritisation and readiness |

*Source: [Tony's Sprint Backlog portfolio](https://github.com/TonyBaloyi/Portfolio/blob/main/sprint-backlog.md), summarising the team logbook.*

## 7. Planned, completed and blocked are different states

A useful sprint review should distinguish four claims: **selected work**, **work started**, **work completed** and **work independently verified**. The logbook shows reported interface delivery and review activities while also identifying outstanding database, payment and sensor connections.

The last category matters most for technical reporting. For backend tasks, I would expect to see relevant commits, an executable test or a demonstration of data persistence before marking an end-to-end service complete.

## 8. The practical meaning of a sprint dependency

<div class="mini-grid"><div><h3>Data-first work</h3><p>A household detail screen needs a data contract. The domain model and permission rules should be agreed before treating its backing service as ready.</p></div><div><h3>External integration</h3><p>A purchase screen can be displayed without payment-provider access. A testable payment integration requires an environment, credentials and evidence of outcomes.</p></div></div>

This distinction is a lesson from the published team's delivery record, not a claim that I personally implemented either workflow.

## 9. What I would add to sprint reporting

| Field | Reason to capture it |
|---|---|
| Story / task ID | Link sprint work to the product backlog |
| Owner and reviewer | Clarify responsibility and verification |
| Dependency | Explain blockers before missed commitments |
| Acceptance criterion | Decide what completion means |
| Commit / test / artefact | Give assessors observable evidence |
| Follow-up | Record what still needs to be finished |

## 10. Personal reflection (STAR) — draft for review

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
