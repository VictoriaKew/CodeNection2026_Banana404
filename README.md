# Orbit by Banana404

**Team:** Yow Jia Yen, Goh Ching Yee, Victoria Kew Kim Tian, Yong Zi Yan

**Problem Statement:** Stress & Workload Manager

**Video Presentation:** [INSERT UNLISTED YOUTUBE LINK]

**Presentation Slides:** [INSERT PUBLIC CANVA LINK]

---

# 1. Project Overview

## The Problem

Traditional productivity applications are designed around the assumption that users should continuously adapt themselves to their workload.

Task lists, deadlines, priorities, overdue indicators, reminders, streaks, and productivity dashboards can be useful when users have enough energy and attention to manage them. However, a person's capacity is not constant. On stressful or exhausting days, seeing the same workload can make tasks feel even more overwhelming.

For students and young adults balancing academic responsibilities, administrative tasks, personal commitments, social activities, and recovery, the problem is not always a lack of productivity.

Sometimes, **the workload simply does not match the user's current capacity.**

Existing productivity applications such as conventional task managers and productivity dashboards primarily focus on what needs to be completed. They generally present tasks as lists and encourage users to complete as many tasks as possible.

Orbit takes a different approach:

> **Instead of asking the user to adapt to the workload, Orbit adapts the workload experience to the user's capacity.**

### Target Users

Orbit is designed primarily for:

* University students
* Young adults
* People balancing multiple responsibilities
* Users who experience fluctuating daily capacity
* Users who feel overwhelmed by conventional task-management interfaces
* Users who want productivity support without guilt or pressure

### Our Core Insight

People do not have the same capacity every day.

Therefore, a task-management system should not treat every day as if the user's available energy and attention are constant.

Orbit explores whether adapting the workload experience to a user's **self-reported capacity** can make the workload feel more manageable and give users greater control over what they need to handle.

> **Design boundary:** Orbit's capacity and Energy Ripple system are symbolic interaction mechanisms. They are not scientific measurements, medical assessments, or mental-health diagnoses.

### Our Solution

**Orbit** is a stress-aware task-management mobile application built around the principle:

> **"When you have less capacity, we ask less of you."**

Instead of immediately presenting users with a large task list, Orbit first asks how much they can handle today. The user's capacity influences the visual environment and workload experience. Users can then perform a natural-language brain dump, which is interpreted into individual tasks that appear one at a time. Tasks can be completed, frozen, chunked, parked, or deleted through physical directional interactions.

The product aims to make workload feel **possible**, rather than simply pushing users to become more productive.

### Feature Set

#### Capacity Check

Users begin with:

> **"Good morning. How much can you handle today?"**

They select their current capacity using a gentle face/emoji scale and slider.

#### Capacity-Adaptive Environment

The cosmic environment responds visually to the user's reported capacity through elements such as:

* Star brightness
* Energy ripple
* Visual activity
* Overall environmental atmosphere

#### Gentle Mode

When capacity is low, Orbit adapts the workload experience towards:

* Smaller actions
* Simpler tasks
* Lower-friction interactions
* Smaller chunks
* Optional recovery suggestions

Gentle Mode does not prevent the user from using the application.

#### Empty Task Environment

After the capacity check, Orbit opens into an empty cosmic task environment.

The user does not immediately see a conventional task list or automatically populated task card.

Instead, the environment waits for the user to tell Orbit what they need to handle.

#### Voice-Based Brain Dump

Users can long-press the task environment to provide a natural-language brain dump.

For example:

> "I need to finish my multimedia assignment, reply to the team email, review the design feedback, and prepare my weekly notes."

Orbit interprets this as separate tasks.

#### AI Task Interpretation

The intended interaction is:

**Listening → Processing → Got It → Task Creation**

One voice interaction can produce multiple independent task objects.

For the prototype, deterministic/hardcoded data may be used to simulate the AI interpretation. The interaction must still demonstrate the correct story: the user provides input first, Orbit processes it, and the resulting tasks appear afterwards.

