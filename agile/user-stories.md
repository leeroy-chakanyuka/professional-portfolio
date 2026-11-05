---
layout: default
title: "User Stories and Tasks"
description: "Linking AquaLink's user needs to planned work"
permalink: /agile/user-stories/
---

[← Agile hub]({{ '/agile/' | relative_url }})

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
