---
layout: default
title: "User Stories & Tasks"
description: "Requirements, acceptance criteria, implementation tasks and my backend-oriented learning"
permalink: /agile/user-stories/
---

<p class="chapter-intro">User needs become useful software only when they are translated into clear work, with a way to verify what has actually been delivered.</p>

AquaLink explored water distribution and management for households, suppliers and administrators. This chapter follows the same **eleven-part evidence and reflection structure** as the team's later portfolio documentation, but it is written from my assigned backend-development perspective. The user stories and screenshots are **shared project records**, not evidence that I individually implemented every feature.

## 01. Understanding AquaLink's users

### Administrator

An administrator needs oversight of household records, plans, purchases and operational information. A dashboard can make those areas accessible, but it is only trustworthy if the data is consistent and the viewer has the appropriate permissions.

### Supplier

A supplier needs to view tanks, refill activities, infrastructure status and alerts. This implies that the system must reliably associate a tank with its supplier, readings and time-based events.

### Households

A household needs understandable information about its service connection, plan, consumption and payments. For a backend developer, these needs lead to questions about identity, subscriptions, transactions and privacy.

The proposed functionality should not be mistaken for verified production deployment. The [original project story]({{ '/agile/our-story/' | relative_url }}) explains how AquaLink's scope evolved.

## 02. Evidence of requirements analysis

Tony's dated logbook records requirements clarification in late July 2026. The following is a **summary of team activities**, not my personal attendance register.

| Date | Shared activity recorded | Why it mattered |
|---|---|---|
| 27 July 2026 | Scope and user stories were reviewed | Established initial Admin and Supplier needs |
| 28 July 2026 | Supplier and household requirements were discussed | Exposed relationships between users and records |
| 29 July 2026 | Plans, purchases, tanks, refills and alerts were grouped | Created a connection between requirements and backlog items |
| 30 July 2026 | Role-specific navigation was considered | Clarified what each user should be able to access |
| 31 July 2026 | Story scope and priorities were consolidated | Prepared subsequent technical work |