#### One Task at a Time

Orbit avoids presenting users with a conventional infinite task list.

After tasks are created, they appear one at a time so the user can focus on the immediate task.

#### Directional Task Gestures

| Direction | Action | Meaning              |
| --------- | ------ | -------------------- |
| **Right** | Done   | "I'm finished."      |
| **Left**  | Freeze | "Not now."           |
| **Up**    | Chunk  | "Make this smaller." |
| **Down**  | Delete | "Remove this."       |

#### Park / Background

Park is a separate depth-based interaction rather than a fifth swipe direction.

A parked task moves farther into the background and becomes smaller, dimmer, softer, and slightly blurred.

It represents:

> **"I don't know what to do with this right now."**

#### Freeze

Frozen tasks move into the outer orbit and visually become colder.

Freeze represents:

> **"Not now."**

The user can later bring the same task back into the active space.

#### Chunk

A large task can be broken into smaller actions.

For example:

**Finish Multimedia Assignment**

can become:

* Open the assignment brief
* Identify the 3 sections I need to complete

The smaller tasks remain connected to the original task through their task identity.

#### Recovery Mode

When capacity is low, users can optionally enter a 2-minute recovery experience.

The prototype includes:

* 2:00 countdown
* Calm breathing visualization
* Cosmic charging/recovery animation

Recovery is an invitation rather than an obligation.

#### No-Guilt Design

Orbit deliberately avoids:

* Streaks
* Productivity scores
* Shame messages
* "You failed" messages
* Red overdue warnings
* Aggressive notifications
* Endless task counters
* Pressure to complete everything

The intended message is:

> **"You are allowed to have limited capacity."**

---

# 2. Ideation & Process

## 2.1 Ideas We Considered

The team explored multiple approaches to the problem of stress and workload management.

| Idea                                              | Why it was kept / dropped                                                                                                                                                                                                                                    |
| ------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **A. Adaptive Load Manager + Cosmic UI — Chosen** | Directly addresses the team's core insight that workload should adapt to the user's current capacity. The cosmic environment also provides a distinctive visual language for communicating capacity without relying on conventional productivity dashboards. |
| **B. Voice-Based Multi-Task Input — Chosen**      | Reduces the friction of manually entering multiple tasks. One natural brain dump can become multiple structured tasks, creating a clear end-to-end interaction for the prototype.                                                                            |
| **C. Gamified Productivity Tracker — Dropped**    | Streaks and productivity-focused mechanics conflicted with Orbit's no-guilt philosophy. A low-capacity day should not make the user feel that they have failed.                                                                                              |

### Decision Principle

The team evaluated ideas around one central question:

> **"How can we make the workload feel possible?"**

This led us towards adaptive workload management, natural task creation, and low-pressure task interactions rather than conventional productivity scoring.

---

## 2.2 Ideation Boards

### FigJam Brainstorming Board

**Link:** [INSERT FIGJAM BRAINSTORMING LINK]

The board documents the team's brainstorming process, including exploration of:

* Burnout and workload problems
* Existing productivity approaches
* Adaptive workload concepts
* Voice input
* Gesture-based interactions
* Cosmic interface concepts
* Feature ideas
* Ideas that were eventually dropped

### Affinity Diagram / User Flow

**Link:** [INSERT MIRO / FIGJAM LINK IF APPLICABLE]

[INSERT IMAGE OR EMBEDDED BOARD HERE IF AVAILABLE]

### Supporting Ideation Documentation

**Google Docs:** [INSERT GOOGLE DOCS DOCUMENTATION LINK]

---

## 2.3 Mentor Consultation

### UI/UX Mentor — May 2026

