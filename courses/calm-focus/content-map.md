---
title: Calm Focus Content Map
layout: page
permalink: /courses/calm-focus/content-map/
---

# Calm Focus: Content Map

### Learning objectives, content, and interaction alignment

[← Back to Project Background](/courses/calm-focus/project-background/)

---

## Course Goal

Learners will develop practical stress management strategies they can apply immediately in their remote work environment, and leave with a personalized plan built from their own choices throughout the course.

**Audience:** Remote workers experiencing stress related to isolation, boundary blur, and screen fatigue
**Format:** Scenario-based, self-paced | No facilitator required
**Duration:** Approximately 20 minutes

---

## Terminal Learning Objectives

By the end of this course, learners will be able to:

1. Recognize physical and behavioral signs of stress in a remote work context
2. Apply at least one in-the-moment stress management technique
3. Evaluate boundary options in a realistic after-hours work scenario
4. Build a personalized end-of-day ritual to signal the transition out of work mode
5. Commit to a specific stress management strategy to use going forward

---

## Content Map

### Section 1 — Recognizing Remote Stress

**Objective addressed:** #1

| Element | Detail |
|---|---|
| **Scenario** | Maya's Tuesday afternoon — deadline in an hour, Slack unread, shoulders tense |
| **Content topics** | Physical stress cues in remote work; environmental triggers; in-the-moment awareness |
| **Interaction** | Click-to-reveal: three techniques introduced (box breathing, 20-20-20 rule, movement break) |
| **Completion condition** | All three cards visited before Continue unlocks |
| **Assessment** | None — discovery only; no right or wrong answer at this stage |
| **Variables initialized** | `TriedBreathing`, `Tried2020`, `TriedMovement` all set to False; `TechniqueCount` set to 0 |

---

### Section 2 — In-the-Moment Techniques

**Objective addressed:** #2

| Element | Detail |
|---|---|
| **Content topics** | Box breathing (steps and application); 20-20-20 rule (mechanism and use); movement breaks (home office–appropriate options) |
| **Interaction** | Non-linear technique hub — learner chooses order of exploration; visited states mark completed techniques |
| **Completion condition** | At least one technique visited; Continue available immediately |
| **Assessment** | None — exploration tracked for personalization, not scored |
| **Variables updated** | Technique variables set to True on first visit; `TechniqueCount` increments with safeguard against double-counting |

---

### Section 3 — Boundary Rituals

**Objectives addressed:** #3, #4

| Element | Detail |
|---|---|
| **Content topics** | Recognizing boundary dilemmas; the cost of unclear limits; end-of-day rituals as a cognitive transition tool |
| **Interaction 1** | Three-choice scenario branch: Maya receives an after-hours Slack message and must respond |
| **Branch options** | Review it now / Set a boundary and decline / Agree but feel guilty |
| **Consequences** | Each choice leads to a distinct outcome screen before converging — no score, consequence-based learning |
| **Interaction 2** | Drag-and-drop ritual builder: learner selects at least 3 of 6 elements for Maya's evening ritual |
| **Completion condition** | Minimum 3 items in drop zone; tracked via custom variable triggers |
| **Assessment** | Consequence-based (Branch 1); completion-based (drag-and-drop) |
| **Variables updated** | `BoundaryChoice` records selected branch; `RitualComplete` set to True on drag-and-drop completion |

---

### Section 4 — Your Action Plan

**Objective addressed:** #5

| Element | Detail |
|---|---|
| **Content topics** | Personal technique recap; boundary reflection; commitment to action |
| **Interaction** | Single-choice commitment screen: learner selects one technique to try this week |
| **Personalization** | Technique summary displays only techniques the learner explored (`TriedBreathing`, `Tried2020`, `TriedMovement`); closing narration varies based on `TechniqueCount` |
| **Completion condition** | Commitment selection made |
| **Assessment** | None — reflection and commitment only; no score |

---

## Objective-to-Section Alignment

| Objective | Section 1 | Section 2 | Section 3 | Section 4 |
|---|:---:|:---:|:---:|:---:|
| 1. Recognize stress signs | ✓ | | | |
| 2. Apply a technique | | ✓ | | |
| 3. Evaluate boundary options | | | ✓ | |
| 4. Build an end-of-day ritual | | | ✓ | |
| 5. Commit to a strategy | | | | ✓ |

---

## Interaction Summary

| Section | Interaction Type | Scored? | Tracked for Personalization? |
|---|---|:---:|:---:|
| 1 | Click-to-reveal | No | No |
| 2 | Non-linear branching hub | No | Yes |
| 3 | Three-choice scenario branch | No | Yes |
| 3 | Drag-and-drop builder | No | Yes |
| 4 | Single-choice commitment | No | No |

---

[← Back to Project Background](/courses/calm-focus/project-background/)
