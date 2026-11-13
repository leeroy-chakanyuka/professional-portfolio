---
layout: default
title: "Product Backlog"
description: "AquaLink's product scope, planned capabilities, priorities and change management"
permalink: /agile/product-backlog/
---

## 1. Purpose and original evidence

The product backlog contains everything the project team knows may be needed to provide value. Unlike a sprint backlog, it is not limited to the current iteration. Backlog items may be clarified, reprioritised, divided into smaller tasks or deferred as the team learns more.

AquaLink's Trello board is the [shared source of live backlog information](https://trello.com/b/5lxVBUSK/aqualink). The screenshots below are independently available in the project manager's portfolio, providing evidence without requiring access to private Trello card details.

![AquaLink product backlog, first screenshot](https://raw.githubusercontent.com/MologadiD/Portfolio/main/assets/img/product-backlog-1.png)

*Shared artefact: [Product backlog image 1](https://github.com/MologadiD/Portfolio/blob/main/assets/img/product-backlog-1.png), published by Mologadi Dikgale.*

![AquaLink product backlog, second screenshot](https://raw.githubusercontent.com/MologadiD/Portfolio/main/assets/img/product-backlog-2.png)

*Shared artefact: [Product backlog image 2](https://github.com/MologadiD/Portfolio/blob/main/assets/img/product-backlog-2.png), published by Mologadi Dikgale.*

## 2. What the documented product backlog covered

The following workstreams were reported in [Faith's AquaLink product backlog overview](https://github.com/FaithA965/FaithA965.github.io/blob/main/agile.md#3-product-backlog).

| Backlog area | Items or decisions appearing in the published project history | Reason for prioritisation |
|---|---|---|
| Community research | Understand local water-access problems, household needs and supply constraints | Product scope needed a clear real-world problem |
| Project setup | Define the team, repository, development setup and working practices | Establish a foundation for collaboration |
| Business modelling | Research the service concept, feasibility and minimum viable scope | Avoid designing features without an operating model |
| Database design | Identify households, suppliers, boreholes, plans, payments, usage and alerts; define relationships and ERD | The data model supports several other components |
| Shared interface | Wireframes, design standards, typography and responsive components | Users need a consistent way to access planned functions |
| Technical design review | Review architecture, ERD, attributes and relationships | Identify issues before committing to implementation |
| Planned platform functionality | Household portal, supplier dashboard, administrator tools, subscriptions, payment and usage information | Provides the intended service functionality |

**Important distinction:** this table is a categorised description of the team backlog, **not** a verbatim prioritised list of live Trello cards. Specific priorities, owners and statuses still need the authoritative board records.

## 3. Connecting the backlog to backend responsibilities

My recorded project role was **Backend Developer**, with planned responsibility for REST APIs, database design and business logic. The data-model workstream is particularly relevant because household/supplier records and relationships influence the eventual API contract, interface requirements and test cases.

For example, a requirement to display the water usage of a household is not independent of the household/account model. It raises questions about how usage is attributed, which service plan applies, how the account is identified and which user should be authorised to see it. Clarifying such dependencies before development reduces the risk of having to redesign an endpoint when the business rules are later agreed.

This is an **analysis of the planning material**, not an assertion that the final endpoints were implemented.

## 4. Refinement and change management

The team narrative describes a shift from a delivery-oriented idea to a permanent network supported by software. This would naturally affect the requirements and the ordering of planned work. Rather than silently rewriting the scope, the backlog should make additions and changed priorities visible to the team.

The [four documented sprint taskboards](https://github.com/FaithA965/FaithA965.github.io/blob/main/agile.md#4-sprint-backlog) provide a way to trace the progression from research to a database model, common interface styling and technical design review.

## 5. Later prioritised backlog from the original logbook

The later AquaLink logbook contains an explicitly prioritised **remaining-work** board. Unlike the earlier conceptual category list, these entries include P1/P2 priority levels. The table is a sourced summary of **team-reported open work**, not a claim that I personally assigned each priority.

| Priority | Recorded backlog item | Delivery implication |
|---|---|---|
| P1 | Real database integration | Persistent workflows and create/read/update/delete verification |
| P1 | Payment integration | Provider setup and real end-to-end transaction verification |
| P1 | IoT and hardware integration | Connect physical readings or clearly label simulations |
| P1 | Final documentation and submission | Setup, architecture, limitations and testing evidence |
| P1 | Demonstration preparation | Stable walkthrough and rehearsed flows |
| P1 | Live presentation | Explain concept, architecture, implementation and boundaries |
| P2 | Mobile application | Defer beyond the immediate presentation scope |

*Primary source: [Tony's Product Backlog portfolio](https://github.com/TonyBaloyi/Portfolio/blob/main/product-backlog.md), referencing the [original Agile Logbook](https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/documents/AquaLink_Agile_Logbook.docx).*

## 6. What the team record called complete

The published taskboard records completed **interface and planning work**, including the database schema design, shared styles and logic, navigation, an administrator dashboard, household pages, plans, purchase screens, supplier tank pages, refill history and alerts. It also records screen-level testing, bug fixing and responsive/browser reviews.

A completed **schema design** is not a completed **database integration**. Similarly, an implemented purchase screen is not necessarily a real payment system, and a tank overview is not proof of live IoT sensing.

This distinction matters to backend reporting. There should be separate backlog items for the screen, the data contract, persistence, authorisation and integration verification. Otherwise, a visually complete feature can mask unresolved work.

## 7. How prioritisation changed during finalisation

| Date in the later logbook | Reported activity | Implication for the backlog |
|---|---|---|
| 29 July 2026 | Plans, purchases, tank information, refills and alerts organised | Grouped feature requirements |
| 7 August 2026 | UI feedback mapped to remaining screens | Linked design review to implementation priorities |
| 5 October 2026 | Completed application reviewed against user stories | Exposed implementation versus integration gaps |
| 22 October 2026 | Remaining work and task ownership reviewed | Separated delivered and outstanding tasks |
| 29 October 2026 | Roadmap revisited before presentation | Documentation and stability became immediate priorities |

The larger project vision remained relevant, but the approaching presentation required a different ordering from an open-ended production roadmap.

## 8. Backend dependency ordering — my evaluation

The following is my proposed order **for backend planning**, not a reconstructed historical task assignment.

1. Agree the household, supplier, plan and transaction model.
2. Define role boundaries and API contracts against user stories.
3. Implement and test persistence and input validation.
4. Verify end-to-end workflows with the UI, using a controlled test dataset.
5. Integrate external providers only when credentials, environments and test evidence are available.
6. Keep simulated sensor and payment states explicitly labelled until verified.

The logic behind this order is dependency reduction: a payment or monitoring screen can be demonstrated early, but a reliable underlying service requires stable data relationships and verifiable integration points.

## 9. Personal reflection (STAR) — draft for review

<a id="personal-reflection"></a>

**Situation.** AquaLink had several interconnected parts: identifying community needs, shaping the service model, designing a data structure, developing interfaces and considering the physical supply infrastructure. Without a common backlog, the team could lose sight of how the work fitted together.

**Task.** My assigned backend role required attention to work items involving data relationships, APIs and business rules. Those tasks depended on the priorities and assumptions established by the wider team.

**Action.** The shared backlog structure made it possible to group project requirements and separate earlier discovery work from later technical work. For the backend, the most significant ordering question is whether the entities, relationships and business rules have been clarified before API implementation begins. The changes to AquaLink's overall approach also underline the importance of keeping the backlog current instead of treating the first proposal as final.

**Result and learning.** The project record establishes a clear sequence of requirements, data design and technical review. My takeaway is that backlog refinement is about controlling uncertainty: identify dependencies, establish value and make the scope of each item small enough to verify. In future I would raise backend dependencies explicitly when items are prioritised and ensure that completion means more than simply drafting a feature.

> **Personal check before submission:** Confirm specific backlog cards assigned to you, along with actual priorities and completion evidence. This reflection does not claim you managed the entire backlog or built every proposed feature.

## Sources

- [AquaLink original Trello board](https://trello.com/b/5lxVBUSK/aqualink)
- [Faith Adams: AquaLink product backlog](https://github.com/FaithA965/FaithA965.github.io/blob/main/agile.md#3-product-backlog)
- [Mologadi Dikgale: original backlog screenshots](https://github.com/MologadiD/Portfolio/tree/main/assets/img)

## 10. Delivery dependencies: a backend reading of the backlog

The later backlog separates completed user-facing screens from three critical unresolved integration areas. This distinction changes the technical definition of progress.

| User-facing capability | Backend dependency | Evidence needed before claiming end-to-end completion |
|---|---|---|
| Household details | Durable household records and authorisation | CRUD tests and a role-restricted read |
| Plans and purchases | Plan model, transaction state and payment integration | A recorded sandbox transaction and error-path test |
| Supplier tank view | Tank identity, reading schema and timestamp handling | Verified ingest or clearly marked simulated sample |
| Admin overview | Accurate aggregation across household and supplier data | A repeatable test dataset and reconciliation |
| Alerts and refill history | Event persistence, business rules and auditability | Test cases for state transitions and historical records |

This is a proposed verification matrix based on the project's requirements; it is **not** evidence that these checks were completed.

## 11. Backlog decisions I would document next time

The logbook records the team revisiting remaining work as the presentation approached. As a backend developer, I would make the reasoning behind such decisions more visible:

1. Identify whether a work item is a demonstration screen, a business workflow or an external integration.
2. Assign a named owner, priority, acceptance criteria and blocking dependency.
3. Keep schema design, implemented persistence and integration testing as separate status checkpoints.
4. Record why mobile work remains future scope while the demonstrable application takes priority.
5. Link each completed task to a test, commit or screenshot that actually substantiates the particular claim.

## 12. Final reflection on prioritisation

AquaLink's backlog illustrates how easy it is to confuse breadth of features with depth of delivery. The team could show dashboards, purchase screens and sensor-oriented interfaces while the original records still identified persistent database, live payment and physical IoT connections as separate work. That is a useful engineering distinction, not a failure to hide.

My learning is that backlog prioritisation should protect the integrity of the system underneath the screens. I would argue for explicitly scheduling model design, validation and persistence work before relying on user-facing flows for a production claim, while keeping a demonstration's limits visible and honest.

The shared backlog entries and screenshots are team evidence. My individual contribution to a specific card must be supported by my own task history before being presented as an accomplished personal deliverable.

[Compare the later team backlog](https://github.com/TonyBaloyi/Portfolio/blob/main/product-backlog.md) · [Review the evidence register]({{ '/agile/evidence-register/' | relative_url }})


## Shared backlog artefacts and evidence

The original team planning screenshots are retained as the most direct examples of backlog documentation. They do not, by themselves, prove individual coding or completion.

<div class="evidence-mosaic">
<figure class="archive-item"><a href="https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/trello/trello-01.jpg"><img loading="lazy" src="https://raw.githubusercontent.com/TonyBaloyi/Portfolio/main/evidence/trello/trello-01.jpg" alt="Trello backlog screenshot 01"></a><figcaption><a href="https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/trello/trello-01.jpg">Original backlog image 01</a></figcaption></figure>
<figure class="archive-item"><a href="https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/trello/trello-02.jpg"><img loading="lazy" src="https://raw.githubusercontent.com/TonyBaloyi/Portfolio/main/evidence/trello/trello-02.jpg" alt="Trello backlog screenshot 02"></a><figcaption><a href="https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/trello/trello-02.jpg">Original backlog image 02</a></figcaption></figure>
<figure class="archive-item"><a href="https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/trello/trello-03.jpg"><img loading="lazy" src="https://raw.githubusercontent.com/TonyBaloyi/Portfolio/main/evidence/trello/trello-03.jpg" alt="Trello backlog screenshot 03"></a><figcaption><a href="https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/trello/trello-03.jpg">Original backlog image 03</a></figcaption></figure>
</div>

The later logbook's P1/P2 list should be interpreted as **remaining work near delivery**, not as an unchanged backlog covering every month. As deadlines approached, documentation, demonstration stability and accurate statements about integration became high priorities.

**Source:** [Tony's dated original Agile Logbook](https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/documents/AquaLink_Agile_Logbook.docx) and [later backlog chapter](https://github.com/TonyBaloyi/Portfolio/blob/main/product-backlog.md).

[Continue to Sprint Backlog]({{ '/agile/sprint-backlog/' | relative_url }})
