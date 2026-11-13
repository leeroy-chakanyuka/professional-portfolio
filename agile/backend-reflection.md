---
layout: default
title: "Engineering Reflection"
description: "A ten-part reflection on the backend role, team dependencies, technical credibility and professional growth."
permalink: /agile/backend-reflection/
---

<p class="chapter-intro">AquaLink challenged me to think beyond the code that might sit behind an interface: about the decisions, agreements and evidence needed to make the whole system trustworthy.</p>

This reflection mirrors the depth and ten-part progression of Tony's leadership-reflection chapter, but it is written from **my assigned backend-development role**. Team activities are attributed; unverified personal coding achievements are not invented.

## 01. The purpose behind the project

Water access is a serious practical problem. AquaLink aimed to explore how households, water suppliers and administrators could coordinate distribution through infrastructure and digital records. That made the project meaningful as a technical case study: the data model was not abstract, because it represented people, services and operational decisions.

The proposal's scope changed as the team moved from a delivery-oriented concept towards piped distribution. I see that as a reminder that engineering must respond to understanding the problem, not merely defend the first implementation plan.

## 02. My role and its responsibilities

### Backend workstream

The shared charter identifies me as Backend Developer, with responsibility allocated around REST APIs, relational data and business logic. These are areas that connect the application's different user-facing modules.

### Cross-team dependencies

I also needed to understand how the proposed server-side model could support the interface, service-plan rules and infrastructure data. This is an account of my assigned responsibilities and technical perspective, not a statement that I delivered every proposed backend feature.

## 03. What system design taught me

One seemingly small feature can have far-reaching implications. A household account requires an identity, a relationship to a supplier and perhaps a plan. A purchase requires a state model, reliable updates and a way to reconcile failures. Monitoring requires timestamps, data quality and rules for abnormal readings.

Designing those relationships is a discipline in reducing ambiguity. If two screens use the same term differently, their shared API contract can become the place where that disagreement causes a failure. For future work I would define entities and their rules together with the team before treating screen designs as final technical specifications.

## 04. The most difficult engineering tension

### Visible progress is not the same as verified capability

The later published logbook describes substantial Admin and Supplier interface work, while identifying real database integration, payments and physical sensors among the remaining tasks. I think this is one of the most important lessons the project offers.

It is tempting to call a flow complete because it looks complete. The more responsible position is to explain whether it uses seeded data, simulated readings or real providers. That distinction protects users, testers and the credibility of the team.

## 05. What I learned about my approach

I learned to think about the question behind a task: what assumption must be true for this feature to work? If the answer involves a database relationship, authorisation rule or third-party service, the team needs to capture it explicitly.

I also learned that good documentation has a human purpose. It prevents a teammate from making a different assumption, helps a reviewer test the correct behaviour and gives future developers a reliable starting point.

## 06. The engineer I want to become

### Establish technical contracts earlier

Document what requests, responses, identifiers and error states mean before several components depend on them.

### Make task ownership clear

A ticket should say who will produce the change, who will review it and how success will be checked.

### Communicate blocked decisions

If a business rule is unresolved, identify the decision, the affected work and the person who can resolve it.

### Test the difficult paths

Prioritise invalid inputs, missing data, permission boundaries and failed integrations, not only a successful demonstration.

### Protect time for verification

A feature should have a testing allowance before it is described as done.

### Keep evidence close to the work

Attach code history, tests and technical review to the relevant story while it is fresh.

## 07. The difference between implementing and engineering

Implementation is the work of making a feature behave as specified. Engineering also asks whether the specification is coherent, whether the feature is safe to depend on, and whether a future maintainer can understand and test it.

AquaLink's many connected workstreams make that distinction visible. When product assumptions evolve, a reliable backend approach requires corresponding changes to contracts, data and acceptance criteria—not simply new screen designs.

## 08. Evidence behind this reflection

| Evidence | What it supports | What it does not establish |
|---|---|---|
| [Original AquaLink team charter](https://github.com/FaithA965/FaithA965.github.io/blob/main/Agile_Team_Charter.pdf) | My listed backend assignment | Completion of every assigned deliverable |
| [Faith's sprint chronology](https://github.com/FaithA965/FaithA965.github.io/blob/main/agile.md) | Early architecture, ERD and planning work | My attendance at each activity |
| [Tony's original logbook](https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/documents/AquaLink_Agile_Logbook.docx) | Extended team progress and remaining integration work | A diary authored by me |
| [Shared screenshots]({{ '/agile/evidence-gallery/' | relative_url }}) | Existence of backlog and task artefacts | Code ownership |
| [Evidence register]({{ '/agile/evidence-register/' | relative_url }}) | Source attribution and verification gaps | Claims beyond the available records |

The later team sources do not agree completely on formal titles: the earlier charter lists Mologadi as Project Manager and Tony in QA, while Tony's later personal account describes Project Lead and substantial frontend work. Those accounts are presented as their respective claims rather than merged into an invented definitive allocation.

## 09. Looking beyond graduation

The practices AquaLink made visible—data modelling, clear contracts, communication, traceability and honest testing—are relevant far beyond one assignment. As I develop applications in backend engineering, I want to make decisions that other developers can inspect and extend.

I would like future portfolios to make that work easy to verify: not by expanding unsupported achievement claims, but by showing the actual design choices, commits, tests and improvements that demonstrate learning.

## 10. Final reflection

AquaLink reinforced the importance of connecting a meaningful product idea to disciplined implementation. The work a user never sees can determine whether an interface can be trusted. That is the responsibility I associate with backend engineering and the standard I want to keep improving.

[← Evidence Gallery]({{ '/agile/evidence-gallery/' | relative_url }}) · [Our Story →]({{ '/agile/our-story/' | relative_url }})
