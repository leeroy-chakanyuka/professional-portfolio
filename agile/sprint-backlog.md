---
layout: default
title: "Sprint Backlog"
description: "Sprint planning, workstreams, dependencies, original records and backend learning"
permalink: /agile/sprint-backlog/
---

<p class="chapter-intro">A sprint backlog represents work selected for an iteration, how it will be approached and why it is achievable. Delivery must still be supported by evidence.</p>

This chapter follows the team's longer project record through October, while also crediting Faith's earlier July–August sprint taskboards. Those records overlap, and neither should be mistaken for my personal diary.

## 01. Understanding our sprint planning

The team's scope included requirements, architecture, Admin and Supplier screens, shared logic, quality checks and final preparation. Sprint planning was useful because it converted a broad concept into shorter sets of tasks.

### Planned work is different from completed work

In the logbook, *completed*, *planned* and *impeded* are separate categories. A sprint backlog should preserve these distinctions. A feature appearing in a sprint does not establish it was implemented, integrated or tested.

## 02. Our documented development timeline

| Recorded period | Workstream | Shared activities |
|---|---|---|
| 27–31 July | Requirements | Stories, scope, navigation and acceptance criteria |
| 3–7 August | UI/UX foundations | Shared styling, screen design and components |
| 10–14 August | Architecture and data | Entities, database design and dependencies |
| 17–21 August | Administrator implementation | Dashboard, households, plans and purchases |
| 24–28 August | Supplier operations | Tank screens, refills and alerts |
| 31 August–4 September | Shared components | Styling, common logic and navigation |
| 7–11 September | Screen integration | Page consistency and navigation |
| 14–18 September | Application review | Comparison of screens to requirements |
| 21–25 September | Quality checks | Admin and Supplier screen testing |
| 28 September–2 October | Quality improvement | Bug fixes, responsive and browser testing |
| 5–9 October | Integration boundaries | Review of completed interfaces and remaining services |
| 12–16 October | Documentation | Business, architecture and supporting records |
| 19–23 October | Presentation preparation | Demo sequence and outstanding-task review |
| 26–29 October | Final review | Reprioritisation and readiness |

