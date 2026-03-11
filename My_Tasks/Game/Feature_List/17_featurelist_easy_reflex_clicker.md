Category: Game

Prompt style: Feature_List

Title: Reflex Rhythm Clicker

Prompt: Build a reflex rhythm game. Display a pulsing target circle that shrinks and expands repeatedly at 1-second intervals. When clicked during the smallest 20% of the pulse cycle, display "Perfect!" in green near the circle and award 10 points. Otherwise display "Miss!" in red near the circle and award 0 points. Show the current score on screen.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                         | Weight | Rationale                                                                                                         | Dependent On |
| --- | ----------- | ------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display circular target element                                     | major  | Players need a circle to click on for the rhythm timing game.                                                     | None         |
| 2   | state       | Animate circle shrinking and expanding in continuous 1-second cycle | major  | The pulsing animation creates the timing challenge players try to match.                                          | None         |
| 3   | interaction | Display "Perfect!" in green when clicked at smallest 20% of cycle   | major  | Green "Perfect!" tells players they clicked at exactly the right moment.                                          | C1           |
| 4   | content     | Display text "Perfect!" for successful timing                       | minor  | The "Perfect!" text confirms successful clicks even if colors aren't visible.                                     | None         |
| 5   | interaction | Display "Miss!" in red when clicked outside smallest 20% of cycle   | major  | Red "Miss!" tells players their timing was off and they need to click faster or slower.                           | C1           |
| 6   | content     | Display text "Miss!" for failed timing                              | minor  | The "Miss!" text shows failed timing even if colors aren't visible.                                               | None         |
| 7   | state       | Award 10 points for "Perfect!" clicks                               | major  | The 10-point reward gives players a score goal to improve their timing.                                           | None         |
| 8   | state       | Award 0 points for "Miss!" clicks                                   | minor  | Zero points for misses makes only perfect timing count toward the score.                                          | None         |
| 9   | content     | Display current score                                               | major  | The score shows how many perfect clicks players have achieved.                                                    | None         |
| 10  | layout      | Position feedback text near the target circle                       | minor  | Keeping feedback near the circle means players don't have to look away to see results.                            | None         |

## Justification

The application achieved a 90.00% pass rate with one specific failure. A circular target displays on screen and continuously animates, shrinking and expanding in a 1-second pulse cycle. When players click during the smallest 20% of the cycle, "Perfect!" appears in green, the score increases by 10 points, and the current score updates on screen. When clicked outside that window, "Miss!" appears in red, 0 points are awarded, and the score remains unchanged. However, the model failed to position feedback text near the target circle. Instead, feedback appears at the top of the screen in a separate panel far from the circle, requiring players to shift their focus away from the target. This positioning issue caused the failure despite all other functionality working correctly.
