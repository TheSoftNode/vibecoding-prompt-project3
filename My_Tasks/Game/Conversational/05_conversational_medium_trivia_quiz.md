Category: Game

Prompt style: Conversational

Title: Timed Trivia Quiz

Prompt: I need a trivia quiz game with 8 questions across different categories like Science, History, Geography, and Sports. Each question shows the question text, category tag, difficulty indicator (Easy/Medium/Hard), and four multiple choice options. Add a 20-second countdown timer for each question that turns orange at 10 seconds left and red at 5 seconds. When time runs out, auto-select a random wrong answer and move to next question. Show running score at top. Award points based on difficulty: Easy 5 points, Medium 10 points, Hard 15 points, plus 3 bonus points if answered in under 5 seconds. After completing all questions, display results showing total score, accuracy percentage, category breakdown showing performance per category, time stats showing fastest and slowest answer, and list of all questions with player's answer vs correct answer marked in green or red. Include lifelines: 50/50 removes two wrong answers (usable twice), and Hint shows first letter of correct answer (usable once). Pre-load with 8 sample questions covering all categories and difficulties.

Required libraries: react, tailwindcss, lucide-react, framer-motion

## Rubric

| ID        | Description                                                                                         | Weight | Rationale                                                                          | Dependent On |
| --------- | --------------------------------------------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------- | ------------ |
| state-1   | Pre-load 8 trivia questions with category, difficulty, and correct answer                           | major  | Question dataset establishes game content with metadata.                           | None         |
| content-1 | Display question text, category tag, and difficulty indicator for current question                  | major  | Complete question context enables informed answering.                              | None         |
| visual-1  | Display four multiple choice buttons for each question                                              | major  | Four options create standard multiple choice interface.                            | None         |
| visual-2  | Display 20-second countdown timer                                                                   | major  | Timer creates time pressure for each question.                                     | None         |
| state-2   | Decrement timer by 1 second every second                                                            | major  | Timer countdown is time-evolving state.                                            | visual-2     |
| visual-3  | Apply orange color to timer when 10 seconds or less remain                                          | major  | Orange signals approaching deadline.                                               | state-2      |
| visual-4  | Apply red color to timer when 5 seconds or less remain                                              | major  | Red signals critical time shortage.                                                | state-2      |
| state-3   | Auto-select random incorrect answer when timer reaches zero                                         | major  | Timeout penalty requires random wrong answer selection.                            | state-2      |
| interaction-1 | Advance to next question when timer expires                                                     | major  | Auto-progression ensures game continues after timeout.                             | state-3      |
| content-2 | Display running score at top of page                                                                | major  | Score visibility provides ongoing performance feedback.                            | None         |
| state-4   | Award 5 points for correctly answered Easy questions                                                | major  | Difficulty-based scoring rewards harder questions more.                            | None         |
| state-5   | Award 10 points for correctly answered Medium questions                                             | major  | Medium difficulty earns double Easy points.                                        | None         |
| state-6   | Award 15 points for correctly answered Hard questions                                               | major  | Hard difficulty earns triple Easy points.                                          | None         |
| state-7   | Award 3 bonus points when question answered in under 5 seconds                                      | major  | Speed bonus rewards fast correct answers.                                          | state-2      |
| state-8   | Update running score when points are awarded                                                        | major  | Score accumulation aggregates points across questions.                             | state-4      |
| interaction-2 | Display results screen after all 8 questions are answered                                      | major  | Results screen completes quiz flow.                                                | None         |
| content-3 | Display total score on results screen                                                               | major  | Final score shows cumulative performance.                                          | interaction-2 |
| content-4 | Display accuracy percentage on results screen                                                       | major  | Accuracy provides normalized correctness metric.                                   | interaction-2 |
| state-9   | Calculate accuracy as (correct answers / total questions) × 100                                     | major  | Accuracy calculation is derived percentage.                                        | content-4    |
| content-5 | Display category breakdown showing performance per category on results screen                       | major  | Per-category stats identify knowledge strengths and weaknesses.                    | interaction-2 |
| state-10  | Calculate category performance by grouping questions by category and counting correct answers       | major  | Category aggregation requires filtering and counting.                              | content-5    |
| content-6 | Display fastest answer time on results screen                                                       | major  | Fastest time highlights peak speed.                                                | interaction-2 |
| content-7 | Display slowest answer time on results screen                                                       | major  | Slowest time identifies questions requiring more thought.                          | interaction-2 |
| state-11  | Identify fastest time by finding minimum across all answer times                                    | major  | Minimum finding compares all time values.                                          | content-6    |
| state-12  | Identify slowest time by finding maximum across all answer times                                    | major  | Maximum finding compares all time values.                                          | content-7    |
| content-8 | Display list of all questions with player answer vs correct answer marked green or red              | major  | Question-by-question review enables detailed analysis.                             | interaction-2 |
| visual-5  | Display 50/50 lifeline button                                                                       | major  | 50/50 lifeline provides assistance option.                                         | None         |
| interaction-3 | Remove two incorrect answers when 50/50 is clicked                                              | major  | 50/50 functionality reduces choices to improve odds.                               | visual-5     |
| state-13  | Limit 50/50 lifeline to 2 uses across entire quiz                                                   | major  | Usage cap prevents overuse of lifeline.                                            | interaction-3 |
| visual-6  | Display Hint lifeline button                                                                        | major  | Hint lifeline provides alternative assistance.                                     | None         |
| interaction-4 | Display first letter of correct answer when Hint is clicked                                     | major  | Hint reveals partial answer information.                                           | visual-6     |
| state-14  | Limit Hint lifeline to 1 use across entire quiz                                                     | major  | Single-use cap makes hint a strategic choice.                                      | interaction-4 |
| visual-7  | Disable lifeline buttons after their usage limit is reached                                         | major  | Disabled state prevents exceeding usage caps.                                      | state-13     |
