How to Design Challenging Prompts
Purpose: Repeatable strategies for creating prompts that test AI capabilities through layered complexity, particularly for Medium (40-70% pass) and Hard (0-40% pass) difficulty tasks.
Core Principle
AI models excel at isolated features but struggle when managing multiple interacting systems simultaneously. The key to challenging prompts lies not in complexity of individual components, but in how those components interact, depend on each other, and evolve together.
The three pillars of complexity:
Complex interactions between features
Dependent rules that cascade through systems
Evolving state that transforms over time
Five Strategies
Strategy 1: Layer Cross-Feature Dependencies
Create features that depend on and influence each other, forming chains of interaction.
Weak approach (easily handled):
Show a score counter. Show a speed indicator. Show a wave counter.
Strong approach (forces dependency chains):
Every 5 kills, all enemies gain a permanent movement speed increase. Display the current speed tier as "Wave X" next to the score, where X increments by 1 for every 5 kills.
Why this works: The kill count drives the wave number, which drives enemy speed, which affects gameplay difficulty. Four systems must work simultaneously: tracking kills, deriving tier, applying modifiers, and updating display.
Implementation tip: After drafting features, map their relationships. If nothing connects, wire them together by asking: "What should change when this changes?"

Strategy 2: Demand Precise Visual and Layout Constraints
Specify exact placement, specific color assignments, and structured layouts rather than general appearance.
Weak approach:
Add a HUD with health and ammo.
Strong approach:
HUD layout: Top-left - inventory bar with 5 slots, slot 1 holds a pistol by default. Top-right - 3 heart icons for lives, lost hearts turn gray. Bottom-center - ammo count for the active weapon.
Why this works: Creates multiple verifiable requirements: position of each element, default states, exact quantities, color change behaviors, and placement hierarchy.
Implementation tip: For every UI element, specify its position (top-left, bottom-center, etc.), default/initial state, and appearance changes based on state transitions.

Strategy 3: Build Evolving State Machines
Design apps where state transforms over time based on rules, rather than remaining static.
Example of evolving state:
Destroyed enemies respawn at a random arena edge after 5 seconds. Every 5 kills, all enemies gain a permanent movement speed increase. The game gets progressively harder until the player runs out of lives.
Why this works: Requires implementing per-enemy respawn timers, global kill counters, derived speed modifiers that persist and compound, and game-over conditions dependent on separate life counters. Each state evolves on its own timeline while interacting with others.
Implementation tip: Add at least one rule where state accumulates or transforms over time (timers, wave progression, score multipliers, difficulty scaling).

Strategy 4: Specify Rich Initial Render State
Since evaluation often uses a single screenshot on initial load, make the initial render substantive and verifiable.
Example:
On initial load, render the full arena with the player centered, all 5 enemies placed, all crates visible, and HUD showing Wave 1, score 0, full hearts, and the pistol selected with its ammo count.
Why this works: Provides 6+ verifiable items from one screenshot: player position, enemy count, crate visibility, wave display, score display, heart display, and selected weapon indicator.
Implementation tip: Always end prompts with an explicit "on initial load" sentence describing everything that should be visible.

Strategy 5: Write Rubrics That Target Known Weak Spots
Focus rubric items on the seams where features connect, not just on individual features.

| What to Check                                 | Why This Is Challenging                  |
| --------------------------------------------- | ---------------------------------------- |
| Derived values (Wave X from kill count)       | Often hardcoded or miscalculated         |
| Conditional visual changes (gray hearts)      | Visuals may not update on state change   |
| Spatial layout (top-left, bottom-center)      | HUD elements frequently misplaced        |
| Default states (slot 1 = pistol)              | Initial/default values sometimes skipped |
| Entity counts (exactly 5 enemies, 8 crates)   | Quantities rounded or approximated       |
| Compound behaviors (respawn + speed increase) | One behavior implemented, other broken   |

