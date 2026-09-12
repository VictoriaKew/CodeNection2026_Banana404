ORBIT by Banana 404

Team: Yow Jia Yen, Victoria Kew Kim Tian, Goh Ching Yee, Yong Zi Yan
Problem Statement: Stress & Workload Manager
Video Presentation: [Insert final unlisted YouTube link]
Presentation Slides: [Insert public Canva link]

1. Project Overview

The Problem

University students often have to manage assignments, deadlines, emails, classes, errands, social commitments, and personal responsibilities at the same time.
However, a student’s capacity is not constant.
The same workload can feel manageable on one day and overwhelming on another. Traditional productivity applications usually continue presenting the same lists, reminders, priorities, and deadlines regardless of how much the user can realistically handle.
This can create another layer of cognitive overhead for students who are already overwhelmed.
Orbit focuses on a more specific group: students who struggle with complex workloads, maintaining focus, and organising multiple responsibilities at once.
This is especially relevant to users who experience difficulties commonly associated with inattention, such as forgetfulness, losing track of tasks, difficulty organising responsibilities, and trouble maintaining focus. Orbit does not diagnose or treat ADHD or any other medical condition; the app focuses on workload and interaction design.

Existing Approach

Conventional task-management applications are useful for recording and organising tasks, but their core model is generally:
User → adapts to workload
Orbit explores the opposite approach:
Workload → adapts to user
The key insight is that the problem is not always having too much work. Sometimes the workload simply does not match the user’s current capacity.

Our Solution

Orbit is a stress and workload management mobile application built around one central principle:
When you have less capacity, we ask less of you.
Instead of immediately presenting a large task list, Orbit first asks the user how much they can handle today. The user’s reported capacity influences the workload experience and visual environment.
Users can then perform a natural-language brain dump, allowing multiple responsibilities to be converted into individual tasks. Instead of managing a long list, users interact with one active card at a time through simple physical gestures.
Orbit is designed to make workload feel possible, rather than simply pushing users to become more productive.

Core Features

Capacity Check

Capacity-Adaptive Environment

Gentle Mode

Voice Brain Dump

AI Task Interpretation

One Active Card

Gesture-Based Task Management

Task Chunking

Freeze

Park

Delete

Recovery Mode

No-Guilt Productivity

Capacity Model

Capacity

Orbit Response

0–20%

Recovery

20–40%

Gentle Mode

>40%

Normal Mode

Capacity is not a difficulty setting. A low-capacity user is never locked out from completing difficult work. Instead, Orbit changes how the workload is presented.

2. Ideation & Process

2.1 Ideas We Considered

The team initially explored the problem from the perspective of productivity and stress management. Through ideation and mentor feedback, we gradually narrowed the concept towards capacity-aware workload management.

Idea

Why it was kept / dropped

Adaptive Workload Manager

Chosen. Became the main concept because it directly addresses the difference between workload and changing user capacity.

Capacity Check

Chosen. Gives Orbit an input that conventional task managers generally do not consider: how much the user can handle today.

One Active Card

Chosen. Reduces the cognitive load of seeing many unfinished tasks at once.

Voice Brain Dump

Chosen. Allows users to describe multiple responsibilities naturally instead of manually organising them first.

Task Chunking

Chosen. Allows overwhelming tasks to be transformed into smaller, more approachable actions.

Gesture-Based Interaction

Chosen. Makes task management physical and simple instead of relying on menus and multiple navigation screens.

Recovery Mode

Chosen. Recognises that sometimes the appropriate response to low capacity is recovery rather than more productivity.

Cosmic Interface

Chosen. Provides a visual language for capacity and task states while making Orbit distinct from conventional productivity dashboards.

Traditional Dashboard

Dropped. The team felt that a dashboard containing many lists and metrics could create additional cognitive overhead.

Bottom Navigation

Dropped. The team interpreted the mentor’s emphasis on simplicity and reduced cognitive overhead as a reason to remove unnecessary navigation from the core interaction.

Hamburger Menu

Dropped. Removed unnecessary navigation complexity.

Floating “+” Button

