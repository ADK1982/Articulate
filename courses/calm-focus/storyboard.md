---
title: Calm Focus Storyboard
layout: page
permalink: /courses/calm-focus/storyboard/
---

# Calm Focus: Storyboard

### Structure, flow, and key design decisions

[← Back to Project Background](/courses/calm-focus/project-background/)

---

## Course Overview

**Tool:** Articulate Storyline 360
**Narration:** AI voiceover via ElevenLabs (voice: Hannah)
**Approach:** Scenario-based learning centered on Maya, a remote worker two years into working from home. Learners experience the course through Maya's perspective, making decisions alongside her and living with the consequences.

**Core design principle:** Every screen presents a situation or choice, not a concept. Learners encounter stress management as a lived experience rather than a topic to study.

---

## Variable Architecture

Before the screens, the variables — because every branching decision and personalized outcome in this course traces back to them.

| Variable | Type | Purpose |
|---|---|---|
| `TriedBreathing` | True/False | Tracks whether learner explored box breathing |
| `Tried2020` | True/False | Tracks whether learner explored the 20-20-20 rule |
| `TriedMovement` | True/False | Tracks whether learner explored movement break |
| `TechniqueCount` | Number | Running total of techniques explored (0–3) |
| `BoundaryChoice` | Text | Records learner's response to the Slack scenario |
| `RitualComplete` | True/False | Tracks completion of the drag-and-drop ritual builder |

**Safeguard logic:** `TechniqueCount` increments only when a technique variable changes from False to True — not on every visit. This prevents double-counting when learners revisit a technique screen.

---

## Section 1 — Recognizing Remote Stress

**Learning goal:** Help learners recognize what remote stress looks and feels like in a realistic moment before naming it clinically.

### Screen Flow

1. **Title card** — Section title and brief orienting narration introducing Maya
2. **Maya's situation** — Scene-setting text: it's 2pm, three tabs open, a Slack notification unread for 20 minutes, a deadline in an hour. Shoulders near her ears. Narration asks: *What might help right now?*
3. **Click-to-reveal interaction** — Three cards, each with a `+` button: *Try box breathing*, *Try the 20-20-20 rule*, *Take a movement break*. Learner clicks each to expand and read a brief description. All three must be visited before the Continue button unlocks.
4. **Transition narration** — Acknowledges that Maya tried something. Sets up Section 2.

### Key Decisions

- **Unordered exploration:** Cards have no required sequence. The goal is discovery, not instruction. Learners can read in any order.
- **No right answer yet:** Section 1 introduces the techniques without evaluating them. Judgment comes in Section 2.
- **Continue gate:** The button unlocks only after all three cards are visited — ensuring learners have seen every option before moving on.

---

## Section 2 — In-the-Moment Techniques

**Learning goal:** Let learners explore each technique in more depth and track which ones they engage with, without penalizing exploration or revisiting.

### Screen Flow

1. **Section intro** — Brief narration framing the three techniques as tools in a toolkit, not a ranked list
2. **Technique hub** — Navigation screen with three paths, each leading to a dedicated technique screen
3. **Box Breathing screen** — Step-by-step guide to the technique, applied to Maya's situation. Sets `TriedBreathing = True`, increments `TechniqueCount` if not already counted.
4. **20-20-20 Rule screen** — Explanation of the technique (every 20 minutes, look 20 feet away, for 20 seconds). Sets `Tried2020 = True`, increments `TechniqueCount` if not already counted.
5. **Movement Break screen** — Short movement options suited to a home office. Sets `TriedMovement = True`, increments `TechniqueCount` if not already counted.
6. **Return to hub** — After each technique screen, learner returns to the hub. Visited states visually mark which techniques have been explored.
7. **Continue trigger** — Hub Continue button is available after at least one technique is visited. Learners are not required to try all three.

### Key Decisions

- **Non-linear, non-penalizing:** Learners choose their own path. Someone who tries all three is not rewarded over someone who tries one — both move forward. The tracking exists for personalization in Section 4, not for scoring.
- **Visited states:** Button or card states change visually after a technique is visited, giving learners a clear sense of what they've seen without a progress bar or checklist.
- **Minimum one, maximum three:** The course tracks what was explored but does not lock the learner into completing all three. This mirrors how real stress management works — people use what works for them.