What to Check
Why This Is Challenging
Derived values (Wave X from kill count)
Often hardcoded or miscalculated
Conditional visual changes (gray hearts)
Visuals may not update on state change
Spatial layout (top-left, bottom-center)
HUD elements frequently misplaced
Default states (slot 1 = pistol)
Initial/default values sometimes skipped
Entity counts (exactly 5 enemies, 8 crates)
Quantities rounded or approximated
Compound behaviors (respawn + speed increase)
One behavior implemented, other broken

Category-Specific Applications
The five strategies above are universal, but the specific failure surfaces shift depending on the application type.
Games
Natural fit for: Cross-feature dependencies through rules, state, and real-time interaction.
Focus on: Interacting subsystems where inventory affects combat, kill counts drive difficulty, physics influences scoring. The more game mechanics feed into each other, the more challenging the implementation.
Effective complexity levers:
Tiered scoring with conditions
Ammo/resource management scoped per-entity (not global)
AI behavior that changes based on game state
Precise HUD layout with derived displays
Web Applications
Natural fit for: Chained validation rules across views and form state affecting multiple UI parts.
Focus on: Multi-step workflows where later steps depend on earlier selections, with live summaries that update as users progress.
Effective complexity levers:
Cross-field validation (e.g., end date after start date, both affecting duration display)
Conditional rendering based on previous input
Persistent summary/preview reflecting all current form state
Undo/back navigation preserving partial entries
Data Visualization
Natural fit for: Multiple coordinated views with interactive filtering.
Focus on: Dashboards where selecting elements in one chart filters tables and updates summary panels, requiring wired components sharing state.
Effective complexity levers:
Linked/brushed views (click on chart A, chart B and table C update)
Computed summary statistics displayed alongside visuals (total, average, median)
User-togglable chart types preserving axis scaling
Upload + parse + visualize pipeline where column type detection matters
Simulations
Natural fit for: Continuous simulation with discrete rule triggers.
Focus on: Combining physics (e.g., bouncing ball) with state changes (color change on bounce), event triggers (split after 5 bounces), and score updates (increment when fragments exit boundary).
Effective complexity levers:
Gravity/collision physics with precise behavioral consequences
Particle systems where individual particles have state
User-adjustable parameters updating simulation in real time without reset
Time-based triggers (e.g., after 10 seconds, spawn new obstacle)
SVG Generation
Natural fit for: Precise spatial relationships and conditional styling.
Focus on: Complex composed graphics where element positions are mathematically derived from inputs, with colors/styles changing based on combination logic.
Effective complexity levers:
Elements that must align or connect precisely (graph nodes and edges, avatar body parts)
Conditional styling where one selection affects multiple elements (angry expression changes eyebrows, mouth, and color tint)
Export preserving all dynamic state as valid SVG
Management Systems
Natural fit for: Cross-entity relationships, derived summaries, and state-dependent UI changes.
Focus on: Project management where tasks belong to categories, categories have budget caps, task assignment deducts from budget and updates progress bars, with over-budget categories turning red.
Effective complexity levers:
Cascading updates (deleting parent entity updates/removes children)
Derived aggregations displayed in real time (totals, percentages, counts)
Filtering/sorting persisting across add/edit/delete operations
Status-dependent styling (overdue items red, completed items moved to different section)
Multimedia Editing
Natural fit for: Undo/redo tracking complex composite state and multiple tool modes interacting with the same canvas.
Focus on: Editors supporting draw, select, move, resize, color change, group objects, with reversible operations in sequence.
Effective complexity levers:
Undo/redo across heterogeneous operations (draw, move, delete all reversible in order)
Tool mode switching where each mode interprets same mouse events differently
Layer/z-order management with visual stacking
Export serializing full editor state (not just visible canvas)
Quick Tools
Natural fit for: Bidirectional conversion, chained computations, and edge-case formatting.
Focus on: Unit converters where editing either field updates the other in real time, with locale-aware formatting, input validation showing inline errors, and history logs.
Effective complexity levers:
Bidirectional/live updates (editing output recalculates input)
Chained conversions where intermediate rounding affects final results
Format-sensitive display (currency symbols, decimal places, thousands separators)
Copy-to-clipboard with specific formatting
Input edge cases (negative numbers, zero, extremely large values)
Complete Worked Examples
Example A: 2D Top-Down Shooter
Concept: 2D top-down shooter in a walled arena.
Layered systems (7 interconnected):
Player mechanics - movement (WASD), aiming (mouse cursor), shooting (left-click), aim indicator line, crosshair at cursor
Inventory system - 5 slots, default pistol, 3 weapon pickups from color-coded crates, crate removal on pickup
Enemy AI - 5 enemies that chase the player, contact damage, one-hit kills from any weapon, respawn at random edge after 5 seconds
Evolving difficulty - every 5 kills triggers a permanent speed increase and wave increment
HUD - precise layout (top-left inventory, top-right hearts, bottom-center ammo), visual feedback (gray hearts), derived display (Wave X)
Game over - dark overlay, red "GAME OVER" text, restart button
Initial render - everything visible on load with specific default values
Why this achieves <40% pass rate: The failure comes from density of interacting rules. Kill count feeds wave number feeds enemy speed. Create color maps to weapon type maps to inventory slots. Contact triggers both life loss and enemy destruction. Every mechanic touches at least two others.
Example B: 3D Clay Pigeon Shooting
Concept: 3D clay pigeon shooting range with rounds, scoring, and physics.
Dual-front attack (3D rendering + complex logic):
3D scene setup - sky-blue gradient background, green ground plane, visible dark launcher structure near bottom-center
Physics - each pigeon follows an arc trajectory with random up-angle and speed, curving back down under gravity
Round structure - 3 rounds of 5 pigeons each (fixed progression requiring state tracking)
Ammo constraint - 2 shots per pigeon, must reset per pigeon (not per round)
Tiered scoring - 2 points on first shot, 1 point on second (tracks which shot hit, not just whether hit occurred)
HUD with derived values - current round, hits vs. launched this round, remaining cartridges for current pigeon, total score
Hit feedback - fragment shatter + particle burst
End state - results overlay with total score, accuracy percentage (hits/shots fired), pigeons hit out of 15, reset button
Initial render - ready state with Round 1 displayed and "Pull!" button visible
Why this works: Attacks on two fronts. First, 3D rendering with Three.js creates inherent challenges with scene composition, click-raycasting on moving objects, and gravity arcs. Second, the scoring system has layered conditionals requiring per-pigeon shot tracking (not global), deriving point values from shot order, computing accuracy ratios, and displaying round-scoped stats alongside global stats.
Key failure points to verify:
Does the pigeon follow a gravity arc (not straight line or random path)?
Does shot counter reset per pigeon (not per round)?
Is scoring 2/1 based on shot order (not flat)?
Does accuracy calculation use shots fired (not pigeons launched)?
Is the launcher structure visible and positioned near the bottom-center?
Does the initial render show Round 1 and Pull button?
Each rubric item tests a specific junction where two systems meet: physics + rendering, ammo tracking + per-pigeon scope, shot order + score value, two counters + one derived percentage.
Pre-Submission Checklist
Before finalizing your prompt, verify:
Cross-feature dependencies: Do at least 3 features depend on each other?
Precise specifications: Are there exact layout/position requirements for HUD or key UI elements?
Evolving state: Does state transform over time (not just toggle on/off)?
Rich initial render: Is the initial render fully specified with verifiable defaults?
Junction-focused rubrics: Do rubric items target connections between features, not just individual features?
Fair verification: Is every rubric item specific and verifiable from a screenshot or code?
If you can check all six boxes, your prompt is well-positioned to achieve target difficulty levels through genuine complexity rather than ambiguity.