Dropped. The team chose long-press interaction instead to make task creation part of Orbit’s physical interaction model.

Priority System

Deprioritised. Prioritisation tells users what is important, but does not necessarily account for their current capacity.

Streaks / Gamification

Dropped. These mechanics conflicted with Orbit’s no-guilt approach.

Heavy Notifications

Dropped. Additional reminders could become another source of cognitive overload.

Calendar / LMS / Email Integration

Future implementation. Potentially useful for understanding a user’s wider workload, but outside the current prototype scope.

How Our Idea Evolved

The team’s direction can be summarised as:
We started with Productivity. We ended with Capacity.
The key decision was to stop asking:
“How do we help students complete more?”
and instead ask:
“How can we make the workload feel manageable?”
This shift led to the current combination of capacity awareness, adaptive workload, one active card, physical interaction, and recovery.

2.2 Ideation Boards

FigJam Brainstorming Board

[Insert FigJam Brainstorming Board Link]
The brainstorming board documents the team’s exploration of:

Student stress and workload

Existing productivity approaches

Target users

Adaptive workload concepts

Voice input

Task chunking

Gesture interaction

Cosmic UI

Features that were retained

Features that were dropped

Storyboard

[Insert Figma Storyboard Link]
The storyboard illustrates the user’s experience and helped the team visualise how Orbit should move from the initial capacity check into the workload environment.

UI Design

[Insert Figma UI Design Link]
The UI exploration helped the team move away from a conventional productivity dashboard towards a more minimal and spatial interaction model.

System & User Flow Diagrams

[Insert Orbit Diagram Link]
The overview and in depth diagrams help illustrate how Orbit moves from the user’s initial capacity check through task creation, task interaction, and recovery.

2.3 Mentor Consultation

Date：10 September 2026 - 8:25pm
Mentor：Looi Wei En

UI/UX Mentor Consultation

The team consulted a UI/UX mentor to review the concept, user experience, and presentation of Orbit. The discussion focused mainly on clarifying the problem, narrowing the target users, simplifying the experience, and making Orbit's concept and interaction model more distinctive.
The mentor feedback led to several important changes:

Feedback

What Was Changed

Define who Orbit is designed for instead of trying to address every type of student stress or workload.

Narrowed the target audience to students who experience difficulty managing complex workloads and too many things at once.

The team was encouraged to look at current productivity applications and consider how their features and interfaces can become complicated for users who already have many things to manage

Simplified the interface by removing unnecessary productivity-app conventions and focusing only on the core interactions needed to manage workload.

The presentation should make it immediately understandable what Orbit does, rather than spending too much time explaining individual UI elements.

Redesigned the main experience around a clear, empty task environment where the purpose and next action are easier to understand.

Briefly show the different ideas explored and explain which ideas were kept and which were removed as the concept became more focused.

Removed features that added unnecessary management, such as dashboards, excessive navigation, and conventional task-management elements, and kept the core ideas of capacity, adaptive workload, attention control, and recovery.

Need to be clearly communicate how Orbit differs from conventional productivity applications, particularly in the way it represents and handles workload.

Introduced a spatial interaction model where tasks are represented through the environment: active tasks stay at the center, parked tasks move into the background, and frozen tasks move to the outer orbit

How the Feedback Influenced Orbit

The consultation helped the team refine Orbit from a broader productivity concept into a more focused experience centered around simplicity, capacity, and reduced cognitive overhead.
Rather than presenting students with another system that requires them to organize and manage everything, the team focused on creating an interaction where users can tell Orbit what they need to handle and move through the workload one step at a time.
This also influenced the team's decision to prioritize the Figma storyboard and core interaction flow in the presentation, while keeping detailed technical diagrams and supporting information in GitHub.
The overall direction became:
Less to manage. Less to organize. One step at a time.

10 September 2026 Mentor / Team Discussion

The discussion further focused on whether Orbit’s main idea was clear enough, how to avoid making it feel like another common productivity application, and how to communicate the concept effectively within a short presentation.
Key directions from the discussion were:

Clearly explain the app concept and target problem.

