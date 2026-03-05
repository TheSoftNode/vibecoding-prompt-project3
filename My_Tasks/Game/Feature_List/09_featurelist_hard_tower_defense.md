Category: Game

Prompt style: Feature List

Title: Tower Defense Game

Prompt: Build a tower defense game with a path that enemies follow from start to finish. Place towers on empty tiles by clicking tile then selecting tower type: Shooter ($100, shoots bullets), Laser ($200, continuous beam), Freeze ($150, slows enemies). Enemies spawn in waves with increasing difficulty. Each enemy has health bar, speed, and reward value. Towers auto-target nearest enemy in range (show range circle on hover). Bullets travel to enemy with hit detection. Lasers deal continuous damage while targeting. Freeze towers apply 50% slow effect for 3 seconds. Enemies reaching end deduct lives (start with 20). Defeating enemy awards gold. Upgrade towers by clicking them: Level 2 increases damage 50%, Level 3 doubles damage and range. Sell towers for 50% refund. Display wave number, lives, gold, enemies remaining. Next Wave button spawns new wave (auto-spawns after 5 seconds). Show tower stats panel when selected. Game over when lives reach zero. Victory after completing wave 10. Results show waves survived, enemies defeated, towers built, final gold. Pre-load with 3x3 grid path and 25 placeable tiles.

Required libraries: react, tailwindcss, lucide-react, framer-motion

## Rubric

| ID | Description | Weight | Rationale | Dependent On |
|----|-------------|--------|-----------|--------------|
| layout-1 | Display game grid with path and placeable tiles | major | Grid establishes game board structure | None |
| visual-1 | Show enemy path from start to finish | major | Path defines enemy movement route | layout-1 |
| interaction-1 | Open tower selection menu when empty tile is clicked | major | Tile click initiates tower placement | layout-1 |
| visual-2 | Display three tower types with costs in selection menu | major | Tower options enable strategic choice | interaction-1 |
| interaction-2 | Place selected tower on tile and deduct cost from gold | major | Tower placement executes purchase | visual-2 |
| state-1 | Spawn enemy at path start | major | Enemy spawning creates gameplay objectives | None |
| content-1 | Display health bar above each enemy | major | Health visibility shows damage progress | state-1 |
| state-2 | Move enemy along path toward end | major | Enemy movement creates time pressure | state-1 |
| state-3 | Set Shooter tower cost to $100 | major | Pricing establishes economic balance | None |
| state-4 | Set Laser tower cost to $200 | major | Higher cost reflects greater power | None |
| state-5 | Set Freeze tower cost to $150 | major | Mid-range cost balances utility | None |
| state-6 | Auto-target nearest enemy within range for Shooter towers | major | Targeting automation implements tower AI | interaction-2 |
| interaction-3 | Shoot bullet toward targeted enemy | major | Bullet firing is attack mechanic | state-6 |
| state-7 | Travel bullet toward enemy position | major | Projectile movement creates visual feedback | interaction-3 |
| state-8 | Detect hit when bullet reaches enemy location | major | Hit detection enables damage application | state-7 |
| interaction-4 | Reduce enemy health when bullet hits | major | Damage application decrements health | state-8 |
| state-9 | Auto-target nearest enemy for Laser towers | major | Laser targeting implements beam AI | interaction-2 |
| interaction-5 | Display continuous beam from Laser to target | major | Beam visualization shows active targeting | state-9 |
| state-10 | Deal continuous damage while beam is active | major | Sustained damage differentiates laser from shooter | interaction-5 |
| state-11 | Apply 50% speed reduction to enemies hit by Freeze tower | major | Slow effect implements crowd control | interaction-2 |
| state-12 | Remove slow effect after 3 seconds | major | Timed effect requires duration tracking | state-11 |
| visual-3 | Display range circle when hovering over tower | major | Range visualization aids placement decisions | interaction-2 |
| state-13 | Detect when enemy reaches path end | major | End detection triggers life loss | state-2 |
| interaction-6 | Deduct one life when enemy reaches end | major | Life loss creates failure condition | state-13 |
| content-2 | Display lives count starting at 20 | major | Lives visibility shows survival progress | None |
| state-14 | Detect when enemy health reaches zero | major | Death detection triggers reward | interaction-4 |
| interaction-7 | Remove dead enemy from game | major | Enemy removal clears defeated targets | state-14 |
| state-15 | Award gold based on enemy reward value | major | Gold reward incentivizes enemy defeat | interaction-7 |
| content-3 | Display current gold amount | major | Gold visibility shows purchasing power | None |
| interaction-8 | Open upgrade menu when placed tower is clicked | major | Tower click accesses upgrade interface | interaction-2 |
| visual-4 | Display upgrade options with costs in upgrade menu | major | Upgrade visibility enables progression decisions | interaction-8 |
| interaction-9 | Increase tower damage by 50% when upgraded to Level 2 | major | Level 2 upgrade improves effectiveness | visual-4 |
| interaction-10 | Double tower damage and range when upgraded to Level 3 | major | Level 3 upgrade provides major boost | interaction-9 |
| visual-5 | Display Sell button in tower menu | major | Sell option enables tower removal | interaction-8 |
| interaction-11 | Remove tower and refund 50% of total cost when sold | major | Sell mechanic allows repositioning | visual-5 |
| content-4 | Display current wave number | major | Wave tracking shows progression | None |
| state-16 | Increase enemy health and speed with each wave | major | Progressive difficulty escalates challenge | content-4 |
| content-5 | Display enemies remaining in current wave | major | Enemy count shows wave completion progress | None |
| visual-6 | Display Next Wave button | major | Manual wave trigger gives player control | None |
| interaction-12 | Spawn next wave when button is clicked | major | Wave spawning advances gameplay | visual-6 |
| state-17 | Auto-spawn next wave after 5 seconds if button not clicked | major | Auto-spawn maintains pacing | interaction-12 |
| visual-7 | Display tower stats panel when tower is selected | major | Stats provide detailed tower information | interaction-8 |
| content-6 | Show tower damage, range, and level in stats panel | major | Complete stats inform upgrade decisions | visual-7 |
| state-18 | Detect game over when lives reach zero | major | Zero lives triggers loss condition | content-2 |
| interaction-13 | Display game over screen when lives depleted | major | Game over shows defeat | state-18 |
| state-19 | Detect victory when wave 10 is completed | major | Wave 10 completion triggers win condition | content-4 |
| interaction-14 | Display victory screen after wave 10 | major | Victory shows success | state-19 |
| content-7 | Display waves survived on results screen | major | Wave count shows progression achieved | interaction-13 |
| content-8 | Display enemies defeated count on results screen | major | Defeat count quantifies kills | interaction-13 |
| content-9 | Display towers built count on results screen | major | Tower count shows strategic investments | interaction-13 |
| content-10 | Display final gold amount on results screen | major | Final gold shows economic efficiency | interaction-13 |
| state-20 | Pre-populate grid with path and 25 empty tiles on load | major | Initial layout provides starting state | None |
