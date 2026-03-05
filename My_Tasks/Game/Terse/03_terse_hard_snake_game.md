Category: Game

Prompt style: Terse

Title: Snake Game with Power-ups

Prompt: Snake game on 20x20 grid. Arrow keys control direction. Snake starts length 3, grows by 1 when eating food. Food spawns randomly, shows points value (10-50). Game over when snake hits wall or itself. Three power-up types spawn randomly every 10 seconds: Speed Boost (blue, doubles speed for 5 seconds), Score Multiplier (gold, 2x points for 10 seconds), Invincibility (green, pass through walls and self for 5 seconds). Power-ups flash when about to expire (last 2 seconds). Display score, current length, high score, active power-ups with timers. Speed increases every 50 points. Level indicator shows current speed level. Pause button freezes game. After game over, show stats: final score, length reached, food eaten, power-ups collected, survival time. Leaderboard shows top 5 scores with names. On load, display empty grid with snake at center, one food item spawned.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| ID        | Description                                                                                         | Weight | Rationale                                                                          | Dependent On |
| --------- | --------------------------------------------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------- | ------------ |
| layout-1  | Display 20x20 grid game board                                                                       | major  | Grid defines playing field boundaries.                                             | None         |
| state-1   | Initialize snake with length 3 at center of grid                                                    | major  | Starting position establishes initial state.                                       | layout-1     |
| interaction-1 | Change snake direction when arrow keys are pressed                                              | major  | Keyboard controls enable player navigation.                                        | None         |
| state-2   | Move snake one cell in current direction at regular intervals                                       | major  | Continuous movement creates game progression.                                      | state-1      |
| state-3   | Randomly spawn food at empty grid position                                                          | major  | Food placement creates collection objectives.                                      | None         |
| content-1 | Display food on grid                                                                                | major  | Food visibility provides target.                                                   | state-3      |
| state-4   | Assign random point value between 10-50 to each food item                                           | major  | Variable value adds strategic collection priority.                                 | state-3      |
| content-2 | Display point value on food item                                                                    | major  | Value display informs collection decisions.                                        | state-4      |
| interaction-2 | Increase snake length by 1 when head reaches food position                                      | major  | Growth mechanic rewards food collection.                                           | state-2      |
| state-5   | Add food point value to score when collected                                                        | major  | Score accumulation tracks performance.                                             | interaction-2 |
| state-6   | Spawn new food after previous food is collected                                                     | major  | Continuous food availability maintains gameplay.                                   | interaction-2 |
| state-7   | Detect collision when snake head hits grid boundary                                                 | major  | Wall collision implements game over condition.                                     | state-2      |
| state-8   | Detect collision when snake head overlaps with body segment                                         | major  | Self-collision implements game over condition.                                     | state-2      |
| interaction-3 | End game when collision is detected                                                             | major  | Collision triggers game termination.                                               | state-7      |
| state-9   | Spawn Speed Boost power-up at random position every 10 seconds                                      | major  | Timed spawn creates power-up availability.                                         | None         |
| visual-1  | Display Speed Boost power-up in blue color                                                          | major  | Blue identifies speed power-up type.                                               | state-9      |
| interaction-4 | Double snake speed for 5 seconds when Speed Boost is collected                                  | major  | Speed doubling creates temporary gameplay change.                                  | visual-1     |
| state-10  | Start 5-second timer when Speed Boost is activated                                                  | major  | Timed effect requires countdown tracking.                                          | interaction-4 |
| state-11  | Return snake to normal speed when Speed Boost timer expires                                         | major  | Effect expiration restores default behavior.                                       | state-10     |
| state-12  | Spawn Score Multiplier power-up at random position every 10 seconds                                 | major  | Timed spawn creates multiplier availability.                                       | None         |
| visual-2  | Display Score Multiplier power-up in gold color                                                     | major  | Gold identifies multiplier power-up type.                                          | state-12     |
| interaction-5 | Apply 2x multiplier to food points for 10 seconds when Score Multiplier is collected            | major  | Multiplier doubling increases point value.                                         | visual-2     |
| state-13  | Start 10-second timer when Score Multiplier is activated                                            | major  | Timed effect requires countdown tracking.                                          | interaction-5 |
| state-14  | Remove 2x multiplier when Score Multiplier timer expires                                            | major  | Effect expiration restores default scoring.                                        | state-13     |
| state-15  | Spawn Invincibility power-up at random position every 10 seconds                                    | major  | Timed spawn creates invincibility availability.                                    | None         |
| visual-3  | Display Invincibility power-up in green color                                                       | major  | Green identifies invincibility power-up type.                                      | state-15     |
| interaction-6 | Disable wall and self-collision for 5 seconds when Invincibility is collected                   | major  | Collision immunity creates temporary safety.                                       | visual-3     |
| state-16  | Start 5-second timer when Invincibility is activated                                                | major  | Timed effect requires countdown tracking.                                          | interaction-6 |
| state-17  | Re-enable collisions when Invincibility timer expires                                               | major  | Effect expiration restores collision detection.                                    | state-16     |
| visual-4  | Flash power-up icon during last 2 seconds before expiration                                         | major  | Flashing provides expiration warning.                                              | state-10     |
| content-3 | Display current score                                                                               | major  | Score visibility tracks performance.                                               | None         |
| content-4 | Display current snake length                                                                        | major  | Length shows growth progress.                                                      | None         |
| content-5 | Display high score                                                                                  | major  | High score provides achievement goal.                                              | None         |
| state-18  | Update high score when current score exceeds previous high                                          | major  | High score tracking maintains best performance.                                    | content-5    |
| content-6 | Display active power-ups with remaining time                                                        | major  | Active effects visibility shows current buffs.                                     | None         |
| state-19  | Show timer countdown for each active power-up                                                       | major  | Timer display informs effect duration.                                             | content-6    |
| state-20  | Increase snake speed every 50 points scored                                                         | major  | Progressive difficulty increases challenge.                                        | state-5      |
| content-7 | Display level indicator showing current speed level                                                 | major  | Level visibility shows difficulty progression.                                     | state-20     |
| visual-5  | Display Pause button                                                                                | major  | Pause enables gameplay interruption.                                               | None         |
| interaction-7 | Freeze all game timers and movement when Pause is clicked                                       | major  | Pause functionality stops game state changes.                                      | visual-5     |
| interaction-8 | Display game over screen after collision ends game                                              | major  | Game over screen shows completion.                                                 | interaction-3 |
| content-8 | Display final score on game over screen                                                             | major  | Final score shows total performance.                                               | interaction-8 |
| content-9 | Display length reached on game over screen                                                          | major  | Final length shows growth achievement.                                             | interaction-8 |
| content-10 | Display food eaten count on game over screen                                                       | major  | Food count quantifies collections.                                                 | interaction-8 |
| content-11 | Display power-ups collected count on game over screen                                              | major  | Power-up count quantifies buff usage.                                              | interaction-8 |
| content-12 | Display survival time on game over screen                                                          | major  | Survival duration quantifies gameplay length.                                      | interaction-8 |
| state-21  | Track total game duration from start to game over                                                   | major  | Duration tracking accumulates elapsed time.                                        | content-12   |
| layout-2  | Display leaderboard showing top 5 scores                                                            | major  | Leaderboard provides competitive context.                                          | None         |
| content-13 | Display player name and score for each leaderboard entry                                           | major  | Name and score identify top performers.                                            | layout-2     |
| state-22  | Add current score to leaderboard if it ranks in top 5                                               | major  | Leaderboard update requires ranking comparison.                                    | state-18     |
| state-23  | Pre-populate grid with snake at center and one food on initial load                                 | major  | Initial state provides rich starting render.                                       | None         |