| Date         | Mentor Feedback Received                                                           | What Was Changed                                                                                                          |
| ------------ | ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| **May 2026** | The initial interface looked too similar to a conventional productivity dashboard. | The team moved away from standard dashboard conventions and redesigned the experience around an empty cosmic environment. |
| **May 2026** | Bottom navigation was unnecessary for the core interaction.                        | Removed bottom navigation.                                                                                                |
| **May 2026** | The hamburger menu added unnecessary navigation complexity.                        | Removed hamburger navigation.                                                                                             |
| **May 2026** | A floating "+" button made the experience feel like a conventional task manager.   | Removed the floating "+" button and made long press the task-creation interaction.                                        |
| **May 2026** | The interface needed to better communicate Orbit's unique concept.                 | Introduced the cosmic environment and capacity-responsive visual language.                                                |

The feedback shifted the product away from:

> **"Here is your task list. Now be productive."**

towards:

> **"Tell me what you need to handle. I'll help make the load manageable."**

### Additional Mentor Consultation

**Documentation / Evidence:** [INSERT GOOGLE DOCS OR OTHER LINK IF APPLICABLE]

---

# 3. Design & Prototype

## UI Prototype

**Figma Prototype:** [INSERT PUBLIC FIGMA PROTOTYPE LINK]

> **Submission check:** Ensure the prototype link can be opened in an incognito window without requiring the reviewer to log in.

The prototype focuses on demonstrating Orbit's core vertical slice rather than attempting to implement every possible future feature.

---

## Key Screens

### 1. Capacity Check

**Screenshot:** [INSERT IMAGE]

The user begins by answering:

> **"Good morning. How much can you handle today?"**

The user selects their capacity using the face/emoji scale and slider.

---

### 2. Empty Task Environment

**Screenshot:** [INSERT IMAGE]

After setting capacity, the user enters the cosmic task environment.

The center is intentionally empty.

There is:

* No conventional task list
* No automatically populated task
* No placeholder card
* No large Continue button
* No floating "+" button

The environment waits for intentional user input.

---

### 3. Listening

**Screenshot:** [INSERT IMAGE]

The user long-presses the environment to begin voice input.

Orbit displays:

> **"Listening..."**

The environment responds with subtle cosmic feedback such as ripples, glow, and movement.

---

### 4. Processing / Got It

**Screenshot:** [INSERT IMAGE]

After the user releases the long press, Orbit transitions through:

**Listening → Processing → Got It**

Possible processing text:

> **"Understanding your tasks..."**

The task card should not appear immediately. The staged interaction makes the AI interpretation experience clear during the demonstration.

---

### 5. Active Task

**Screenshot:** [INSERT IMAGE]

After "Got It", the first interpreted task enters the center of the environment.

Only one task is active at a time.

The task card contains useful information such as:

* Task title
* Estimated duration
* Category
* Optional subtle deadline information

The card avoids unnecessary dashboard-style controls.

---

### 6. Chunk

**Screenshot:** [INSERT IMAGE]

The user drags a large task upward.

The card visually cracks/splits into smaller actions.

Example:

**Finish Multimedia Assignment**

↓

**Open the assignment brief**

**Identify the 3 sections I need to complete**

The resulting tasks have their own unique IDs and retain their relationship to the original task.

---

### 7. Freeze / Park

**Screenshot:** [INSERT IMAGE]

**Freeze — LEFT**

The task moves into the colder outer orbit.

Meaning:

> **"Not now."**

**Park — Background**

The task moves backwards into the inner background and becomes:

* Smaller
* Dimmer
* Softer
* Slightly blurred

Meaning:

> **"I don't know what to do with this right now."**

These two states are intentionally different.

---

### 8. Recovery Mode

**Screenshot:** [INSERT IMAGE]

When appropriate, the user can enter:

> **"2 MIN RESET"**

The recovery environment shows:

**2:00 → 0:00**

with a calm cosmic breathing/charging visualization.

After the countdown reaches zero, the application returns to the task environment rather than resetting the user's tasks.

---

## Complete Golden Demo Path

The main demonstration focuses on one complete end-to-end transformation.

### Step 1 — Capacity

Open Orbit.

Show:

> **"Good morning. How much can you handle today?"**

Set capacity around 40%.

The environment becomes softer.

### Step 2 — Empty Environment

Swipe upward into the task environment.

The center is empty.