**Primary source:** [AquaLink Agile Logbook](https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/documents/AquaLink_Agile_Logbook.docx). Earlier shared requirements evidence is also published in [Faith's team portfolio](https://github.com/FaithA965/FaithA965.github.io/blob/main/agile.md).

## 03. User stories and related features

The six representative stories below are derived from the team's later story mapping. They describe **user needs**, not verified end-to-end functionality.

| ID | User story | Linked screen or capability |
|---|---|---|
| US-01 | As an administrator, I want an operational overview so I can inspect relevant platform activity. | Admin dashboard |
| US-02 | As an administrator, I want household details so I can understand household accounts and assignments. | Household list and detail |
| US-03 | As an administrator, I want plans and purchases so I can understand subscription activity. | Plans and purchase screens |
| US-04 | As a supplier, I want tank information so I can monitor infrastructure conditions. | Tank overview and detail |
| US-05 | As a supplier, I want refill history so I can review previous activities. | Refill history |
| US-06 | As a supplier, I want operational alerts so I can identify issues needing attention. | Supplier and sensor alerts |

## 04. From user story to development task

A story identifies value; a development task breaks the outcome into manageable work. The following is a **proposed backend task decomposition**, not a recreated personal Trello history.

### Household information

For US-02, a sound technical breakdown would define household identity and supplier relationships, establish the read contract, validate authorisation and test both list and individual-record responses. The interface can then present the same information consistently across screens.

### Tank monitoring

For US-04, technical tasks should cover a tank identifier, supplier ownership, status, reading values, units and timestamps. The service also needs a clear distinction between live sensor values, test data and unavailable measurements.

### Operational alerts

For US-06, the team needs agreement on alert severity, the conditions that trigger an event, who may view it and what qualifies as a resolved alert. The interface is only the visible part of this workflow.

## 05. Acceptance criteria

Acceptance criteria turn a proposed feature into something that can be checked. I would separate interface checks from the additional backend checks needed for a complete service.

| Story | User-visible acceptance check | Backend evidence needed |
|---|---|---|
| US-01 | Clear dashboard with usable navigation | Verified data query and access rules |
| US-02 | Household list and details agree | Persistence and authorised household lookup test |
| US-03 | Purchases have accurate statuses | Valid state transitions and payment-provider test if live payments are claimed |
| US-04 | Tank status and values are understandable | Reading provenance, timestamps and consistent data mapping |
| US-05 | Refill events show their tank and date | Persisted history in a repeatable test |
| US-06 | Alert urgency and status are clear | Alert rule, storage and permissions tests |

The backend column is **my proposed acceptance standard**. It must not be read as a declaration that the team finished those tests.

## 06. My backend contribution and perspective

The published team charter assigned me responsibility for REST APIs, relational data design and business logic. Those responsibilities make requirements analysis especially relevant to my role: one ambiguous story can affect a database relationship, an endpoint and the interpretation of several screens.

I would prioritise clarification of who owns each data record, how actions change state, and how errors are shown to the user. These are engineering lessons supported by the project context. The shared documents do not establish an individually verified list of endpoints I completed.

## 07. Original user-story evidence

The following are source-linked screenshots from the later team's published evidence collection.

<figure class="archive-item"><a href="https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/trello/trello-12.jpg"><img loading="lazy" src="https://raw.githubusercontent.com/TonyBaloyi/Portfolio/main/evidence/trello/trello-12.jpg" alt="Original AquaLink Trello requirements screenshot 12"></a><figcaption>Requirements and task evidence · <a href="https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/trello/trello-12.jpg">Original screenshot 12</a></figcaption></figure>

<figure class="archive-item"><a href="https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/trello/trello-13.jpg"><img loading="lazy" src="https://raw.githubusercontent.com/TonyBaloyi/Portfolio/main/evidence/trello/trello-13.jpg" alt="Original AquaLink Trello requirements screenshot 13"></a><figcaption>Requirements and task evidence · <a href="https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/trello/trello-13.jpg">Original screenshot 13</a></figcaption></figure>

Additional shared evidence: [Faith's story records](https://github.com/FaithA965/FaithA965.github.io/blob/main/agile.md), [Mologadi's story image 1](https://github.com/MologadiD/Portfolio/blob/main/assets/img/stories-1.png), [image 2](https://github.com/MologadiD/Portfolio/blob/main/assets/img/stories-2.png), and [the original logbook](https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/documents/AquaLink_Agile_Logbook.docx).

## 08. Personal reflection: why acceptance criteria matter

At first glance a user story can look complete once there is a visible page for it. The project helped me distinguish that milestone from a completed service. A purchase screen can demonstrate the intended journey without a live provider. A supplier view can show an example tank reading without a physical sensor.

For someone assigned to backend work, acceptance criteria should remove that ambiguity. The team should be able to state what was implemented, what was tested and what remains simulated. This is the standard I want to hold myself to, even when presentation deadlines create pressure to describe a feature as more complete than the evidence allows.

## 09. What I would improve

1. Attach an owner and acceptance criteria to each story before planning the sprint.
2. Make database, security, service and UI tasks separately visible.
3. Identify dependencies on hardware or third-party providers early.
4. Add explicit error and permission scenarios, not only the ideal path.
5. Link every claimed completion to a verifiable artefact.
6. Record changes to story scope rather than silently replacing the initial requirement.

## 10. Connection to Agile practice

Scrum treats the Product Backlog as an evolving description of work, with refinement adding details such as order and size. A clear story and its acceptance criteria help make an increment inspectable. For AquaLink, I would apply this by separating a screen-level increment from a fully integrated workflow when those are demonstrably different.

**Reference:** Schwaber, K. and Sutherland, J. (2020), [The Scrum Guide](https://scrumguides.org/scrum-guide.html).

## 11. Final reflection

A user story is a promise to solve a user's problem, not a list of screens to draw. Its value becomes credible when requirements, technical tasks and acceptance evidence point to the same outcome. The AquaLink records provide the shared context; my next step in any individual assessment is to attach only the personal work that I can verify.

[← Agile Team Charter]({{ '/agile/team-charter/' | relative_url }}) · [Product Backlog →]({{ '/agile/product-backlog/' | relative_url }})
