# PROJECT 3 - VIBE CODING PROJECT: COMPREHENSIVE SUMMARY

## **OVERVIEW**

**Project Goal:** Train models to build client-side web applications through prompts, rubrics, and metadata that test state management, event handling, and layout correctness.

**Evaluation Method:** Vision-language models grade tasks using **only a single screenshot** and the submitted HTML/JS code—**no manual interaction**.

---

## **CORE DELIVERABLES**

Each task requires:
1. **Prompt** - Natural-language specification (client-side only, self-contained web app)
2. **Rubric** - 8-20 atomic, tagged criteria (visual, layout, content, interaction, state)
3. **Metadata** - Category, difficulty, prompt style, required libraries

---

## **GOLDEN RULE ⚠️**

**Tasks are evaluated by vision-language models using only:**
- A single screenshot (initial render)
- The submitted HTML/JS code

**This means:**
- ✅ Applications should be interactive, stateful, with buttons/inputs/controls
- ✅ Rubric items must be verifiable from screenshot + code inspection ONLY
- ❌ NO criteria requiring clicking, typing, or exploring UI states
- ❌ NO hidden states, pages, or flows requiring interaction to verify
- ❌ NOT purely static pages with only text/images

---

## **1. CATEGORIES (Choose One)**

| # | Category | Description |
|---|----------|-------------|
| 1 | **Game** | Rules, scoring, controls, game states |
| 2 | **Web Application** | Multi-view apps, forms, validation flows |
| 3 | **Data Visualization** | Charts, graphs, client-side data parsing |
| 4 | **Simulation** | Physics interactions, animations, Canvas/WebGL |
| 5 | **SVG Generation** | Vector graphics, interactive SVG manipulation |
| 6 | **Management System** | CRUD workflows, tables, dashboards |
| 7 | **Multimedia Editing** | Canvas editors, timelines, undo/redo |
| 8 | **Quick Tools** | Calculators, converters, utility apps |

---

## **2. PROMPT STYLES (Choose One Based on Length)**

### **1. Terse** (Very short)
Minimal, imperative description focusing on core functionality.
```
✅ GOOD: Snake game with arrow key controls. Show score. Game over when you hit the wall.
❌ BAD: Snake game.
```

### **2. Conversational** (Short)
Natural user request, expressing intent in casual tone.
```
✅ GOOD: Need a Pomodoro timer with 25/5-minute cycles, big countdown and start/pause/reset buttons.
❌ BAD: I want a timer.
```

### **3. Feature List** (150-500 chars, Moderate)
Explicit bullet points or short sentences listing features.
```
✅ GOOD: Build a Kanban board with three columns (To Do, In Progress, Done). Users should be able to add tasks with a title and description, drag them between columns and delete them. Each column should show a count of tasks. Add a search bar that filters tasks by title.
```

### **4. Detailed Specification** (>500 chars, Long)
Structured, multi-requirement description with clear constraints, features, UI expectations.
```
✅ GOOD: Create a data dashboard that lets users upload a CSV file, select columns to visualise and choose from bar, line, pie or scatter charts. Parse the data client-side and build a responsive grid that shows the raw data alongside the visualisation. Add controls to switch chart types, reorder columns, change colours and export the chart as an image. Provide date range and category filters. Compute and display summary statistics (total, average, median, min, max) below the chart. Everything must resize gracefully on mobile and desktop.
```

### **5. Casual** (Short, informal)
Informal, shorthand-style request mirroring real user behavior.
```
✅ GOOD: Todo list app, but make it actually good, with drag to reorder, swipe to delete, persist to localStorage.
❌ BAD: Make a to-do app that works well.
```

---

## **3. DIFFICULTY TARGETING (Model Failure Requirement)**

**Target Pass Rates:**
- **Easy:** 70-100% pass rate
- **Medium:** 40-70% pass rate
- **Hard:** 0-40% pass rate

### **Five Strategies to Create Challenging Prompts:**