**Source:** [Tony's July–October dated Agile Logbook](https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/documents/AquaLink_Agile_Logbook.docx). Faith's earlier record separately documents [Sprint 1](https://github.com/FaithA965/FaithA965.github.io/blob/main/Taskboard_Sprint1.png), [Sprint 2](https://github.com/FaithA965/FaithA965.github.io/blob/main/Taskboard_Sprint2.png), [Sprint 3](https://github.com/FaithA965/FaithA965.github.io/blob/main/Taskboard_Sprint3.png) and [Sprint 4](https://github.com/FaithA965/FaithA965.github.io/blob/main/Taskboard_Sprint4.png).

## 03. Planned work and impediments

### Example A: Requirements planning

At the start of the project, the challenge was to settle user needs and the water-service model. Unresolved scope affects every later technical workstream, especially data ownership and transactions.

### Example B: Interface implementation

Admin and Supplier screens were developed in the later recorded iterations. Shared design components and navigation became dependencies: a change in one common element could affect many pages.

### Example C: Responsive and regression testing

The published logbook reports screen-level review and responsive checks. These activities demonstrate quality attention, but they should not be used as proof of unrecorded API, payment or IoT integration tests.

### Example D: Final reprioritisation

As the November presentation approached, the reported priorities shifted towards documentation, stable demonstration routes and explaining outstanding integrations. That was an adaptation to time and scope.

## 04. Connecting sprint work to deliverables

| Area | Team-reported output | Boundary to retain |
|---|---|---|
| Requirements | Stories and criteria recorded | Not all proposed stories equal deployed services |
| Architecture | Schema design and review | Schema design is not live persistence |
| Shared UI | Layouts, navigation and reusable logic | Does not prove server integration |
| Admin screens | Household, plan, dashboard and purchase views | Purchase interface is not verified payment processing |
| Supplier screens | Tank, refill and alert views | Sensor display is not live hardware integration |
| Quality | Screen and browser testing reported | API and end-to-end evidence should be separate |
| Database | Integration appeared in remaining work | Avoid claiming complete CRUD without proof |
| Payments | Real provider connection appeared in remaining work | Verify test transaction before claiming completion |
| IoT | Physical sensors appeared in remaining work | Label simulated readings honestly |

## 05. How dependencies affected iteration work

### Interface dependencies

Navigation and shared styles enabled a consistent user experience but also required regression checks as pages were added.

### Backend dependencies

A household record, plan or tank view depends on well-defined entities, relationships and access rules. From my assigned role, this is the point where clear technical contracts are essential.

### External dependencies

Payment gateways and sensors introduce credentials, test environments and hardware availability beyond ordinary page development. They should have their own risk and acceptance criteria.

## 06. Original Trello sprint evidence

<div class="evidence-mosaic">
<figure class="archive-item"><a href="https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/trello/trello-05.jpg"><img loading="lazy" src="https://raw.githubusercontent.com/TonyBaloyi/Portfolio/main/evidence/trello/trello-05.jpg" alt="AquaLink Trello sprint evidence 05"></a><figcaption><a href="https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/trello/trello-05.jpg">Sprint screenshot 05</a></figcaption></figure>
<figure class="archive-item"><a href="https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/trello/trello-06.jpg"><img loading="lazy" src="https://raw.githubusercontent.com/TonyBaloyi/Portfolio/main/evidence/trello/trello-06.jpg" alt="AquaLink Trello sprint evidence 06"></a><figcaption><a href="https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/trello/trello-06.jpg">Sprint screenshot 06</a></figcaption></figure>
<figure class="archive-item"><a href="https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/trello/trello-07.jpg"><img loading="lazy" src="https://raw.githubusercontent.com/TonyBaloyi/Portfolio/main/evidence/trello/trello-07.jpg" alt="AquaLink Trello sprint evidence 07"></a><figcaption><a href="https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/trello/trello-07.jpg">Sprint screenshot 07</a></figcaption></figure>
</div>

These images are reproduced by linking to [Tony's original evidence files](https://github.com/TonyBaloyi/Portfolio/tree/main/evidence/trello). They remain attributed **shared team evidence**, not individual authorship claims.

## 07. My assigned workstream

The team charter lists me as Backend Developer, associated with REST APIs, relational schema and business rules. That assignment helps explain which sprint dependencies mattered most to me: data relationships must be consistent before multiple screens rely on them, and persistence tests must distinguish a working service from demonstration data.

I am not asserting that every endpoint or integration was completed by me; that requires my own issue and commit history.

## 08. Reflection: capacity and adaptation

A sprint plan creates focus, but cannot eliminate uncertainty. AquaLink's evolution shows that discovery work can change implementation assumptions and that several features may depend on the same unresolved decision.

### The importance of reviewing progress

What I would carry forward is the habit of checking the definition of done at the end of each iteration. If the UI is present but its backend dependency remains open, the review should make that difference visible. Otherwise the team can underestimate remaining work at precisely the point when delivery becomes most time-sensitive.

## 09. Improvements I would make

1. Estimate the work the team can actually verify within a sprint.
2. Record each task's owner, expected output and dependencies.
3. Give screen implementation and real integration different acceptance conditions.
4. Review blockers during the sprint, not only at the end.
5. Reserve time for tests, documentation and regression checks.
6. Preserve a dated decision log whenever scope or priorities change.
7. Keep the individual contribution record separate from team status updates.

## 10. Connection to Agile practice

The Scrum Guide frames the Sprint Backlog as a plan by and for the Developers, including the Sprint Goal, selected backlog items and a plan for delivering them. AquaLink illustrates why the plan should be regularly inspected and adapted as new information arises.

**Reference:** Schwaber, K. and Sutherland, J. (2020), [The Scrum Guide](https://scrumguides.org/scrum-guide.html).

## 11. Final reflection

My main lesson is that an iterative plan is only useful when it gives the team an accurate view of reality. The shared record shows substantial progression in requirements and screens while distinguishing unresolved integrations. As a backend developer, I would make technical dependencies and verification visible earlier, so the final demonstration represents the system faithfully.

[← Product Backlog]({{ '/agile/product-backlog/' | relative_url }}) · [Agile Logbook →]({{ '/agile/agile-logbook/' | relative_url }})
