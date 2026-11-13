---
layout: default
title: "Agile Team Charter"
description: "AquaLink's shared purpose, roles, working agreements and changes"
permalink: /agile/team-charter/
---

## Evidence: the actual team charter

The AquaLink team designed a proposal to improve household access to water in **Muraleni, Limpopo**, connecting households, borehole suppliers and administrators through a digital platform alongside a planned physical distribution network.

The charter provides a common statement of purpose, role assignments, responsibilities, values and communication expectations. It is a **shared project artefact**; the original PDF and Mologadi's screenshots provide the evidence.

[Read the full team charter PDF](https://github.com/FaithA965/FaithA965.github.io/blob/main/Agile_Team_Charter.pdf).

![AquaLink team charter: page one](https://raw.githubusercontent.com/MologadiD/Portfolio/main/assets/img/charter-1.png)

*Source: [Mologadi's charter image 1](https://github.com/MologadiD/Portfolio/blob/main/assets/img/charter-1.png).*

![AquaLink team charter: page two](https://raw.githubusercontent.com/MologadiD/Portfolio/main/assets/img/charter-2.png)

*Source: [Mologadi's charter image 2](https://github.com/MologadiD/Portfolio/blob/main/assets/img/charter-2.png).*

## Shared purpose and stakeholder value

The project evolved from an initially narrower water-delivery concept into the proposal for a piped-water network supported by digital records. The proposed platform considers three principal users:

| User | Intended benefit |
|---|---|
| Household | Easier connection requests and a clearer view of subscription, usage and payment information |
| Borehole supplier | A structured way to register and manage supply information |
| Administrator | Visibility over users, supply, accounts and operational information |

These describe **intended capabilities**, not independently verified completed features.

## Roles and working agreements

| Team member | Role in AquaLink | Charter responsibilities |
|---|---|---|
| Mologadi Dikgale | Project Manager | Plans iterations, tracks progress and raises blockers |
| Uhmar Adams | Lead Developer | Technical design, integration and code-review coordination |
| **Leeroy Chakanyuka** | **Backend Developer** | **REST APIs, relational schema and business logic** |
| Faith Adams | UI/UX Designer | User journeys, wireframes and interfaces |
| Phatushedzo Baloyi (Tony) | QA Tester | Test planning, verification and defect tracking |

*Role descriptions from [Faith's AquaLink Agile portfolio](https://github.com/FaithA965/FaithA965.github.io/blob/main/agile.md#1-agile-team-charter). Tony's responsibilities in a different university project are not used here.*

The team's reported values include community focus, transparency, accountability, respect, fairness, reliability and simplicity. WhatsApp was the main short-update channel, with Teams or in-person meetings for more involved planning and review discussions, and GitHub for development work. A daily stand-up was intended to communicate what had been completed, what came next and where progress was blocked.

## Changes that tested the charter

Two issues in the shared project history show why a charter must remain adaptable. First, the original charter anticipated **two-week sprints** but the initial documented sprints ran on roughly **one-week cycles**. Second, project scope changed as the water-service concept and user requirements developed. An effective charter should record such changes rather than leave the written agreements detached from reality.

## Coordination practices visible in the later team record

The later [AquaLink Agile Logbook maintained by Tony](https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/documents/AquaLink_Agile_Logbook.docx) includes examples of requirements review, interface feedback and outstanding-task analysis. The examples below provide **team-level context** about coordination rather than a claim that I led each meeting.

| Date | Documented group activity | What it illustrates |
|---|---|---|
| 27 July 2026 | Scope and agreed user stories reviewed | Shared understanding before task assignment |
| 31 July 2026 | User-story scope and priorities consolidated | Coordinating the next workstream |
| 7 August 2026 | UI feedback and outstanding screens reviewed | Making dependencies visible |
| 22 October 2026 | Remaining backlog and incomplete integrations considered | Distinguishing progress from unverified completion |
| 29 October 2026 | Roadmap and final presentation priorities revisited | Adapting as deadlines approached |

A charter is valuable only when it influences actual decisions. These records show a need for regular inspection, but they do not prove that every proposed communication rule was followed or that everyone agreed to a signed charter.

## Evidence versus retrospective proposals

The [original team charter PDF](https://github.com/FaithA965/FaithA965.github.io/blob/main/Agile_Team_Charter.pdf) is evidence of documented team intentions. Tony's later portfolio notes limitations around the team's formal agreement. Rather than erase this difference, my evaluation separates **what the original artefact says**, **what the project records show** and **what I would change next time**.

| Practice | Evidence available | Improvement I would recommend |
|---|---|---|
| Responsibility allocation | Named roles and workstreams | Record a primary owner and reviewer for each technical task |
| Communication | WhatsApp, meetings and planned stand-ups | Capture decisions and blockers against the associated backlog item |
| Scope changes | Delivery concept evolved into network-based model | Log scope and business-rule changes with their effect on the data model |
| Quality | Reviews and reported testing activities | Define a checkable completion standard for each API and workflow |
| Accountability | Tasks and progress were recorded | Agree in advance how missed deadlines are escalated |

These improvements are **recommendations**, not invented historical commitments.

## Backend-specific coordination decisions

The decisions most likely to affect my assigned workstream were about entity ownership, access control, state changes and integration boundaries. An administrator viewing households, for example, depends on a shared agreement about the household record and whether that information comes from a persistent service or a demonstration dataset.

The charter therefore matters technically: if one team member assumes a fully connected payment process while another implements only an interface, the discrepancy can survive until final testing. A written decision about integration scope, expected data and definition of done would make the dependency explicit.

## Personal reflection (STAR) — draft for review

<a id="personal-reflection"></a>

**Situation.** We had a community-focused idea that required agreement across business planning, interface design, backend development and testing. The team needed a way to avoid overlapping work, unclear decision-making and lost requirements.

**Task.** My allocated role was Backend Developer, with responsibility for thinking through how data, API contracts and business rules would support the household, supplier and administrator journeys.

**Action.** The charter established clear areas of ownership and a communication framework in which issues could be raised before they affected other members. In reviewing the shared plan, the most important dependencies for the backend role are the identity and relationship of household/supplier records, the rules for subscriptions and water usage, and the contract expected by the interface. The change from the original sprint cadence also shows why planning assumptions should be revisited.

**Result and learning.** The charter created a useful starting agreement, but the evolving scope and sprint length demonstrate that planning documents need maintenance. My main takeaway is to confirm technical dependencies early and make changes to working agreements explicit rather than assuming that everyone has the same understanding.

> **Personal check before submission:** Confirm the planning discussions you actually attended or influenced; this text does not claim you personally authored the charter or implemented the entire proposed backend.

## References

- [Faith Adams — AquaLink charter summary and team roles](https://github.com/FaithA965/FaithA965.github.io/blob/main/agile.md).
- [Mologadi Dikgale — AquaLink charter screenshots](https://github.com/MologadiD/Portfolio/tree/main/assets/img).
- [Original team charter PDF](https://github.com/FaithA965/FaithA965.github.io/blob/main/Agile_Team_Charter.pdf).

## Charter assessment: agreements compared with delivery evidence

A strong charter can be tested against the project's recorded decisions, rather than judged only by its wording. The shared charter supplies the team roles and intended values; the dated logbook and boards show which coordination activities were actually reported.

| Charter concern | What the evidence establishes | What remains uncertain | Backend lesson |
|---|---|---|---|
| Ownership | Named roles and shared planning artefacts | Assignment and completion of every individual card | Each service and data task needs a named owner and reviewer |
| Communication | WhatsApp and planning meetings were identified | Whether every stand-up occurred | Record decisions alongside the affected API or schema |
| Iteration | Early weekly sprint boards and later roadmap reviews exist | Consistent adherence to the original two-week cadence | Re-estimate work when sprint length changes |
| Quality | Team records describe screen checks and regression review | End-to-end API and persistence test coverage | Define 'done' with testable results |
| Accountability | Progress and impediments were logged | Each person's response to a specific blocker | Escalate unresolved technical dependencies before integration |

### My proposed backend working agreement

For a future team project, I would propose the following *new* agreement rather than portray it as a rule adopted by AquaLink: changes to the data model should include an updated ERD, migration or schema change, API contract impact and a test plan. Any task blocked by a product decision should name the decision-maker and expected resolution. A completed UI mock-up should never be labelled as an integrated backend feature without an end-to-end check.

## Reflection: from role allocation to shared accountability

My assigned position gave me a particular lens on the charter. A backend workstream can appear self-contained, but it depends on agreed business rules from the product side and stable expectations from frontend contributors. A supplier's tank record, for example, may affect administrator oversight, household information and monitoring screens simultaneously.

What I take from the project is the distinction between *knowing who is responsible* and *having a reliable way to verify work*. The team charter addressed the first question; tracking links between requirements, technical tasks and verifiable outcomes would strengthen the second.

This reflection describes my interpretation of the shared evidence. It does not claim that I authored Tony's logbook, chaired every recorded meeting or personally completed every listed integration.

[Read Tony's later coordination record](https://github.com/TonyBaloyi/Portfolio/blob/main/agile-team-charter.md) · [Open the original team charter](https://github.com/FaithA965/FaithA965.github.io/blob/main/Agile_Team_Charter.pdf)