#### **Strategy 1: Layer Cross-Feature Dependencies**
Create features that depend on and influence each other.
```
❌ Weak: Show a score counter. Show a speed indicator. Show a wave counter.
✅ Strong: Every 5 kills, all enemies gain a permanent movement speed increase. Display the current speed tier as "Wave X" next to the score, where X increments by 1 for every 5 kills.
```

#### **Strategy 2: Demand Precise Visual and Layout Constraints**
Specify exact placement, colors, structured layouts.
```
❌ Weak: Add a HUD with health and ammo.
✅ Strong: HUD layout: Top-left - inventory bar with 5 slots, slot 1 holds a pistol by default. Top-right - 3 heart icons for lives, lost hearts turn gray. Bottom-center - ammo count for the active weapon.
```

#### **Strategy 3: Build Evolving State Machines**
Design apps where state transforms over time based on rules.
```
✅ Example: Destroyed enemies respawn at a random arena edge after 5 seconds. Every 5 kills, all enemies gain a permanent movement speed increase. The game gets progressively harder until the player runs out of lives.
```

#### **Strategy 4: Specify Rich Initial Render State**
Make the initial load substantive and verifiable.
```
✅ Example: On initial load, render the full arena with the player centered, all 5 enemies placed, all crates visible, and HUD showing Wave 1, score 0, full hearts, and the pistol selected with its ammo count.
```

#### **Strategy 5: Write Rubrics That Target Known Weak Spots**
Focus on junctions where features connect, not individual features.

| What to Check | Why Challenging |
|--------------|----------------|
| Derived values (Wave X from kill count) | Often hardcoded or miscalculated |
| Conditional visual changes (gray hearts) | Visuals may not update on state change |
| Spatial layout (top-left, bottom-center) | HUD elements frequently misplaced |
| Default states (slot 1 = pistol) | Initial values sometimes skipped |
| Entity counts (exactly 5 enemies) | Quantities rounded or approximated |
| Compound behaviors (respawn + speed increase) | One behavior works, other broken |

---

## **4. RUBRIC REQUIREMENTS**

### **Quantity:**
- **8-20 criteria** (strongly preferred)
- If exceeding 20, prioritize and reduce

### **Five Tags:**

| Tag | Focus | Verification |
|-----|-------|-------------|
| **visual** | Element existence, color, styling (no text/position) | Screenshot (initial render) |
| **layout** | Spatial placement, alignment relative to other elements | Screenshot or Code |
| **content** | Exact text, labels, numbers, data values displayed | Screenshot or Code |
| **interaction** | User action (click, drag, type) → immediate result | Code Review |
| **state** | Data/app state changing or persisting over time | Code Review |

### **Weight:**
- **major** - Critical/core functionality essential to task success
- **minor** - Nice-to-have or secondary aesthetic details

### **dependent_on:**
- List of criterion IDs that MUST pass before this one can be evaluated
- Example: Can't check "Score updates on click" if "Score display exists" failed

---

## **5. RUBRIC QUALITY REQUIREMENTS**

### **Description Must Be:**

1. **Clear and unambiguous** - Precise language, obvious pass/fail
   - ❌ Forbidden words: correctly, properly, appropriately, clearly, adequately, thoroughly
   ```
   ❌ BAD: Countdown works correctly
   ✅ GOOD: Start button begins countdown
   ```

2. **Self-contained** - Enough context to evaluate independently
   ```
   ❌ BAD: Centered
   ✅ GOOD: Display center timer on the page
   ```

3. **Task-specific** - Tied to unique features
   ```
   ❌ BAD: Includes a button
   ✅ GOOD: Reset button returns timer to 25:00
   ```

4. **Non-stacked** - One expectation per item
   ```
   ❌ BAD: Start and pause the timer
   ✅ GOOD (split into 2):
   - Begin countdown when the Start button is clicked
   - Stop countdown without resetting when the Pause button is clicked
   ```

5. **Appropriately flexible** - Allow different valid implementations
   ```
   ❌ BAD: Use a table element for tasks
   ✅ GOOD: Display tasks in a list or table
   ```

