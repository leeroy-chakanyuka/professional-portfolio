---
layout: default
title: "Backend Reflection"
description: "An individual perspective on system design, dependencies, evidence and technical accountability."
permalink: /agile/backend-reflection/
---

## The difference between a screen and a system

AquaLink's purpose was to explore reliable community water management. The team imagined a connected experience spanning suppliers, households, administrators, subscriptions, usage information and operational monitoring.

My allocated position was **Backend Developer**. The charter associates that role with APIs, relational schema design and business logic. This role made me think about the information beneath visible features: what data is needed, who owns it, what rules apply and how another component can depend on it.

The team's published material documents planning and interface progress. It does not on its own verify my individual code contributions. My reflection is therefore about **the technical decisions illustrated by the project**, not a manufactured implementation history.

## The data model as a shared contract

A household detail page raises questions about household identity and its relationship to a service plan. A purchase page introduces payment events, validation and state. A tank monitor raises questions about readings, the time those readings were generated and whether data is measured or simulated.

These are not merely database concerns. They affect the interface, acceptance criteria, testing and even what the team can accurately demonstrate. A well-designed model makes assumptions visible so that a change in product scope does not silently undermine the system.

## When project scope changes

The project evolved from a delivery-oriented concept towards a piped network supported by digital records. That kind of change creates pressure on the technical plan: entities, workflows and responsibilities may all need reconsideration.

The lesson I take from the team's shared documentation is to record a decision, its assumptions and the backlog tasks it affects. The developer who sees a dependency should raise it early, not hope that another workstream will resolve it later.

## Testing and credibility

The later group logbook describes completed interface work but identifies live database, payment and physical sensor integrations as outstanding or requiring verification. This distinction is essential.

A UI can demonstrate a journey without proving an end-to-end service exists. Backend progress should be tied to evidence such as migrations, API contracts, tests and reproducible requests. That is how a technical team can communicate both ambition and delivery limits accurately.

## My STAR reflection — review against personal evidence

**Situation.** AquaLink was a collaborative project with a community-focused goal and multiple connected technical areas.

**Task.** My assigned backend responsibility covered REST APIs, data relationships and business logic in support of the project's users and workflows.

**Action / evaluation.** The documented sequence of requirements, ERD design, technical review and later integration discussion shows why backend planning requires clear contracts. I would use acceptance criteria, explicit dependencies and verifiable artefacts to keep such a workstream aligned with the UI and business model.

**Result / learning.** The key insight is that architectural assumptions and proof of completion matter as much as feature lists. My individual achievements still need to be supplemented with my own commits, tests or dated assignments before a personal completion claim is made.

## What I would carry into the next project

1. Connect every API task to a user story and acceptance criterion.
2. Record the owner and reviewer of domain-model changes.
3. Treat persistence, authorisation and external integrations as separately testable work.
4. Document whether demonstration data is live, seeded or simulated.
5. Link completed work to reproducible tests or code history.
6. Keep an individual logbook alongside the shared sprint board.

[Read the complete Agile dossier]({{ '/agile/' | relative_url }}) · [Inspect original evidence]({{ '/agile/evidence-gallery/' | relative_url }}).
