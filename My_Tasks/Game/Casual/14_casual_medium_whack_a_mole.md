Category: Game

Prompt style: Casual

Title: Whack-a-Mole Game

Prompt: Whack-a-mole but make it actually fun. Show 9 holes in a 3x3 grid. Moles randomly pop up for 1 second then hide. Click mole to whack it, scores 10 points. Miss clicks (clicking empty holes) deduct 5 points. Game runs for 30 seconds. Moles pop up faster as time goes on (every 2 seconds at start, every 0.5 seconds at end). Show score, timer, and combo counter. Combo increases when you hit consecutive moles without missing, resets on miss. 3x combo adds 5 bonus points per hit, 5x combo adds 10 bonus points. Display "Combo x3!" notification when combo milestones hit. After 30 seconds show final score, total hits, misses, highest combo reached, and accuracy percentage. Moles should have cute animation popping up/down. Add sound effects toggle. High score persists across games.

Required libraries: react, tailwindcss, lucide-react, framer-motion

## Rubric

| ID        | Description                                                                                         | Weight | Rationale                                                                          | Dependent On |
| --------- | --------------------------------------------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------- | ------------ |
| layout-1  | Display 9 holes arranged in 3x3 grid                                                                | major  | Grid creates game playing field.                                                   | None         |
| state-1   | Randomly select hole for mole to pop up                                                             | major  | Random selection creates unpredictable gameplay.                                   | None         |
| visual-1  | Display mole popping up in selected hole                                                            | major  | Mole appearance creates clickable target.                                          | state-1      |
| state-2   | Keep mole visible for 1 second then hide                                                            | major  | Timed visibility creates time pressure.                                            | visual-1     |
| interaction-1 | Award 10 points when mole is clicked                                                            | major  | Successful hit scores points.                                                      | visual-1     |
| interaction-2 | Deduct 5 points when empty hole is clicked                                                      | major  | Miss penalty discourages random clicking.                                          | layout-1     |
| content-1 | Display current score                                                                               | major  | Score shows performance progress.                                                  | None         |
| state-3   | Update score when points are awarded or deducted                                                    | major  | Score accumulation tracks net performance.                                         | content-1    |
| visual-2  | Display 30-second countdown timer                                                                   | major  | Timer bounds game duration.                                                        | None         |
| state-4   | Start timer countdown on game start                                                                 | major  | Timer initialization begins game.                                                  | visual-2     |
| state-5   | Decrement timer by 1 second every second                                                            | major  | Timer countdown is time-evolving state.                                            | state-4      |
| state-6   | Set mole pop interval to 2 seconds at game start                                                    | major  | Initial interval establishes base difficulty.                                      | None         |
| state-7   | Gradually decrease interval to 0.5 seconds as timer approaches zero                                 | major  | Progressive speed increase creates escalating difficulty.                          | state-5      |
| content-2 | Display combo counter                                                                               | major  | Combo shows consecutive hit streak.                                                | None         |
| state-8   | Increment combo when mole is hit                                                                    | major  | Combo increases on successful hits.                                                | interaction-1 |
| state-9   | Reset combo to zero when empty hole is clicked                                                      | major  | Combo reset penalizes misses.                                                      | interaction-2 |
| state-10  | Award 5 bonus points per hit when combo reaches 3x                                                  | major  | 3x combo multiplier rewards consistency.                                           | state-8      |
| state-11  | Award 10 bonus points per hit when combo reaches 5x                                                 | major  | 5x combo multiplier rewards sustained accuracy.                                    | state-8      |
| visual-3  | Display "Combo x3!" notification when combo reaches 3                                               | major  | Milestone notification celebrates achievement.                                     | state-10     |
| visual-4  | Display "Combo x5!" notification when combo reaches 5                                               | major  | Milestone notification celebrates higher achievement.                              | state-11     |
| state-12  | End game when 30-second timer reaches zero                                                          | major  | Time expiration triggers game end.                                                 | state-5      |
| interaction-3 | Display results screen after game ends                                                          | major  | Results show final performance metrics.                                            | state-12     |
| content-3 | Display final score on results screen                                                               | major  | Final score shows total performance.                                               | interaction-3 |
| content-4 | Display total hits count on results screen                                                          | major  | Hit count quantifies successful clicks.                                            | interaction-3 |
| content-5 | Display misses count on results screen                                                              | major  | Miss count quantifies failed clicks.                                               | interaction-3 |
| content-6 | Display highest combo reached on results screen                                                     | major  | Max combo shows peak streak achievement.                                           | interaction-3 |
| state-13  | Track highest combo by comparing current combo to maximum                                           | major  | Max tracking requires ongoing comparison.                                          | content-6    |
| content-7 | Display accuracy percentage on results screen                                                       | major  | Accuracy provides normalized success metric.                                       | interaction-3 |
| state-14  | Calculate accuracy as (hits / (hits + misses)) × 100                                                | major  | Accuracy is derived percentage.                                                    | content-7    |
| visual-5  | Animate mole popping up and down                                                                    | major  | Animation enhances visual appeal.                                                  | visual-1     |
| visual-6  | Display sound effects toggle button                                                                 | major  | Toggle enables audio control.                                                      | None         |
| interaction-4 | Enable or disable sound effects when toggle is clicked                                          | major  | Toggle functionality controls audio output.                                        | visual-6     |
| state-15  | Persist high score across multiple games                                                            | major  | High score persistence maintains historical best.                                  | None         |
| visual-7  | Display high score on game screen                                                                   | major  | High score visibility provides achievement goal.                                   | state-15     |
| state-16  | Update high score when final score exceeds previous high score                                      | major  | High score update requires comparison and storage.                                 | state-15     |
