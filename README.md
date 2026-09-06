# Orbit by Banana404

**Team:** Yow Jia Yen, Goh Ching Yee, Victoria Kew Kim Tian, Yong Zi Yan
**Problem Statement:** Lifestyle Track: Beating the Burnout - Stress & Workload Manager

**Video Presentation:** [YouTube Link](#) 
*Brief Explanation:* A video presentation demonstrating the core cosmic task environment, voice input interaction, and the fluid task gestures (Done, Freeze, Chunk, Delete).

**Presentation Slides:** [Canva Link](#)
*Brief Explanation:* Our pitch deck outlining the problem of productivity burnout, introducing our philosophy "When you have less capacity, we ask less of you," and visualizing the adaptive UI.

---

## 1. Project Overview

**The Problem**
Traditional productivity apps attempt to maximize output, which frequently leads to burnout and anxiety for stakeholders like students and professionals. Similar apps in the market (e.g., Todoist, Notion, or standard calendar apps) fall short because they rely on conventional dashboards, infinite scrolling lists, and guilt-driven mechanics like red overdue text and streaks. They do not account for a user's fluctuating daily mental capacity.

**Our Solution**
Orbit is a stress-aware task management experience designed around a quiet, cosmic notebook interface. It explicitly adapts the volume and difficulty of tasks presented to the user based on a daily capacity check. Core features include a gesture-based task card system (Right: Done, Left: Freeze, Up: Chunk, Down: Delete), a voice-to-task AI interpreter that breaks down brain-dumps into single tasks, and a dynamic visual environment where elements like the "energy ripple" and star brightness shift with your daily load.

---

## 2. Ideation & Process

### 2.1 Ideas We Considered

| Idea | Why it was dropped / kept |
| :--- | :--- |
| **A (Chosen): Adaptive Load Manager with Cosmic UI** | Kept because it inherently solves the pressure of traditional task lists by matching UI elements (stars, ripples) to user capacity, communicating a forgiving environment. |
| **B (Chosen): Voice-based multi-task input** | Kept because it significantly lowers task-entry friction. Users can brain-dump tasks while the AI automatically parses them into manageable cards. |
| **C: Gamified Productivity Tracker with Streaks** | Dropped because it introduces guilt mechanics and pressure to maintain streaks, which completely contradicts our core "no guilt" philosophy. |

### 2.2 Ideation Boards

* **[Figjam link for brainstorming](#):** Affinity diagrams mapping out stress triggers in standard productivity apps and brainstorming the "cosmic" visual identity (stars, dark backgrounds, organic outlines).
* **[Draw.io link for technical flowchart diagram](#):** Flowchart illustrating the state logic for tasks (Active, Parked, Frozen, Done, Deleted) ensuring task IDs remain stable across transitions, and detailing the Voice-to-AI processing pipeline.
* **[Figma storyboard](#):** User flow sequences documenting the crucial "Open App -> Capacity Check -> Empty Task Space -> Long Press Voice Input" journey.

### 2.3 Mentor Consultation

| Date | Mentor | Feedback Received | What Was Changed |
| :--- | :--- | :--- | :--- |
| May 2026 | UI/UX Mentor | The initial interface feels too much like a standard dashboard with menus. | We removed the traditional bottom navigation, hamburger menu, and floating "+" button, replacing the interface entirely with an empty cosmic space and a long-press voice input mechanism. |

---

## 3. Design & Prototype

**UI Prototype:** [Figma prototype](#)
*Brief Explanation:* A clickable high-fidelity prototype showcasing the dark midnight/charcoal environment, the daily capacity slider (0-100%), and physical card gestures. 

**Key Screens & Interactions:**
1. **Capacity Check Screen:** The app asks, "Good morning. How much can you handle today?" with a visual face/emoji scale and slider. It avoids scoring and instead offers gentle interpretations like "Let's take it easy."
2. **Empty Task Environment:** A quiet cosmic space waiting for intentional input. There are no placeholder cards or fake tasks; the user must long-press to initiate the "Listening..." state.
3. **Task Chunking (UP Gesture):** Dragging a task card UP physically cracks/splits the large task into two smaller, more manageable task cards (e.g., splitting "Finish Multimedia Assignment" into two smaller steps).
4. **Recovery Mode:** Triggered when capacity is low. It initiates a 2:00 minute countdown with a breathing star visualization to encourage the user to step away and recharge before returning to the task environment.

---

## 4. What Makes It Different

* **No Guilt Mechanics:** Orbit strictly avoids streaks, productivity scores, red overdue warnings, and endless task counters. 
* **Dynamic, Emotion-Responsive Environment:** The visual atmosphere (brightness, animation speed, energy ripple size) changes dynamically based on the user's declared capacity, shifting into "Gentle Mode" when capacity is low.
* **Physical Interaction:** Tasks are manipulated via direction-based physical gestures (Chunk, Freeze, Delete) instead of traditional checkboxes, giving a tactile sense of clearing one's plate.
* **One Task at a Time:** There is no conventional list or dashboard. Only one active task card is presented in the center at a time, preserving focus and preventing visual overwhelm.

---

## 5. Technical Architecture & Feasibility

**Tech Stack**
* **Frontend:** React Native / Expo. Chosen to support Orbit’s fluid directional gestures (Right = Done, Left = Freeze, Up = Chunk, Down = Delete), interactive task cards, Task Space navigation, and custom animations such as card cracking, orbital movement, meteor transitions, and energy ripples across mobile platforms.
* **Backend:** Spring Boot (Java). Chosen based on our team's existing familiarity with Java, AI model integration (such as Z.ai GLM-5.1), and external APIs. The backend architecture provides a foundation for future AI-powered task parsing and adaptive workload features.
* **Database / Architecture:** PostgreSQL via Supabase. Chosen for its simple setup and suitability for storing persistent task data and states. Each task is assigned a unique ID so that tasks can safely move between Active, Parked, Frozen, Chunked, Completed, and Deleted states without losing their identity. 
* **Links:** 
  * **[Github link](#):** Repository for version control and collaborative code integration.
  * **[dbdiagram link for data api flow diagram](#):** Explains the schema ensuring unique task IDs map accurately to their respective states (active, frozen, background) independently of UI array indices.
  * **[Google docs link for timeline, reports, summary and calendar](#):** Project management hub tracking development milestones and sprint summaries.
  * **[Google docs link for all the meeting notes](#):** Log of team standups, decision-making rationales, and action items.

**Build Plan & Scope**
FFor the submission phase, we will focus on delivering the core Orbit interaction loop: the Capacity Check screen, adaptive Gentle Mode, the empty task environment, voice-based brain dump processing (using hardcoded data to simulate AI natural-language task parsing), one-by-one task display, the four main directional gestures, Task Space for viewing and switching between tasks, manual task input, Recovery Mode, and the completed-task state. AI processing, passive load detection, calendar/email integrations, and complex background synchronization will be scoped out of the initial build. This keeps the prototype technically realistic while allowing us to focus on the distinctive interaction between user capacity, task states, and gesture-based workload management.