Show the Figma storyboard/UI rather than spending too much time explaining every design detail.

Make the target group more specific instead of trying to solve every form of stress.

Research existing applications and explain where conventional approaches become too complicated.

Highlight simplicity and reduced cognitive overhead.

Show all major ideas considered and explain what the team decided to let go.

Focus the presentation on how Orbit works and why its interaction is different.

Explain the main flow in approximately two minutes.

Include the detailed diagrams in GitHub, while only briefly showing the simplified version during the presentation.

Consider how the workload should be visually represented rather than relying on a conventional task list.

The discussion reinforced the team’s decision to focus the product around simplicity, capacity, and one-step-at-a-time interaction.

3. Design & Prototype

UI Prototype

Published Prototype:
[Insert published Figma prototype link]
The prototype demonstrates Orbit’s main product loop rather than attempting to implement every future feature.

Key Screens

1. Capacity Check

The experience begins with:
“Good morning. How much can you handle today?”
The user selects their current capacity.
The capacity determines how Orbit presents the workload.

2. Empty Task Environment

After setting capacity, the user enters Orbit’s main environment.
The center is intentionally empty.
There is:

No conventional task list

No automatically displayed task

No large Continue button

No floating “+” button

No dashboard

Instead, Orbit waits for the user to tell it what they need to handle.
This is an important part of the concept because the user should feel that they are initiating the workload rather than being immediately presented with another list to manage.

3. Voice Brain Dump

The user long-presses the environment.
Orbit enters:
“Listening…”
The user can naturally say multiple responsibilities in one interaction.
For example:
“I need to finish my multimedia assignment, reply to the team email, review the design feedback, and prepare my weekly notes.”
One voice interaction can therefore become multiple structured tasks.

4. AI Processing

After the user releases the long press, Orbit shows:
Listening → Processing → Got It
For the current prototype, the AI behaviour can be simulated where required.
This allows the demonstration to show the intended transformation without depending entirely on live AI services.

5. One Active Card

After processing, Orbit presents one active task card at a time.
The active card becomes the user’s immediate focus.
Other tasks remain in the surrounding environment instead of being displayed as a long conventional list.
One card. One decision. One step at a time.

6. Gesture Interaction

The user manages the active card through four directional gestures, while Park provides a separate spatial way to move a task into the background.

Interaction

Action

Meaning

→

Done

“I’m finished.”

←

Freeze

“Not now.”

↑

Chunk

“Make this smaller.”

↓

Delete

“I don’t need it.”

Long press

Move to background / Park

”I don’t know what to do with this yet”

The interaction makes task management more physical and reduces the need for multiple menus.

7. Chunking

A large task can be made smaller.
For example:
Finish Multimedia Assignment
becomes:

Open the assignment brief

Identify the 3 sections to complete

The goal is to change:
“This is too much.”
into:
“I can start with this.”

8. Freeze & Park

Orbit gives postponement two different meanings.
Freeze
“Not now.”
The task moves into the colder outer orbit.
Park
“I don’t know what to do with this right now.”
The task moves into the background and becomes smaller, dimmer, and less visually demanding.
This distinction allows task state to be communicated spatially instead of relying only on labels.

9. Recovery

When the user’s capacity is very low, Orbit enter a recovery mode:
“2 MIN RESET”
The recovery experience does not delete or reset tasks.
Instead, it gives the user a short pause before returning to the workload.
Recovery is an invitation, not a punishment or failure.

4. What Makes It Different

Orbit is not simply a conventional task manager with a cosmic theme.
Its main difference is that capacity becomes part of the workload-management experience.

1. Capacity Comes First

Traditional productivity asks:
“What do I need to finish?”
Orbit asks:
“What can I realistically handle right now?”
The answer influences the workload experience.

2. One Active Card

Instead of presenting every responsibility at once:
One card → one decision → one step
This reduces the immediate amount of information competing for the user’s attention.

3. The Workload Can Change Size

Orbit does not only organise tasks.
It can change how a task is approached.
A large task can be transformed into smaller actions through Chunk.