### Step 3 — Voice Brain Dump

Long press and show:

> **"Listening..."**

Say:

> "I need to finish my multimedia assignment, reply to the team email, review the design feedback, and prepare my weekly notes."

### Step 4 — AI Interpretation

Release.

Show:

> **"Understanding your tasks..."**

Then:

> **"Got it."**

### Step 5 — Tasks Appear One at a Time

The first task appears:

**Multimedia Assignment**

↓

User completes it.

Then:

**Reply to Team Email**

↓

User completes it.

Then:

**Review Design Feedback**

↓

User completes it.

Then:

**Prepare Weekly Notes**

↓

User completes it.

This demonstrates:

> **One natural voice input → AI interpretation → multiple separate task objects → one active task at a time.**

### Step 6 — Chunk

Demonstrate:

**Finish Multimedia Assignment → UP**

The task splits into two smaller actions.

### Step 7 — Freeze

Demonstrate:

**Reply to Team Email → LEFT**

The task moves into the colder outer orbit.

Explain:

> **"Freeze means not now."**

### Step 8 — Park

Demonstrate:

**Review Design Feedback → Background**

The task becomes smaller, dimmer, softer, and farther away.

Explain:

> **"Park means I don't know what to do with this right now."**

### Step 9 — Delete

Demonstrate:

**Prepare Weekly Notes → DOWN**

The task falls into the cosmic void.

### Step 10 — Recovery

When capacity is low, show:

> **"You've done enough for now."**

> **"Your capacity is low."**

> **"2 MIN RESET"**

Enter Recovery Mode.

---

# 4. What Makes It Different

Orbit is not simply a conventional task manager with a different visual theme.

Its main difference is that **user capacity becomes part of the workload-management experience.**

## 1. Capacity Changes the Workload Experience

Traditional task managers generally present the workload regardless of how much capacity the user has that day.

Orbit begins with:

> **"How much can you handle today?"**

The response influences the experience and environment.

---

## 2. The Cosmic UI Is Functional

The cosmic environment is part of the interaction model rather than purely decorative.

Elements such as:

* Energy Ripple
* Star brightness
* Orbit depth
* Visual movement

help communicate the user's current capacity and task state.

The Energy Ripple is explicitly symbolic rather than scientific.

---

## 3. One Active Task at a Time

Orbit avoids showing a conventional task list.

Instead, the user's attention is directed towards one active task.

This makes the immediate next action more obvious.

---

## 4. Four-Direction Task Interaction

Orbit turns task management into a physical interaction system:

| Direction | Action | User Meaning         |
| --------- | ------ | -------------------- |
| Right     | Done   | "I'm finished."      |
| Left      | Freeze | "Not now."           |
| Up        | Chunk  | "Make this smaller." |
| Down      | Delete | "Remove this."       |

The interaction is designed to make task management feel more physical and less administrative.

---

## 5. Voice Brain Dump

Instead of manually creating tasks one at a time, the user can describe multiple responsibilities naturally.

One voice interaction can become multiple independent tasks.

This creates a clear transformation:

> **Unstructured thoughts → structured tasks → manageable actions**

---

## 6. Chunking Instead of Simply Prioritizing

Conventional task managers often ask users to prioritize or schedule large tasks.

Orbit provides a different interaction:

> **If the task feels too big, make it smaller.**

Chunking converts one large task into smaller actions.

---

## 7. Freeze and Park Have Different Meanings

Orbit distinguishes between:

**Freeze**

> "Not now."

and

**Park**

> "I don't know what to do with this right now."

Freeze uses the outer orbit and colder visual treatment.

Park uses depth, distance, size, softness, and blur.

This allows task state to communicate different forms of postponement without relying on conventional status labels.

---

## 8. No-Guilt Productivity

Orbit intentionally avoids mechanics that turn productivity into a measure of personal success or failure.

There are no:

* Streaks
* Productivity scores
* Shame messages
* Red overdue warnings
* Endless task counters
* Punitive visual effects

The system is designed around acceptance of fluctuating capacity.

