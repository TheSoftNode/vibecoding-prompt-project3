Category: Game

Prompt style: Feature_List

Title: Pattern Lock

Prompt: Build a dot pattern drawing game with these features: Display a 3x3 grid of 9 circular dots all colored gray. Display a "Set Pattern" button and a "Draw Pattern" button below the grid. When players click "Set Pattern", allow clicking and dragging across dots to create a connected pattern, coloring connected dots in blue. When players release the mouse, save this pattern. When players click "Draw Pattern", reset all dots to gray and allow clicking and dragging to draw a new pattern with dots colored in green. When the green pattern matches the blue pattern's exact dot sequence, display "Pattern Unlocked!" message in bold text.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 3x3 grid of 9 circular dots                  | major  | The grid provides the canvas for pattern creation.                                           | None         |
| 2   | visual      | Color all dots gray initially                        | major  | Gray shows the neutral state before any pattern is drawn.                                    | C1           |
| 3   | visual      | Display "Set Pattern" button below grid              | major  | The button lets players create the target pattern to match.                                  | None         |
| 4   | visual      | Display "Draw Pattern" button below grid             | major  | The button lets players attempt to recreate the pattern.                                     | None         |
| 5   | interaction | Enable clicking and dragging across dots when Set Pattern clicked | major  | Drag interaction lets players create connected dot patterns.                                 | C3           |
| 6   | visual      | Color connected dots in blue during Set Pattern      | major  | Blue shows which dots form the target pattern.                                               | C5           |
| 7   | state       | Save pattern sequence when mouse released            | major  | Saving the pattern stores what players need to match later.                                  | C5           |
| 8   | interaction | Reset all dots to gray when Draw Pattern clicked     | major  | Resetting provides a clean canvas for the matching attempt.                                  | C4           |
| 9   | interaction | Enable clicking and dragging across dots when Draw Pattern clicked | major  | Drag interaction lets players attempt to recreate the pattern.                               | C4           |
| 10  | visual      | Color connected dots in green during Draw Pattern    | major  | Green distinguishes the attempt pattern from the target pattern.                             | C9           |
| 11  | state       | Compare green pattern to saved blue pattern sequence | major  | Comparing determines if the player matched the pattern.                                      | C7, C10      |
| 12  | content     | Display "Pattern Unlocked!" in bold when patterns match | major  | The bold message confirms the player successfully recreated the pattern.                     | C11          |

## Justification

The pattern lock game works exactly as expected for pattern matching challenges. A 3x3 grid of 9 gray circular dots displays on screen. A "Set Pattern" button and a "Draw Pattern" button display below the grid. When players click "Set Pattern", they can click and drag across dots to create a connected pattern with dots colored in blue. When the mouse is released, this pattern is saved. When players click "Draw Pattern", all dots reset to gray and players can click and drag to draw a new pattern with dots colored in green. When the green pattern matches the blue pattern's exact dot sequence, "Pattern Unlocked!" message displays in bold text.
