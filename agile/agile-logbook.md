---
layout: default
title: "Agile Logbook"
description: "AquaLink team chronology, documented blockers and individual learning"
permalink: /agile/agile-logbook/
---

## 1. What the logbook demonstrates

The purpose of an Agile logbook is to make work visible over time: what was done, what was planned, what impeded progress, how issues were addressed and what was learned. It supports sprint planning and retrospectives rather than serving only as an attendance register.

**Source distinction:** Mologadi's images and Faith's published chronology show the group's project record. They are not a substitute for my own dated stand-up notes and must not be presented as if I personally made every entry.

## 2. Original logbook artefacts

![AquaLink logbook screenshot one](https://raw.githubusercontent.com/MologadiD/Portfolio/main/assets/img/logbook-1.png)

*Source: [Mologadi's original Agile logbook screenshot 1](https://github.com/MologadiD/Portfolio/blob/main/assets/img/logbook-1.png).*

![AquaLink logbook screenshot two](https://raw.githubusercontent.com/MologadiD/Portfolio/main/assets/img/logbook-2.png)

*Source: [Mologadi's original Agile logbook screenshot 2](https://github.com/MologadiD/Portfolio/blob/main/assets/img/logbook-2.png).*

The taskboards for [Sprint 1](https://github.com/FaithA965/FaithA965.github.io/blob/main/Taskboard_Sprint1.png), [Sprint 2](https://github.com/FaithA965/FaithA965.github.io/blob/main/Taskboard_Sprint2.png), [Sprint 3](https://github.com/FaithA965/FaithA965.github.io/blob/main/Taskboard_Sprint3.png) and [Sprint 4](https://github.com/FaithA965/FaithA965.github.io/blob/main/Taskboard_Sprint4.png) provide additional dated team context.

## 3. Team-level chronological summary

The following is an **attributed synthesis of Faith's public AquaLink logbook**. It is not my personal stand-up transcript.

| Date | Team-level activity described in the source | Question or dependency recorded |
|---|---|---|
| 14 July 2026 | Began clarifying the community water-access problem | Scope and requirements were still forming |
| 15 July 2026 | Discussed connections between households and suppliers | Which functions belonged in the first version |
| 16 July 2026 | Considered subscriptions, usage and supplier-payment processes | How the physical system and software should fit together |
| 17 July 2026 | Reviewed requirements and the proposed direction | Technical and operational aspects still needed work |
| 21 July 2026 | Began planning the database schema | Task detail needed clarification |
| 22 July 2026 | Considered entities for different types of users | Some business rules were not final |
| 23 July 2026 | Discussed relationships between entities | Work depended on team decisions |
| 24 July 2026 | Continued preparation and review of the proposed schema | Source reports no major blocker for its author |
| 28 July 2026 | Began work on the shared stylesheet | Design decisions were not final |
| 29 July 2026 | Reviewed colours, typography and reusable styles | Styles might change following review |
| 30 July 2026 | Worked on layout elements and responsiveness | Source reports no major blocker for its author |
| 4 August 2026 | Reviewed architecture and began ERD review | Some decisions needed discussion |
| 5 August 2026 | Examined ERD entities and relationships | Certain relationships needed clarification |
| 6 August 2026 | Recorded technical design issues and proposed changes | The author reported fewer immediate blockers |
| 7 August 2026 | Prepared reviewed design for team approval | Final approval was still pending in the source |

*Source: [Faith's Agile Logbook section](https://github.com/FaithA965/FaithA965.github.io/blob/main/agile.md#5-agile-logbook). The table describes shared project context; it is **not a claim of my presence or participation in every activity**.*

## 4. What the team record reveals

### Sprint 1 — Scope and uncertainty

Initial questions were not just technical: the team needed to decide what kind of water service was being proposed, what households needed and how suppliers would participate. This uncertainty mattered because the solution changed from an initial delivery approach toward network connections and a multi-user digital platform.

### Sprint 2 — Data modelling and business rules

By the database sprint, the main uncertainty concerned the representation of data and relationships. The proposed concepts included households, suppliers, water sources, service plans, usage and payments. A backend developer cannot confidently specify API interactions without agreeing these relationships and the rules governing them.

### Sprint 3 — Interface consistency

The shared stylesheet work focused on ensuring that different pages had consistent layout and components. This illustrates how a project can have parallel technical areas, though it does not establish a personal backend contribution to those UI tasks.

### Sprint 4 — Review before implementation

The team used technical review to revisit the architecture and ERD. The original record explicitly notes questions about entity relationships and an approval dependency; these are more useful than a generic entry saying only that the team was 'busy'.

## 5. Retrospective: learning from the evidence

**What worked:** The documented work moved from problem discovery to a data design and then a review of its technical implications. The taskboard and stand-up structure helped make unfinished decisions visible.

**Challenges:** The scope and business rules were still evolving, so technical design depended on decisions that were not fully settled. The initial charter sprint length and actual iteration cadence also differed.

**Improvement for future work:** Record assumptions and owners early, identify the decision needed to unblock a technical task, update plans when the scope changes and distinguish planned tasks from verified outputs.

**How to measure improvement:** Track whether story acceptance criteria and entity relationships were agreed before implementation, and whether blockers were linked to an owner and resolved through review.

## 6. Extended chronology: development through October

Tony's original document provides a second, later source of team-level chronology spanning **27 July to 29 October 2026**. The timeline below extends the earlier summary without presenting Tony's first-person entries as my own.

| Period | Team-reported focus | Interpretation for backend planning |
|---|---|---|
| 27–31 July | Scope, stories and navigation requirements | Agree data needs before specifying APIs |
| 3–7 August | UI foundations and reusable components | Maintain stable expectations between UI and services |
| 10–14 August | Architecture, entities and tank/sensor data | Clarify IDs, readings, status and timestamps |
| 17–28 August | Administrator and Supplier screens | Distinguish interface progress from data access |
| 31 August–11 September | Shared logic and cross-screen consistency | Recheck API assumptions as navigation develops |
| 14 September–2 October | Testing, review, responsiveness and bug fixing | Separate screen-level tests from backend integration tests |
| October | Outstanding integrations, documentation and demo readiness | Report limitations clearly rather than overstating completion |

*Source: [Tony's Agile Logbook page](https://github.com/TonyBaloyi/Portfolio/blob/main/agile-logbook.md) and the [original dated Word document](https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/documents/AquaLink_Agile_Logbook.docx).*

## 7. What the later record clarifies about project completion

The later logbook describes development of Administrator and Supplier screens and a range of review activities. It also distinguishes those interfaces from unfinished or unverified elements, especially persistent database workflows, payment-provider integration and physical sensor data.

From a backend perspective this is not a small semantic difference. A page can render data without a live persistence layer; a tank widget can show sample readings without connected sensors; and a purchase flow can illustrate the intended interaction without processing a verified payment. A logbook should tell an assessor which of those states exists.

## 8. A stronger logbook method for future work

A verifiable individual entry would include the date, task reference, what changed, the result, a blocker if any and an independent artefact. A Git commit can show a code change; a test result can support behaviour; an issue comment can document a design decision. A screenshot alone may show a screen but does not necessarily establish its author.

The distinction is why the template below remains deliberately open until my own dated records are added.

## 9. Personal logbook records — to confirm

| Date | My actual backend activity | Next action | Blocker / decision | Verifiable evidence |
|---|---|---|---|---|
| *Verify* | *An activity I can personally account for* | *What I planned at that time* | *My actual blocker, or none* | *Trello card, commit, document or message* |

This table is intentionally not populated with someone else's daily accomplishments. My own commits, notes and task assignments are the appropriate basis for completing it.

## 10. Personal reflection (STAR) — draft for review

<a id="personal-reflection"></a>

**Situation.** AquaLink involved a series of linked decisions about the service concept, users, database and architecture. The team needed to see what had changed between iterations and which issues remained unresolved.

**Task.** As Backend Developer, I needed to understand the requirements affecting the data model and planned APIs, and work within a process that raised dependencies rather than leaving them hidden.

**Action.** The published Agile logbook illustrates the value of recording specific issues: uncertainty about scope in the first sprint, missing business rules during database design and questions about relationships during technical review. For my backend work, the lesson of those entries is that technical tasks should begin with a clear statement of what is known, what is assumed and who can resolve outstanding questions.

**Result and learning.** The record makes the project's evolution easier to understand and gives a more useful basis for reflection than a list of activities without context. I would improve future work by linking each significant technical decision and blocker to the user story or task it affected, and by keeping explicit evidence of how an uncertainty was resolved.

> **Personal check before submission:** The chronology above is Faith's published team context, **not** an individual diary authored by Leeroy. Add your actual dated entries and outcomes before representing this as a complete personal logbook.

## References

- [Faith Adams — AquaLink Agile Logbook and four early sprints](https://github.com/FaithA965/FaithA965.github.io/blob/main/agile.md#5-agile-logbook)
- [Mologadi Dikgale — Agile logbook screenshots](https://github.com/MologadiD/Portfolio/tree/main/assets/img)
- [AquaLink Trello Board](https://trello.com/b/5lxVBUSK/aqualink)

## 11. How the later logbook connects technical work and delivery

Tony's dated record is particularly useful because it distinguishes *completed*, *planned* and *impeded* activities. Reading it from a backend perspective reveals a recurrent theme: the relationship between a screen that represents intended data and a system that can actually persist, validate and retrieve that data.

| Development phase | Team-reported evidence | Backend question I would raise |
|---|---|---|
| Requirements (July) | Stories and scope reviewed | Which rules determine a valid household or supplier? |
| Interface foundations (early August) | Shared UI and consistency work | What response shape will every screen expect? |
| Architecture (mid-August) | Database and sensor requirements discussed | How are readings associated with tanks and timestamps? |
| Role-specific screens (late August) | Admin and Supplier pages developed | Which endpoints and permissions support these views? |
| Shared logic (September) | Navigation and reuse reviewed | How will clients handle unavailable or invalid data? |
| Testing and finalisation (September–October) | Regression review and remaining integrations noted | Which flows were actually verified end-to-end? |

The final column records questions I would ask as a backend developer; it is not a retrospective claim that I asked them on those dates.

## 12. A verifiable individual-entry standard

My individual logbook would be strongest if each entry connected the planned work to an independently inspectable outcome. This is the record format I would apply to evidence I can personally verify:

| Field | What belongs here |
|---|---|
| Date and task reference | Actual work date and Trello/issue identifier |
| Work completed | Specific API, entity, rule, schema or review contribution |
| Evidence | Commit, PR, approved ERD, test result or message |
| Blocker and resolution | What prevented progress and who resolved it |
| Next action | The next verifiable development step |

Without those records, the published July–October chronology remains attributed shared context. Reusing its dates as my personal daily work would make the portfolio less reliable, not more complete.

## 13. My final learning from the chronological record

The clearest lesson from the record is that planning and implementation are not interchangeable. Early uncertainty about the water-service model flowed into database questions, and unresolved integrations remained visible even after interface work progressed. A useful logbook makes that relationship traceable.

In my next team project I would attach backend decisions to the story they affect, write down unresolved assumptions and use tests or code history to establish when a technical task is truly finished. I would also distinguish project-wide progress from the work that I can substantiate as my own.

[Read Tony's original timeline and reflection](https://github.com/TonyBaloyi/Portfolio/blob/main/agile-logbook.md) · [Original AquaLink logbook document](https://github.com/TonyBaloyi/Portfolio/blob/main/evidence/documents/AquaLink_Agile_Logbook.docx)