---

## 9. Persistent Task Identity

Every task has a unique persistent identity independent of:

* Card position
* Animation order
* Array index
* Visual position

For example:

```text
voice-session-1
    │
    ├── multimedia-assignment
    ├── reply-team-email
    ├── review-design-feedback
    └── prepare-weekly-notes
```

A task must remain the same task when moving between states.

For example:

```text
ACTIVE → BACKGROUND → ACTIVE
```

must return the exact same task.

Similarly:

```text
ACTIVE → FROZEN → ACTIVE
```

must preserve the same task identity.

---

## Comparison With Conventional Productivity Tools

| Dimension             | Conventional Productivity Tools            | Orbit                             |
| --------------------- | ------------------------------------------ | --------------------------------- |
| Starting point        | Task list / dashboard                      | Capacity Check                    |
| Workload presentation | Generally fixed                            | Capacity-responsive               |
| Task creation         | Manual entry                               | Voice brain dump + manual input   |
| Focus                 | Multiple visible tasks                     | One active task                   |
| Large tasks           | User manually breaks them down             | Chunk interaction                 |
| Postponement          | Status / due date                          | Freeze / Park                     |
| Completion            | Checkbox / button                          | Directional gesture               |
| Visual feedback       | Dashboard / list                           | Cosmic environment                |
| Motivation            | Streaks / productivity metrics may be used | No-guilt design                   |
| Recovery              | Usually separate                           | Integrated optional Recovery Mode |

---

# 5. Technical Architecture & Feasibility

## Tech Stack

| Layer                        | Technology                                  | Why It Fits                                                                                                                                        |
| ---------------------------- | ------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Frontend**                 | React Native / Expo                         | Suitable for building a mobile prototype and implementing gesture-driven interactions.                                                             |
| **Backend**                  | Spring Boot / Java                          | Provides a structured backend/API layer for task management and application logic.                                                                 |
| **Database**                 | PostgreSQL / Supabase                       | Provides persistent storage for task objects and their states.                                                                                     |
| **AI / Task Interpretation** | [INSERT ACTUAL AI SERVICE / IMPLEMENTATION] | Used to interpret natural-language brain dumps into structured tasks. If the prototype uses hardcoded deterministic data, state that clearly here. |
| **Hosting / Deployment**     | [INSERT ACTUAL HOSTING]                     | [INSERT WHY THIS SERVICE WAS CHOSEN / CONSTRAINTS]                                                                                                 |

> **Important:** Only list technologies and services that the team actually uses or plans to use. Replace all placeholders before submission.

---

## System Architecture Diagram

**Architecture Diagram:**
[INSERT FIGMA / LUCIDCHART SYSTEM ARCHITECTURE LINK]

### High-Level Architecture

```text
┌──────────────────────────────┐
│       Orbit Mobile App      │
│    React Native / Expo      │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│       Spring Boot API       │
│            Java             │
└──────────────┬───────────────┘
               │
       ┌───────┴────────┐
       │                │
       ▼                ▼
┌───────────────┐  ┌─────────────────────┐
│ Task & State  │  │ Task Interpretation │
│    Logic      │  │ [ACTUAL METHOD]     │
└───────┬───────┘  └─────────────────────┘
        │
        ▼
┌──────────────────────────────┐
│     PostgreSQL / Supabase   │
└──────────────────────────────┘
```

[REPLACE OR SUPPLEMENT THIS WITH THE FINAL ARCHITECTURE DIAGRAM]

---

## Task State Lifecycle

**Task State Lifecycle Diagram:**
[INSERT LUCIDCHART / DRAW.IO LINK]

Orbit separates task identity from task state.

### Core States

* **Active**
* **Parked / Background**
* **Frozen**
* **Chunked**
* **Completed**
* **Deleted**

Conceptual flow:

