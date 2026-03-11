Category: Game

Prompt style: Terse

Title: Whack-a-Mole

Prompt: 3x3 grid of holes. Random hole highlights in red for 1 second every 2 seconds. Click highlighted hole before it disappears to score 1 point. Display current score. Game runs continuously.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                              | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | -------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 3x3 grid of 9 holes                              | major  | The 3x3 grid provides the game board with multiple targets for the whack-a-mole gameplay.                        | None         |
| 2   | layout      | Arrange holes in 3 rows and 3 columns                    | minor  | Grid arrangement creates the classic whack-a-mole layout with equal spacing.                                     | None         |
| 3   | state       | Randomly select one hole to highlight                    | major  | Random selection makes the game unpredictable and challenging.                                                   | None         |
| 4   | visual      | Highlight selected hole in red color                     | major  | Red highlighting shows players which hole is the active target to click.                                         | None         |
| 5   | state       | Show highlight for 1 second duration                     | major  | The 1-second window creates the timing challenge that defines the game difficulty.                               | None         |
| 6   | state       | Generate new highlight every 2 seconds                   | major  | The 2-second interval between highlights sets the game pace and rhythm.                                          | None         |
| 7   | interaction | Award 1 point when highlighted hole is clicked           | major  | Scoring 1 point for successful clicks provides the reward feedback for good timing.                              | C4           |
| 8   | state       | Award 0 points when clicking non-highlighted holes       | minor  | Zero points for wrong clicks prevents button-mashing and requires focus on the highlighted target.               | None         |
| 9   | state       | Award 0 points when highlight disappears before click    | minor  | Zero points for missed timing teaches players to click faster within the 1-second window.                        | None         |
| 10  | content     | Display current score                                    | major  | Showing the score lets players track their performance and improvement over time.                                | None         |
| 11  | state       | Run game continuously without stopping                   | major  | Continuous gameplay keeps the challenge going indefinitely for extended play sessions.                           | None         |
| 12  | layout      | Position score display above the grid                    | minor  | Placing score above keeps it visible without interfering with clicking the holes below.                          | None         |

## Justification

The application achieved a 91.67% pass rate with one specific failure. A 3x3 grid of 9 holes displays arranged in 3 rows and 3 columns. The game randomly selects one hole and highlights it in red for 1 second. Every 2 seconds, a new random hole highlights. When players click a highlighted hole before it disappears, they score 1 point. Clicking non-highlighted holes or missing the timing window awards 0 points. The current score displays on screen, and the game runs continuously without stopping. However, the model failed to position the score display above the grid. Instead, the score appears below the grid or to the right side in a separate panel, not above as required. This positioning issue caused the failure despite all other functionality working correctly.
