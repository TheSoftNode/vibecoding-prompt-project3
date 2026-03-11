Category: Game

Prompt style: Feature_List

Title: Reflex Rhythm Clicker

Prompt: Build a reflex rhythm game with these features:
- Display a pulsing target circle that shrinks and expands repeatedly at 1-second intervals
- When clicked during the smallest 20% of the pulse cycle, display "Perfect!" in green and award 10 points; otherwise display "Miss!" in red and award 0 points

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                         | Weight | Rationale                                                                                                         | Dependent On |
| --- | ----------- | ------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display circular target element                                     | major  | The circle is the core game element that players interact with to test their timing.                              | None         |
| 2   | state       | Animate circle shrinking and expanding in continuous 1-second cycle | major  | The pulsing animation creates the timing challenge that defines the rhythm gameplay.                              | None         |
| 3   | state       | Track current size of circle in pulse cycle                         | major  | Tracking size is necessary to determine if clicks happen during the smallest 20% of the cycle.                    | None         |
| 4   | interaction | Display "Perfect!" in green when clicked at smallest 20% of cycle   | major  | Green "Perfect!" feedback rewards players for clicking with precise timing during the optimal window.             | C1           |
| 5   | interaction | Display "Miss!" in red when clicked outside smallest 20% of cycle   | major  | Red "Miss!" feedback tells players their timing was off, helping them learn the rhythm.                           | C1           |
| 6   | state       | Award 10 points for "Perfect!" clicks                               | major  | The 10-point reward for perfect timing is the scoring mechanic that motivates skilled play.                       | None         |
| 7   | state       | Award 0 points for "Miss!" clicks                                   | major  | Zero points for misses creates meaningful distinction between good and bad timing.                                | None         |
| 8   | content     | Display current score                                               | major  | Showing the score lets players track their performance across multiple clicks.                                    | None         |
| 9   | visual      | Display feedback text "Perfect!" or "Miss!" on screen               | major  | Visible feedback text ensures players know immediately whether their click counted as perfect or missed.          | None         |
| 10  | content     | Display color green for "Perfect!" feedback                         | minor  | Green color provides instant visual confirmation of successful timing without reading text.                       | None         |
| 11  | content     | Display color red for "Miss!" feedback                              | minor  | Red color provides instant visual warning of failed timing, reinforcing the negative result.                      | None         |
| 12  | layout      | Position feedback text near the target circle                       | minor  | Placing feedback near the circle keeps players' eyes focused on the target area during rapid clicking.           | None         |

## Justification

The application achieved a 91.67% pass rate with one specific failure. A circular target displays on screen and continuously animates, shrinking and expanding in a 1-second pulse cycle. The game tracks the current size of the circle throughout the cycle. When players click during the smallest 20% of the cycle, "Perfect!" appears in green, the score increases by 10 points, and the current score updates on screen. When clicked outside that window, "Miss!" appears in red, 0 points are awarded, and the score remains unchanged. Feedback text appears near the target circle with appropriate green or red coloring. However, the model failed to position feedback text near the target circle. Instead, feedback appears at the top of the screen or in a separate score panel far from the circle, requiring players to shift their focus away from the target. This positioning issue caused the failure despite all other functionality working correctly.
