# Orbit by Team Banana404

**Team:** Victoria Kew Kim Tian, Yow Jia Yen, Yong Zi Yan, Goh Ching Yee  
**Problem Statement:** Stress & Workload Manager  
**Video Presentation:** [Unlisted Youtube Link]  
**Presentation Slides:** [Public Link]  

---

## 1. Project Overview

**The Problem.** University students juggle immense cumulative loads across their academic and personal schedules without knowing they are heading toward a crash. Traditional time-management and checklist tools merely track time, treating all tasks equally and waiting until the student crashes to reflect the overload. Existing apps fall short because they add cognitive and administrative friction, such as rigid planners, complex dashboards, or punitive streak counters, that actually increase a student's mental load.

**Our Solution.** Orbit is an adaptive workload manager that protects the user's mental bandwidth[cite: 2]. Built on the core philosophy that "When you have less capacity, we ask less of you," Orbit shifts from traditional rigid tracking to dynamic capacity management[cite: 2]. Utilizing a minimalist, calm visual hierarchy featuring a dark cosmic background and hand-drawn paper task cards, Orbit allows users to report their daily capacity via a horizontal slider[cite: 2]. The system automatically adapts task presentation so the user is never confronted with their entire workload at once[cite: 2].

*   **Daily Capacity Check-in:** A horizontal slider on Screen 1 used exclusively for self-reported daily capacity, scaling animation speed, background brightness, and task difficulty[cite: 2].
*   **Single-Card Task Deck (Screen 2):** Displays only ONE task card at a time to prevent cognitive overload[cite: 2].
*   **Four Core Gesture Mechanics:** Intuitive swipe controls on the card: Right for Done (meteor animation), Left for Freeze (safe storage), Up for Chunk (simplifying large tasks), and Down for Delete (cosmic void)[cite: 2].
*   **Physical Undo System:** Opposite-direction drag to easily pull a card back into orbit[cite: 2].
*   **Voice Task Creation:** Long-press anywhere on the task deck to activate a clean listening and AI processing state without a microphone button[cite: 2].
*   **Gentle Mode & Quiet Protection:** Automatic scaling when capacity is extremely low, paired with anti-spam notification protection that never punishes the user for being away[cite: 2].

---

## 2. Ideation & Process

### 2.1 Ideas We Considered

| Idea | Why it was dropped / kept |
| :--- | :--- |
| **A. Adaptive Single-Card Workload Manager ("Orbit")** | **Kept:** Solves burnout by replacing intimidating dashboards with a single-card deck and gesture-based interactions that automatically scale down when user capacity drops[cite: 2]. |
| **B. Hand-Drawn Cosmic & Sketch Aesthetic** | **Kept:** Replaces high-stress corporate productivity apps with a calming interface (dark cosmic background, hand-drawn lines, paper-like cards) that feels like a quiet notebook[cite: 2]. |
| **C. Traditional Dashboard Checklists & Streaks** | **Dropped:** Adds pressure and guilt via red badges, streaks, and score tracking, which our research showed accelerates student burnout[cite: 2]. |

### 2.2 Ideation Boards
*   **Central Workspace & Documentation:** CodeNection 2026_Banana 404 | Project Buffer Space (including Confluence pages for *5.9.2026 1st meeting*, *10.9.2026 Mentor Consultation*, *Project Overview & Impact*, *Technical Architecture & API Strategy*, *Accessibility & UX Guidelines*, and *Ideation & Pivot Log*)[cite: 3].
*   **Multilayered Problem Tree & Planning:** [Insert FigJam Link] - Problem mapping and interaction workflows.
*   **Database Schema Mapping:** [Insert dbdiagram.io Link] - Visualizing Firebase Firestore NoSQL schema structures, capacity logs, and triage events[cite: 3].

> *Fig. 1: Multilayered problem tree mapping out student cognitive overload triggers and the design rules for zero-punishment task management.*

### 2.3 Mentor Consultation

| Date | Mentor | Feedback Received | What Was Changed |
| :--- | :--- | :--- | :--- |
| Sep 10, 2026 | Looi Wei En[cite: 3] | Advised streamlining gesture responsiveness in Figma prototypes and validating interaction boundaries early. | Refined prototype rules to ensure the horizontal slider and card swipe areas do not conflict, keeping gesture triggers strictly separated[cite: 2]. |

---

## 3. Design & Prototype

**UI Prototype:** [Public Link]  
*Check that it opens in an incognito window. Features the Daily Capacity Check-in, Single-Card Deck, 4-way swipe mechanics, voice long-press simulation, and Gentle Mode states[cite: 2].*

> *Embedded key prototype views demonstrating the transition from the Daily Capacity Check slider (Screen 1) to the Single-Card Task Deck (Screen 2) and gesture responses[cite: 2].*

---

## 4. What Makes It Different

*   **Active Bandwidth Adaptation:** Unlike traditional task apps that display an unyielding backlog, Orbit actively shrinks task demands based on user-reported capacity ("When you have less capacity, we ask less of you")[cite: 2].
*   **Gesture-First, Zero-Button Interface:** Eliminates traditional UI clutter (no bottom navigation, hamburger menus, floating action buttons, or checkboxes) in favor of physical card manipulation[cite: 2].
*   **Guilt-Free Protection:** Completely avoids streaks, score trackers, and shame language, introducing "Quiet Protection" and "Soft Landing" screens that never punish users for having low capacity or stepping away[cite: 2].

---

## 5. Technical Architecture & Feasibility

**Tech Stack:**
*   **Frontend:** Cross-platform mobile framework (React Native / Flutter) optimized for smooth gesture physics and transition animations. Chosen for rapid prototyping and fluid gesture responsiveness.
*   **Backend:** Spring Boot / Firebase backend for secure handling of capacity logs and user data state.
*   **Database:** Firebase Firestore (NoSQL schema structured via dbdiagram.io for capacity logging and triage/task events)[cite: 3].
*   **APIs & Services:** OpenAI API for processing voice input transcripts into structured task cards, alongside calendar API integration for contextual task scheduling[cite: 1, 3].

**System Architecture Diagram:** [Insert Draw.io Link] and [Insert dbdiagram.io Link]  
*Complete backend system flow mapping from mobile UI actions to AI processing, database logging, and relational/NoSQL entity relationship mapping[cite: 3].*

**Build Plan & Scope:**
*   Focus strictly on implementing the core Orbit interaction loop consistently (Capacity Check $\rightarrow$ Single Card $\rightarrow$ Gesture Actions $\rightarrow$ Adaptive States) without scope creep[cite: 2].
*   Ensure prototype triggers are accurately bound to prevent accidental gesture overlapping, such as separating the horizontal slider from the vertical upward transition[cite: 2]. Narrow scope reads as realistic and feasible rather than a lack of ambition.