6. **Verifiable** - Observable behavior, not internal reasoning
   ```
   ❌ BAD: Keep track of score internally
   ✅ GOOD: Show current score near the board
   ```

7. **Comprehensive** - Every prompt requirement has ≥1 rubric item

8. **Non-redundant** - No overlapping/duplicate checks

9. **Action word usage** - Start with present-tense action verb
   ```
   ❌ BAD: Countdown displays in MM:SS format
   ✅ GOOD: Display countdown in MM:SS format
   ```

10. **Checkable from screenshot + code** - VLM must be able to verify
    ```
    ❌ BAD:
    - Ensure user data is saved to production database
    - The page should load very quickly
    ✅ GOOD: Display the current score near the board
    ```

### **Rationale Must:**
- Explain WHY the criterion matters (not restate description)
- Be aligned with description
- Contain no factual errors
- Be specific to this task

### **Rationale Must NOT:**
- ❌ Refer to the agent (e.g., "the agent may assume...")
- ❌ Refer to specific implementation (e.g., "during development...")
- ❌ Be generic (e.g., "Because this is important")
- ❌ Expose implementation hints (e.g., "methods should throw error silently...")

---

## **6. VISUAL TAG SPECIAL REQUIREMENT**

**All `visual` criteria must be verifiable from initial load screenshot.**

**If the app would render blank/empty on load, you MUST specify pre-loaded sample data in the prompt:**

Examples:
- Tables/lists: "On initial load, render a table pre-populated with at least 5 sample rows using placeholder data."
- Cards/grids: "On initial load, display a grid of 6 sample product cards, each with a title, price, and image, using mock data."
- Charts: "On initial load, render a bar chart using predefined sample data (e.g., values for Jan–Jun)."

---

## **7. CORE REQUIREMENTS**