---

## Section 3 — Boundary Rituals

**Learning goal:** Present a realistic boundary dilemma with meaningful consequences, then give learners a tool to build their own end-of-day ritual.

### Screen Flow

**Beat 1 — The Slack notification**

1. **Scene setup** — It's 6:45pm. Maya's day is supposed to be over.
2. **Notification screen** — A Slack message appears from a colleague asking Maya to review a proposal tonight before it goes out tomorrow. The message is friendly and low-pressure in tone. Narration prompt: *What does Maya do?*
3. **Three-choice branch:**
   - *She reviews it now* → consequence screen showing Maya working late, skipping her walk, feeling resentful
   - *She sets a boundary and declines* → consequence screen showing Maya logging off with a brief, professional response
   - *She says yes but feels guilty about it* → consequence screen exploring the cost of an unclear boundary
4. **Consequence screens** — Each branch plays out briefly, then converges. Narration reframes the moment: how Maya ends her day shapes how tomorrow starts. Sets `BoundaryChoice` to the selected response.
5. **Convergence** — All three branches return to the same screen before Beat 2.

**Beat 2 — The ritual builder**

6. **Intro screen** — Narration introduces the idea of an end-of-day ritual as a deliberate signal to the brain that work is over
7. **Drag-and-drop interaction** — Six ritual elements on the left: *Close the laptop with intention*, *Write tomorrow's top three tasks*, *Change out of work clothes*, *Take a short walk*, *Turn off Slack notifications*, *Make a cup of tea*. A drop zone on the right labeled *Maya's Evening Ritual*. Learners drag at least three elements into the zone.
8. **Completion trigger** — Custom variable triggers (layered on top of Storyline's freeform interaction) track when at least three items are in the drop zone. Sets `RitualComplete = True`. Continue button unlocks.

### Key Decisions

- **Three-choice branch, not two:** A simple yes/no boundary scenario is too easy to read. Three options — comply, decline, comply-but-resent — capture the way real boundary decisions actually feel.
- **Consequences, not judgment:** Each branch shows what happens without a score or a "wrong answer" label. Learners experience the outcome and draw their own conclusion.
- **Custom drag-and-drop tracking:** Storyline's built-in freeform drag-and-drop uses a correct/incorrect system that doesn't fit here — all combinations are valid. Custom triggers bypass that system entirely, tracking drop-zone count without evaluating which items were chosen.
- **Minimum three items:** Enough to require intentional selection, not so many that it feels prescriptive.

---

## Section 4 — Your Action Plan

**Learning goal:** Surface a personalized closing summary that reflects each learner's specific choices throughout the course.

### Screen Flow

1. **Intro screen** — Narration acknowledges that Maya (and the learner) has been through a full week. Time to build something to take forward.
2. **Personalized technique summary** — Conditional text blocks display based on `TriedBreathing`, `Tried2020`, and `TriedMovement`. Only the techniques the learner explored appear. Each is shown as a concrete action item, not a reminder of content.
3. **Boundary reflection** — A brief conditional screen references `BoundaryChoice`, acknowledging the decision made in Section 3 without re-evaluating it.
4. **Commitment screen** — Learner selects one technique they plan to try this week. A simple single-choice interaction, no branching — the action is the point.
5. **Closing slide** — Personalized sign-off. If `TechniqueCount` is 3, narration acknowledges they explored everything. If 1 or 2, it acknowledges the focused approach. No score, no certificate — just a specific, personal close.

### Key Decisions

- **Personalization through variables, not branching:** The outcome isn't a different version of the course — it's a different arrangement of the same closing content based on what was tracked. This keeps the Storyline file manageable while still feeling individualized.
- **No wrong path to arrive here:** Whether the learner tried one technique or three, declined the Slack message or accepted it, the closing screen feels like it was written for them specifically.
- **No score:** Stress management isn't pass/fail. A score would undermine the tone of the entire course.

---

[← Back to Project Background](/courses/calm-focus/project-background/)
