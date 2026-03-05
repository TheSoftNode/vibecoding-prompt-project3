Write the Prompt
A good prompt tells the model exactly what to build and leaves no ambiguity. Follow these core requirements to ensure high-quality, testable results.

🎯 Core Requirements
Client‑side Only Applications: Focus strictly on front-end specifications.
No Backend: Requirements must be client-side only and scoped to a self-contained web application. There should be no real backend, authentication, or paid APIs.
Data Handling: All data must be local or mocked, but do not include this technical instruction in the prompt itself.
Concrete Features: Describe specific, testable interactions rather than vague aesthetics.
Interactive: The application should involve user actions (clicks, keypresses, drags, etc.) that change the state.
Self‑contained: The solution must be buildable in a single HTML/JS file or a small React app without external build steps.

📚 Required Libraries
When setting up your task, include a comma-separated list of library names that are required for the implementation.
You can use any JavaScript or CSS library (e.g., React, Tailwind CSS, Lucide React).
Ensure the libraries chosen do not violate the client-side only rule.

🗂️ Select Category
Choose the category that best matches the task concept based on the primary functionality:

Choose the category that best matches the task concept based on the primary functionality:

| #   | Name                   | Details                                                         |
| --- | ---------------------- | --------------------------------------------------------------- |
| 1   | **Game**               | Tasks involving rules, scoring, controls, and game states.      |
| 2   | **Web Application**    | Multi-view applications, forms, and validation flows.           |
| 3   | **Data Visualization** | Charts, graphs, and client-side data upload or parsing.         |
| 4   | **Simulation**         | Physics-based interactions, animations, and Canvas/WebGL tasks. |
| 5   | **SVG Generation**     | Vector graphics generation and interactive SVG manipulation.    |
| 6   | \*\*Management System  |

#

Name
Details
1
Game
Tasks involving rules, scoring, controls, and game states.
2
Web Application
Multi-view applications, forms, and validation flows.
3
Data Visualization
Charts, graphs, and client-side data upload or parsing.
4
Simulation
Physics-based interactions, animations, and Canvas/WebGL tasks.
5
SVG Generation
Vector graphics generation and interactive SVG manipulation.
6
Management System
CRUD workflows, tables, dashboards, and administrative interfaces.
7
Multimedia Editing
Canvas-based editors, timelines, and undo/redo systems.
8
Quick Tools
Calculators, converters, and lightweight utility applications.

🎭 Select Prompt Style
Available options depend on the total character length of your prompt. Always focus on observable behavior; requirements should test the rendered output or the code, not the model’s internal reasoning.

1. Terse
   Minimal, imperative description of the task focusing only on core functionality.
   ❌ BAD (unverifiable):
   Snake game.

✅ GOOD (verifiable):
Snake game with arrow key controls. Show score. Game over when you hit the wall.

2. Conversational
   Written as a natural user request, expressing intent and desired behavior in a casual tone.
   ❌ BAD (unverifiable):
   I want a timer.

✅ GOOD (verifiable):
Need a Pomodoro timer with 25/5-minute cycles, big countdown and start/pause/reset buttons.

3. Feature List
   Explicit list of required features and behaviors, often structured as bullet points or short sentences.
   ❌ BAD (unverifiable):
   Build a Kanban board.

✅ GOOD (verifiable):
Build a Kanban board with three columns (To Do, In Progress, Done).
Users should be able to add tasks with a title and description, drag them between columns and delete them.
Each column should show a count of tasks. Add a search bar that filters tasks by title

This example (≈200 characters) enumerates each feature and interaction explicitly, staying within the 150–500 character range for moderate prompts. 4. Detailed Specification
Structured, multi-requirement description with clear constraints, supported features, and UI expectations.
❌ BAD (unverifiable):
Make an awesome data visualizer.

✅ GOOD (verifiable):
Create a data dashboard that lets users upload a CSV file, select columns to visualise and choose from bar, line, pie or scatter charts.
Parse the data client‑side and build a responsive grid that shows the raw data alongside the visualisation.
Add controls to switch chart types, reorder columns, change colours and export the chart as an image.
Provide date range and category filters.
Compute and display summary statistics (total, average, median, min, max) below the chart.
Everything must resize gracefully on mobile and desktop.

This long prompt (>500 characters) details the data flow, interactions and UI expectations. 5. Casual
Informal, shorthand-style request that mirrors real user behavior while still implying concrete requirements.
❌ BAD (unverifiable):
Make a to-do app that works well.

✅ GOOD (verifiable):
Todo list app, but make it actually good, with drag to reorder, swipe to delete, persist to localStorage.
