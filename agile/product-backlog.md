---
layout: default
title: "Product Backlog"
description: "AquaLink's product scope, planned capabilities, priorities and change management"
permalink: /agile/product-backlog/
---

[← Agile hub]({{ '/agile/' | relative_url }})

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

## 5. Personal reflection (STAR) — draft for review

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