```text
                         ┌──────────────┐
                         │    ACTIVE    │
                         └──────┬───────┘
                                │
             ┌──────────────────┼──────────────────┐
             │                  │                  │
             ▼                  ▼                  ▼
        COMPLETED            FROZEN              CHUNKED
             │                  │                  │
             │                  ▼                  ▼
             │                ACTIVE        SMALLER TASKS
             │
             ▼
          END

ACTIVE ───────────────► PARKED / BACKGROUND
                              │
                              ▼
                            ACTIVE

ACTIVE ───────────────► DELETED
```

The same task ID must be preserved when a task moves between states.

---

## Database Schema

**ERD:**
[INSERT DBdiagram.io LINK]

### Conceptual Task Object

```text
Task
├── id
├── title
├── duration
├── deadline
├── category
├── state
├── parentTaskId
├── created_at
└── updated_at
```

The exact database fields should reflect the team's actual implementation.

### Task Identity

Task identity must not depend on:

* Card position
* Array index
* Animation order
* Visual position

This prevents state transitions from accidentally displaying the wrong task.

---

## Task Categories

Orbit uses five task categories:

* **Academic**
* **Chores**
* **Financial**
* **Social**
* **Errands**

The category describes:

> **What area of life is this task from?**

Task state describes:

> **Where is this task in my attention space?**

These are separate concepts.

Categories can be represented subtly through the cosmic environment rather than conventional colourful category labels.

---

## Voice-to-Task Architecture

The intended interaction is:

```text
User Brain Dump
       │
       ▼
   LISTENING
       │
       ▼
   PROCESSING
       │
       ▼
     GOT IT
       │
       ▼
Structured Task Objects
       │
       ▼
One Active Task
       │
       ▼
Gesture / Action
       │
       ▼
Updated Task State
```

### Prototype AI Approach

The prototype may use deterministic/hardcoded data behind the scenes.

This is acceptable for demonstrating the concept as long as the interaction correctly communicates:

> **"I told the app what I needed to do, and the AI understood and created my tasks."**

The prototype should not imply that a production-grade speech-recognition or AI system has been implemented if it has not.

---

## Technical Feasibility

Orbit is intentionally scoped around a narrow vertical slice:

> **Input → Interpretation → Task Creation → Task State → Interaction → Updated State**

The core system does not require every future productivity integration to demonstrate its central value.

### Core Vertical Slice

```text
Capacity Check
      ↓
Adaptive Environment
      ↓
Voice Brain Dump
      ↓
Task Interpretation
      ↓
Task Creation
      ↓
One Active Task
      ↓
Gesture
      ↓
Updated Task State
```

This allows the team to focus implementation effort on the most visible and important part of the product.

---

## Reliability & Demo Fallback

The prototype should remain demonstrable even if an external AI/API dependency is unavailable.

Potential fallback mechanisms include:

* Deterministic task data
* Prepared demo inputs
* Seeded task objects
* Local/cached prototype outputs
* Recorded backup demonstration
* Screenshots of completed flows

The core product story should remain functional without depending entirely on live external services.

---

## Validation & Testing

### Capacity

* [ ] Capacity Check works.
* [ ] Different capacity selections produce the intended visual response.
* [ ] Low capacity does not prevent the user from continuing.
* [ ] Gentle Mode adapts the experience without locking the user out.

### Voice Input

* [ ] Long press activates Listening.
* [ ] Normal tap does not accidentally create a task.
* [ ] Short drag does not accidentally trigger voice input.
* [ ] Listening state is clearly visible.
* [ ] Processing state is clearly visible.
* [ ] "Got It" state appears before task creation.
* [ ] Multiple tasks can be produced from one voice interaction.

### Task Identity

* [ ] Every task has a unique ID.
* [ ] Task identity does not depend on array index.
* [ ] Task identity does not depend on visual position.
* [ ] Frozen tasks return as the same task.
* [ ] Parked tasks return as the same task.
* [ ] Chunked tasks retain their parent relationship.

### Gestures

* [ ] Right → Done
* [ ] Left → Freeze
* [ ] Up → Chunk
* [ ] Down → Delete
* [ ] Failed/short swipes return the card to the center.
* [ ] Gestures do not trigger unintended actions.