4. Physical Interaction

Done, Freeze, Chunk, and Delete are represented through directional gestures.
This reduces administrative interaction and makes the task itself the main interface.

5. Voice Before Organisation

Users can first dump their thoughts naturally and let Orbit structure them afterwards.
This creates:
Unstructured thoughts → structured tasks → manageable actions

6. The Environment Communicates State

The cosmic environment is functional rather than purely decorative.
Elements such as:

Energy ripple

Star brightness

Visual movement

Spatial distance

Orbit depth

can communicate changes in capacity and task state.

7. No-Guilt Productivity

Orbit intentionally avoids:

Streaks

Productivity scores

Shame messages

Punitive overdue warnings

Aggressive notifications

Endless task counters

The user is allowed to have limited capacity.

5. Technical Architecture & Feasibility

Tech Stack

Frontend — React Native / Expo

Used for:

Mobile interface

Cosmic environment

Task cards

Gesture interactions

Animations

Capacity experience

Backend — Spring Boot / Java

Responsible for:

Task logic

Capacity logic

Task state transitions

Recovery logic

API endpoints

Database — PostgreSQL / Supabase

Planned for storing:

Users

Tasks

Task states

Capacity information

Recovery sessions

AI / Speech Services

Planned processing flow:
Voice Input → Speech Recognition → AI Task Interpretation → Structured Tasks
The prototype can use simulated/deterministic AI responses where necessary.

Architecture

React Native / Expo
↓
Spring Boot / Java
↓
PostgreSQL / Supabase
↓
AI / Speech Services
The architecture separates the mobile interface, application logic, persistent data, and external AI services.
The technical direction is intended to support the transition from the current prototype into a real product.

Build Plan & Scope

The team will focus on a realistic vertical slice instead of attempting to implement every possible future feature.

Core Product Loop

Capacity Check
↓
Capacity-Adaptive Environment
↓
Voice Brain Dump
↓
Task Interpretation
↓
One Active Card
↓
Gesture Interaction
↓
Updated Task State

Prototype Scope

The building phase will focus on:

Capacity Check

Capacity-adaptive environment

Gentle Mode

Empty task environment

Voice brain dump interaction

Simulated/deterministic AI task interpretation

One active task at a time

Four directional gestures

Task chunking

Freeze

Park

Delete

Completed state

Recovery Mode

Persistent task identity and state transitions

Current Limitations

Simulated AI — the prototype may not use a fully production-ready AI service.

Self-Reported Capacity — capacity is currently provided by the user rather than automatically measured.

No Personalisation — Orbit does not yet learn an individual’s workload patterns.

Early Validation — further testing is required with real users.

Orbit is a workload-management concept, not a medical or mental-health diagnostic system. Capacity is self-reported and the visual capacity system is symbolic rather than scientific.

Future Implementation

Future development can move Orbit from a manually configured system towards a more adaptive platform.

User Input → Behaviour → Learning → Adaptation

Potential future implementations include:

Real speech recognition

Advanced AI task decomposition

Personalised workload adaptation

Workload prediction

Calendar integration

LMS integration

Email integration

Cloud task persistence

Background synchronisation

User accounts

Additional accessibility features

The long-term direction is:
Today, you tell Orbit your capacity.
Tomorrow, Orbit learns it.
These future features would only be introduced after validating the core Orbit experience.

Project Resources

Ideation

FigJam Brainstorming Board:
[Insert FigJam link]
Figma Storyboard:
[Insert Figma storyboard link]

Design & Prototype

Figma UI Design:
[Insert Figma UI link]
Published Prototype:
[Insert published Figma prototype link]

Presentation

Video Presentation:
[Insert final unlisted YouTube link]
Presentation Slides:
[Insert Canva link]

Documentation

Project Documentation:
[Insert Google Docs link]
System / User Flow Diagrams:
[Insert Figma diagrams link]

Source Code

GitHub Repository:
[Insert GitHub repository link]

ORBIT

Capacity Management for Modern Student Life

Workload adapts to you. Not the other way around.
When you have less capacity, we ask less of you.
