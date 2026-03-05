Category: Game

Prompt style: Casual

Title: Multiplayer Battleship

Prompt: Battleship game but make it slick. Two 10x10 grids side-by-side: your fleet (left) and enemy waters (right). Place 5 ships: Carrier (5 cells), Battleship (4), Cruiser (3), Submarine (3), Destroyer (2). Drag ships to position, click to rotate. Ships can't overlap or go off-grid. Once all placed, game starts. Take turns clicking enemy grid to fire. Hits show red X, misses show white O. When all cells of a ship are hit, show "Carrier sunk!" message and reveal full ship. Track shots fired, hit percentage, ships remaining for both players. AI opponent has three difficulty levels: Easy (random shots), Medium (targets adjacent cells after hit), Hard (hunts systematically and finishes ships). Show hit streak counter (consecutive hits). Power-ups spawn randomly on your grid after 5 shots: Sonar (reveals 3x3 area), Airstrike (hits 5 random cells), Shield (protects one ship from next hit). Power-up usage limited to one per type. Display tactical mini-map showing hit patterns. After game ends show battle stats: accuracy, ships sunk vs lost, longest hit streak, power-ups used, total turns. Leaderboard tracks wins. Rematch button. Include sound effects and sinking ship animations.

Required libraries: react, tailwindcss, lucide-react, framer-motion

## Rubric

| ID | Description | Weight | Rationale | Dependent On |
|----|-------------|--------|-----------|--------------|
| layout-1 | Display two 10x10 grids side-by-side | major | Dual grid layout separates player and enemy boards | None |
| content-1 | Label left grid as player's fleet | major | Fleet grid shows player ships | layout-1 |
| content-2 | Label right grid as enemy waters | major | Enemy grid is attack target | layout-1 |
| state-1 | Create 5 ships with correct cell counts | major | Ship definitions establish game pieces | None |
| visual-1 | Display ships as draggable elements during placement | major | Drag interface enables positioning | state-1 |
| interaction-1 | Move ship position by dragging | major | Drag mechanic implements placement | visual-1 |
| interaction-2 | Rotate ship orientation when clicked | major | Rotation enables horizontal/vertical placement | visual-1 |
| state-2 | Prevent ship placement if overlapping another ship | major | Overlap prevention enforces spacing rules | interaction-1 |
| state-3 | Prevent ship placement if extending off grid | major | Boundary checking enforces grid limits | interaction-1 |
| interaction-3 | Lock ships and start game when all 5 are placed | major | Placement completion triggers game start | state-2 |
| interaction-4 | Fire shot at clicked cell in enemy grid | major | Click attack is primary game interaction | layout-1 |
| state-4 | Check if shot hits enemy ship | major | Hit detection determines shot outcome | interaction-4 |
| visual-2 | Display red X on hit cells | major | Red marks successful hits | state-4 |
| visual-3 | Display white O on miss cells | major | White marks unsuccessful shots | state-4 |
| state-5 | Track hits per ship to detect sinking | major | Hit accumulation detects ship destruction | state-4 |
| state-6 | Detect when all cells of a ship are hit | major | Sinking detection identifies destroyed ships | state-5 |
| content-3 | Display "[Ship name] sunk!" message when ship destroyed | major | Sinking notification confirms destruction | state-6 |
| visual-4 | Reveal full sunken ship on enemy grid | major | Ship reveal shows destruction location | state-6 |
| content-4 | Display shots fired count | major | Shot tracking quantifies attempts | None |
| content-5 | Display hit percentage | major | Accuracy metric shows shooting efficiency | None |
| state-7 | Calculate hit percentage as (hits / shots fired) × 100 | major | Percentage is derived accuracy metric | content-5 |
| content-6 | Display ships remaining for player and AI | major | Ship counts show survival progress | None |
| state-8 | Generate random shot positions for Easy AI | major | Easy AI uses simplest strategy | None |
| state-9 | Target adjacent cells after hit for Medium AI | major | Medium AI implements smart follow-up | state-4 |
| state-10 | Hunt systematically and finish ships for Hard AI | major | Hard AI uses optimal targeting | state-9 |
| visual-5 | Display difficulty selector with Easy, Medium, Hard | major | Difficulty selection customizes challenge | None |
| content-7 | Display hit streak counter | major | Streak shows consecutive success | None |
| state-11 | Increment streak on hit, reset on miss | major | Streak tracking alternates on outcome | state-4 |
| state-12 | Spawn Sonar power-up after 5 shots fired | major | Power-up spawn rewards progress | content-4 |
| visual-6 | Display Sonar power-up icon on player grid | major | Power-up visibility enables activation | state-12 |
| interaction-5 | Reveal 3x3 area on enemy grid when Sonar is used | major | Sonar reveals hidden ships | visual-6 |
| state-13 | Spawn Airstrike power-up randomly | major | Airstrike spawn adds strategic option | None |
| interaction-6 | Hit 5 random cells when Airstrike is used | major | Airstrike deals multi-cell damage | state-13 |
| state-14 | Spawn Shield power-up randomly | major | Shield spawn adds defensive option | None |
| interaction-7 | Block next hit on protected ship when Shield is used | major | Shield prevents damage | state-14 |
| state-15 | Limit each power-up type to one use per game | major | Usage cap prevents power-up spam | interaction-5 |
| visual-7 | Display tactical mini-map showing hit patterns | major | Mini-map provides attack overview | None |
| state-16 | Update mini-map after each shot | major | Real-time update maintains accuracy | visual-7 |
| state-17 | Detect game end when all player ships sunk | major | All ships destroyed triggers loss | state-6 |
| state-18 | Detect game end when all AI ships sunk | major | All enemy ships destroyed triggers win | state-6 |
| interaction-8 | Display battle stats screen after game ends | major | Stats show game summary | state-17 |
| content-8 | Display accuracy percentage on stats screen | major | Accuracy shows shooting efficiency | interaction-8 |
| content-9 | Display ships sunk vs lost on stats screen | major | Ship comparison shows combat outcome | interaction-8 |
| content-10 | Display longest hit streak on stats screen | major | Max streak shows peak performance | interaction-8 |
| state-19 | Track longest streak by comparing to current | major | Max tracking requires ongoing comparison | content-10 |
| content-11 | Display power-ups used count on stats screen | major | Power-up count shows strategic usage | interaction-8 |
| content-12 | Display total turns taken on stats screen | major | Turn count quantifies game duration | interaction-8 |
| layout-2 | Display leaderboard showing win records | major | Leaderboard provides competitive context | None |
| state-20 | Add win to leaderboard after victory | major | Win tracking maintains historical records | state-18 |
| visual-8 | Display Rematch button on stats screen | major | Rematch enables replay | None |
| interaction-9 | Reset game and return to ship placement when Rematch clicked | major | Rematch starts new game | visual-8 |
| visual-9 | Play sound effects for hits, misses, and sinking | major | Audio enhances feedback | state-4 |
| visual-10 | Animate ships sinking when destroyed | major | Animation enhances destruction feedback | state-6 |