### Recovery

* [ ] Recovery Mode can be entered.
* [ ] 2:00 countdown works.
* [ ] Recovery visualization works.
* [ ] Task gestures are disabled during Recovery Mode.
* [ ] The app returns to the task environment after 0:00.
* [ ] Tasks are not reset after recovery.

---

## Ethics, Safety & User Boundaries

Orbit is a **stress and workload management application**, not a medical or mental-health diagnostic system.

The project therefore follows these boundaries:

* Capacity is self-reported.
* Energy Ripple is symbolic rather than scientific.
* Orbit does not diagnose users.
* Orbit does not claim to treat mental-health conditions.
* Low capacity does not lock the user out of the application.
* Recovery Mode is optional.
* The product avoids shame-based productivity mechanics.
* External API keys and credentials must not be exposed in the public repository.
* Any AI/API dependency should have a reasonable demonstration fallback.

---

## Build Plan & Scope

The team prioritizes a realistic vertical slice rather than attempting to implement every possible future feature.

### Priority 1 — Core Product Loop

**Capacity Check**

↓

**Capacity-Adaptive Environment**

↓

**Voice Brain Dump**

↓

**Task Interpretation**

↓

**One Active Task**

↓

**Gesture-Based Task Management**

↓

**Updated Task State**

### Priority 2 — Supporting Features

* Gentle Mode
* Empty Task Space
* Manual Task Input
* Park / Background
* Freeze
* Chunk
* Recovery Mode
* Completed state
* Persistent task identity

### Prototype Scope

The prototype will focus on:

* Capacity Check
* Gentle Mode
* Empty Task Environment
* Voice-based brain dump interaction
* Deterministic/hardcoded task interpretation where required
* One-by-one task display
* Four directional gestures
* Task Space
* Manual input
* Recovery Mode
* Completed task state
* Persistent task identity and state transitions

### Out of Scope for the Prototype

The following are future possibilities rather than requirements for the current prototype:

* Full production speech recognition
* Advanced autonomous AI planning
* Calendar synchronization
* Email synchronization
* Background synchronization
* Large-scale notification infrastructure
* Medical/mental-health assessment
* Scientific stress measurement

Keeping these features outside the initial scope allows the team to concentrate on delivering a reliable and demonstrable core experience.

---

## Future Development

Once the core product loop is validated, Orbit could be extended with:

* Real speech recognition
* More advanced AI task decomposition
* Calendar integration
* Email integration
* Background synchronization
* Persistent user accounts
* More sophisticated workload planning
* Additional accessibility features
* Cloud-based task persistence
* More personalized workload adaptation

The fundamental product boundary remains:

> **Help users make their workload feel manageable according to their available capacity.**

---

# Project Resources

The following resources provide supporting evidence and materials for the project.

### Design & Ideation

**FigJam Brainstorming:**
[INSERT FIGJAM LINK]

**Figma Prototype:**
[INSERT FIGMA LINK]

### Presentation

**YouTube Demo / Presentation:**
[INSERT YOUTUBE LINK]

**Canva Pitch Deck:**
[INSERT CANVA LINK]

### Technical Diagrams

**Task State Lifecycle:**
[INSERT LUCIDCHART / DRAW.IO LINK]

**Database ERD:**
[INSERT DBdiagram.io LINK]

**System Architecture:**
[INSERT FIGMA / LUCIDCHART LINK]

### Documentation

**Google Docs — Project Documentation:**
[INSERT GOOGLE DOCS LINK]

**Additional Documentation:**
[INSERT LINK IF APPLICABLE]

### Repository

**GitHub Repository:**
[INSERT PUBLIC GITHUB REPOSITORY LINK]

---

# Final Product Philosophy

Orbit is built around one simple principle:

> ## **When you have less capacity, we ask less of you.**

The goal is not to make users complete more tasks at any cost.

The goal is to help users understand:

**What can I handle right now?**

and then make that workload feel possible.

> **Tell me what you need to handle. I'll help make the load manageable.**
