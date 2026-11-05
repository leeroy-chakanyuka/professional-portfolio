---
layout: default
title: "Agile Team Charter"
description: "AquaLink's shared purpose, roles, working agreements and changes"
permalink: /agile/team-charter/
---

[← Agile hub]({{ '/agile/' | relative_url }})

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
