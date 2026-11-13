---
layout: default
title: "User Stories and Tasks"
description: "Linking AquaLink's user needs to planned work"
permalink: /agile/user-stories/
---

## Evidence: original user-story artefacts

User stories describe a need from the user's point of view. The associated tasks turn that need into work that can be planned and verified. In AquaLink, stories were considered for **households**, **borehole suppliers** and **administrators**, with a series of research, data-modelling, design and technical-review activities.

![AquaLink user stories](https://raw.githubusercontent.com/MologadiD/Portfolio/main/assets/img/stories-1.png)

*Source: [Mologadi's user-story screenshot](https://github.com/MologadiD/Portfolio/blob/main/assets/img/stories-1.png).*

![AquaLink task breakdown](https://raw.githubusercontent.com/MologadiD/Portfolio/main/assets/img/stories-2.png)

*Source: [Mologadi's task-breakdown screenshot](https://github.com/MologadiD/Portfolio/blob/main/assets/img/stories-2.png).*

The following summary draws on [Faith's published AquaLink story breakdown](https://github.com/FaithA965/FaithA965.github.io/blob/main/agile.md#2-user-stories-and-tasks). The source is a teammate's narrative, **not** a verified export of individual Trello assignments.

## Story and task mapping

| User / desired outcome | Work described in team documentation | Reported sprint |
|---|---|---|
| Resident needing reliable water | Research the water-access problem, household needs and service model | 1 |
| Household requesting a connection | Identify required household details and map the request journey | 1 |
| Borehole owner registering supply | Identify supplier information and proposed monitoring requirements | 1 |
| Household managing subscriptions, payments and usage | Define entities and relationships joining households, plans, transactions and usage | 2 |
| Borehole owner managing water-source information | Define borehole/supplier entities and attributes; develop the ERD | 2 |
| User expecting consistent navigation | Develop shared typography, controls, colours and responsive layout | 3 |
| Administrator overseeing supply | Review architecture, relationships and access to operational data | 4 |

## Relevance to my allocated backend role

My assigned responsibility was **REST API development, database schema and business logic**. The backend-related story work therefore depended on requirements that were often identified before implementation.

A household-account story, for example, raises specific technical questions: Which record represents the household? How does it link to a service plan? How are payments and water usage associated with the correct account? Which part of the application enforces each rule? The data-model sprint addressed relationships between these concepts; the technical-review sprint provided a later point at which the design could be challenged.

This demonstrates why a developer should separate **story definition**, **design**, **implementation** and **verification**. A planned data relationship or approved story is not the same as a working and tested endpoint.

## User-story quality and acceptance criteria

The project's documentation highlights the value of breaking a broad goal into smaller tasks. A strong technical acceptance criterion should be specific enough to verify: the required data is valid, linked to the correct entity, handled consistently for failures and accepted by the relevant user role. These are recommendations for quality, not claims about a completed AquaLink API test suite.

## User stories from the later application record

Tony's [User Stories and Tasks portfolio](https://github.com/TonyBaloyi/Portfolio/blob/main/user-stories-and-tasks.md) describes an application focused on **Administrator** and **Supplier** sign-in roles. Households were represented through records and subscriptions rather than confirmed as users of a separate consumer application. This is an important distinction between the original vision and the interfaces described in the later logbook.

The following IDs are **portfolio traceability labels**, not a claim to reproduce exact Trello card identifiers.

| ID | User need, expressed as a story | Related proposed feature |
|---|---|---|
| US-01 | As an administrator, I need an operational overview so I can review platform activity. | Admin dashboard |
| US-02 | As an administrator, I need household information so I can inspect records and supplier assignments. | Household list and detail |
| US-03 | As an administrator, I need plan and purchase information so I can track subscription-related records. | Plans and purchases |
| US-04 | As a supplier, I need tank details so I can review water infrastructure status. | Tanks overview and details |
| US-05 | As a supplier, I need refill history so I can inspect earlier activity. | Refill history |
| US-06 | As a supplier, I need relevant alerts so I can respond to operational issues. | Supplier and sensor alerts |

## From a story to a backend acceptance criterion

A story is not sufficient until its **testable behaviour** is clear. As a worked example, consider US-02 (household records). A backend plan would need to determine:

1. Which household fields are required, optional or protected.
2. How a household maps to a supplier or service plan.
3. Who may view, create or change each record.
4. What response is expected when the record does not exist or validation fails.
5. What evidence proves the data persists and is associated with the correct user.

These are **proposed acceptance questions**, not statements that AquaLink passed these tests.

## Feature and integration traceability

| User-facing capability reported in the logbook | Backend dependency to verify | Evidence still required for an end-to-end claim |
|---|---|---|
| Household detail page | Stable household model and retrieval API | Endpoint contract, sample response, test and stored record |
| Plan and purchase screens | Subscription and transaction relationships | Persistence and verified payment-provider interaction |
| Tank monitoring screen | Tank and reading data contracts | Data source and, for real IoT claims, connected hardware |
| Operational alerts | Event schema and alert lifecycle | Trigger logic, handling, storage and tests |

The [original team logbook](https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/documents/AquaLink_Agile_Logbook.docx) identifies some of these integrations as outstanding at the documented point in the project. A visible screen does not establish that all dependencies were fulfilled.

## Personal reflection (STAR) — draft for review

<a id="personal-reflection"></a>

**Situation.** AquaLink began with a community water problem, but that broad problem needed to be translated into requirements for very different users. A household, supplier and administrator do not need the same information or actions.

**Task.** As the Backend Developer, my allocated responsibility was to connect those requirements to the data model and planned backend functionality, rather than treating endpoints as isolated pieces of code.

**Action.** The team story record shows a progression from identifying household and supplier needs during research to defining their relationships in the schema, followed by a technical review. Looking at the household-account requirement shows how a story's purpose informs which entities and rules must be considered. This also demonstrates the need to confirm assumptions with the team before finalising API behaviour.

**Result and learning.** Writing and refining stories around user value creates a stronger basis for technical decisions. The key lesson is to clarify what the user needs and what counts as an acceptable outcome **before** deciding how the backend should implement it. In future, I would request explicit acceptance criteria and link each backend task to its originating story.

> **Personal check before submission:** Add the exact story IDs/cards and specify which database or API tasks you actually completed. No undocumented implementation is claimed here.

## References

- [Faith Adams — AquaLink user stories and tasks](https://github.com/FaithA965/FaithA965.github.io/blob/main/agile.md#2-user-stories-and-tasks).
- [Mologadi Dikgale — project story screenshots](https://github.com/MologadiD/Portfolio/tree/main/assets/img).
- [AquaLink Trello](https://trello.com/b/5lxVBUSK/aqualink).