✅ **Client-side only** - No backend, authentication, or paid APIs
✅ **Data handling** - All data local or mocked (don't state this in prompt)
✅ **Concrete features** - Specific, testable interactions (not vague aesthetics)
✅ **Interactive** - User actions (clicks, keypresses, drags) change state
✅ **Self-contained** - Buildable in single HTML/JS file or small React app

---

## **8. EVALUATION WORKFLOW**

1. Click "Generate App" button
2. Copy & paste URL into new browser tab (clicking doesn't work)
3. Take screenshot of initial render
4. Upload ONE screenshot for entire task
5. Click "Evaluate" button
6. Check fairness: Are failures legitimate?
7. Verify passes: Do passing rubrics actually work in the app?
8. If rubrics unfair → Fix criteria and restart

---

## **9. LLM USAGE POLICY**

### **✅ Allowed (with human oversight):**
- Ideas & brainstorming
- Prompt review (tone, grammar)
- Rubric review (vague language, compound criteria)
- Grammar & clarity polishing

### **🔍 Required Human Verification:**
- Criteria are truly atomic
- No forbidden words
- Completeness against prompt
- Verifiable from screenshot/code

### **🚫 Prohibited:**
- LLM-generated rubric content
- LLM-generated prompt content

### **📝 Requirements:**
- Attribution: You're fully accountable for final result
- Originality: Keep authentic voice, avoid robotic language

---

## **10. PATTERN ANALYSIS FROM EXAMPLES**

### **Example 1: SVG Avatar (Medium, Game, Detailed Spec)**
- **10 rubric items** (9 major, 1 minor)
- Uses 6 tags: 3 visual, 4 content, 2 interaction, 1 layout
- Rich initial state: avatar preview visible on load
- Cross-feature dependency: interaction-1 depends on visual-1

### **Example 2: Audio Visualizer (Hard, Multimedia, Feature List)**
- **9 rubric items** (7 major, 2 minor)
- Uses 5 tags: 4 visual, 1 state, 3 interaction, 1 content
- Hard difficulty from: Canvas rendering + real-time audio frequency analysis + multiple input modes

### **Example 3: Shopping App (Medium, Web App, Feature List)**
- **11 rubric items** (9 major, 2 minor)
- Uses 5 tags: 2 visual, 5 interaction, 1 state, 3 content
- Multiple dependencies: interaction-3 depends on content-1 AND content-2
- Multi-view navigation testing

### **Example 4: Color Grid Game (Medium, Game, Detailed Spec)**
- **13 rubric items** (10 major, 3 minor)
- Uses 5 tags: 2 visual, 5 state, 4 interaction, 4 content, 1 layout
- Evolving state: sequence grows each round, progressive scoring
- Cross-feature dependencies: state chains (state-1 → state-2 → interaction-1)

### **Example 5: Password Strength (Easy, Quick Tools, Feature List)**
- **11 rubric items** (8 major, 3 minor)
- Uses 5 tags: 1 visual, 2 layout, 6 state, 2 interaction, 1 content
- Easy difficulty: straightforward state rules, no complex dependencies
- Rich initial state specified: "On load the text input should be blank and the indicator should be red with text 'Weak'"

### **Example 6: Scheduling Board (Hard, Management System, Detailed Spec)**
- **14 rubric items** (11 major, 3 minor)
- Uses 5 tags: 3 layout, 7 state, 2 interaction, 1 content, 1 visual
- Hard from: Complex drag-drop logic + priority-based conflict resolution + GPU resource constraint across workers + timeline adjustment cascading effects
- Heavy on state criteria (50% of rubric) = complex state machine

### **Example 7: Weather Dashboard (Vague One-liner)**
- **8 rubric items** (6 major, 2 minor)
- Prompt: Just "Build a weather dashboard"
- Shows that even minimal prompts need comprehensive rubrics
- All visual tags require mock data pre-loaded

### **Example 8: Wordle Clone (Clone/Replica)**
- **9 rubric items** (7 major, 2 minor)
- Recreates well-known game mechanics
- Keyboard synchronization tested as separate criterion from grid feedback

### **Example 9: SaaS Landing Page (UI/Landing Page)**
- **9 rubric items** (6 major, 3 minor)
- Tests cross-section state coordination (pricing toggle updates hero CTA)
- All sections visible on initial load requirement

---

## **KEY PATTERNS OBSERVED:**

1. **Rubric count:** 8-14 items typical, stays under 20
2. **Major/minor ratio:** ~70-80% major, 20-30% minor
3. **Tag distribution varies by category:**
   - Games: Heavy on state + interaction
   - Web apps: Heavy on interaction + content
   - Tools: Heavy on state
   - Simulations: Heavy on visual + state
4. **Dependencies:** 0-3 per task, used sparingly for critical chains
5. **Initial render state:** Always specified explicitly when visual tags present
6. **Action verbs:** Render, Display, Enable, Allow, Update, Apply, Position, Provide, Include, Arrange

---

## **PRE-SUBMISSION CHECKLIST:**

- [ ] Cross-feature dependencies: ≥3 features depend on each other?
- [ ] Precise specifications: Exact layout/position requirements for key UI?
- [ ] Evolving state: State transforms over time (not just toggle)?
- [ ] Rich initial render: Initial render fully specified with defaults?
- [ ] Junction-focused rubrics: Target connections between features?
- [ ] Fair verification: Every rubric item verifiable from screenshot or code?
- [ ] 8-20 rubric items total
- [ ] Every prompt requirement covered by ≥1 rubric item
- [ ] No forbidden words in descriptions
- [ ] All descriptions start with action verbs
- [ ] Rationales explain WHY, not restate WHAT
- [ ] Visual tags have pre-loaded data specified in prompt
- [ ] Category and prompt style selected
- [ ] Required libraries listed
- [ ] Difficulty aligns with target pass rates

---

## **READY TO DECIDE:**

Now I need to choose:
1. **Category** (1 of 8)
2. **Prompt Style** (1 of 5)

Following the example: "Henry is going with web app and conversational"
