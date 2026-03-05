Category: Game

Prompt style: Terse

Title: Word Scramble Game

Prompt: Word scramble game with 10 preset words. Display scrambled letters. Player types guess in input, clicks Submit. Show "Correct!" in green or "Wrong!" in red. Award 10 points for correct answer, 5 bonus points if answered in under 10 seconds. Display timer counting up from 0. Skip button loads next word. Score shows total points. Words answered correctly show with green checkmark, wrong answers show red X. After all 10 words, show results screen with final score, time breakdown per word, and average solve time. Highlight fastest solve in gold. Restart button begins new game with reshuffled words.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| ID            | Description                                                                 | Weight | Rationale                                                                      | Dependent On |
| ------------- | --------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| state-1       | Pre-load 10 words for the game                                              | major  | Word dataset establishes game content.                                         | None         |
| state-2       | Scramble letters of current word randomly                                   | major  | Letter randomization creates the puzzle challenge.                             | state-1      |
| content-1     | Display scrambled letters on screen                                         | major  | Scrambled display presents the puzzle to solve.                                | state-2      |
| visual-1      | Display input field for player guess                                        | major  | Input enables guess submission.                                                | None         |
| visual-2      | Display Submit button                                                       | major  | Submit button triggers answer evaluation.                                      | None         |
| interaction-1 | Compare player guess to original word when Submit is clicked                | major  | Comparison logic validates answer correctness.                                 | visual-2     |
| content-2     | Display "Correct!" message in green when guess matches original word        | major  | Success feedback confirms correct answer with positive color.                  | interaction-1 |
| content-3     | Display "Wrong!" message in red when guess does not match original word     | major  | Failure feedback indicates incorrect answer with warning color.                | interaction-1 |
| visual-3      | Display timer counting up from 0 seconds                                    | major  | Timer tracks solving duration for each word.                                   | None         |
| state-3       | Increment timer by 1 second every second                                    | major  | Timer incrementation creates time-evolving state.                              | visual-3     |
| state-4       | Stop timer when answer is submitted                                         | major  | Timer stop captures solve duration at submission moment.                       | interaction-1 |
| state-5       | Award 10 base points for correct answer                                     | major  | Base scoring provides standard reward for correctness.                         | interaction-1 |
| state-6       | Award 5 bonus points when correct answer is given in under 10 seconds       | major  | Speed bonus rewards fast solving with conditional points.                      | state-4      |
| content-4     | Display total score showing sum of base and bonus points                    | major  | Score display shows cumulative performance metric.                             | None         |
| state-7       | Update total score when points are awarded                                  | major  | Score accumulation aggregates points across all words.                         | state-5, state-6 |
| visual-4      | Display Skip button                                                         | major  | Skip button enables moving to next word without answering.                     | None         |
| interaction-2 | Load next word when Skip button is clicked                                  | major  | Skip functionality allows bypassing difficult words.                           | visual-4     |
| state-8       | Mark word as correct with green checkmark when answered correctly           | major  | Visual marker tracks correctly answered words.                                 | interaction-1 |
| state-9       | Mark word as wrong with red X when answered incorrectly                     | major  | Visual marker tracks incorrectly answered words.                               | interaction-1 |
| content-5     | Display list showing which words were answered correctly or incorrectly     | major  | Word status list provides progress overview.                                   | None         |
| state-10      | Detect when all 10 words have been attempted or skipped                     | major  | Completion detection triggers results screen.                                  | None         |
| interaction-3 | Display results screen when all words are complete                          | major  | Results transition completes game flow.                                        | state-10     |
| content-6     | Display final score on results screen                                       | major  | Final score shows total performance outcome.                                   | interaction-3 |
| content-7     | Display time breakdown showing solve time for each word on results screen   | major  | Per-word timing provides detailed performance analysis.                        | interaction-3 |
| content-8     | Display average solve time on results screen                                | major  | Average time is aggregate statistic across all attempted words.                | interaction-3 |
| state-11      | Calculate average solve time by summing all times and dividing by word count | major  | Average calculation requires aggregation and division.                         | content-8    |
| visual-5      | Highlight fastest solve time in gold on results screen                      | major  | Gold highlighting celebrates peak performance moment.                          | content-7    |
| state-12      | Identify fastest time by finding minimum value across all solve times       | major  | Minimum finding requires comparison across all time values.                    | visual-5     |
| visual-6      | Display Restart button on results screen                                    | major  | Restart button enables new game initiation.                                    | None         |
| interaction-4 | Reshuffle words and reset all state when Restart is clicked                 | major  | Restart creates new game with randomized word order.                           | visual-6     |
| state-13      | Reset timer to 0 when new word is loaded                                    | major  | Timer reset ensures each word starts with clean time tracking.                 | interaction-2 |
