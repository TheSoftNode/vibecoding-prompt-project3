Category: Game

Prompt style: Feature_List

Title: Circle Filler

Prompt: Build a circle-filling game with these features: Display 12 circular dots positioned in three horizontal rows of 4 dots each. All dots initially use a white fill and a gray outline. When players click any dot, that dot becomes filled with green color and remains filled permanently. Display a fill counter labeled "Fills: 0" positioned at the top of the screen that increments by one each time players click any dot. When all 12 dots are filled with green color, display "All Filled! Well done!" message in bold text.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                           | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 12 circular dots                                  | major  | The dots provide the interactive objects users fill during the game.                | None         |
| 2   | layout      | Position dots in three horizontal rows of 4 each          | minor  | The row arrangement creates an organized grid that structures the filling gameplay. | C1           |
| 3   | visual      | Display each dot with white fill initially                | minor  | White fill establishes the unfilled starting state before users interact.           | C1           |
| 4   | visual      | Display each dot with gray outline initially              | minor  | Gray outlines define the dot boundaries so users can see what to click.             | C1           |
| 5   | interaction | Fill dot with green when clicked                          | major  | Green filling on click is the core mechanic that makes the game interactive.        | C1           |
| 6   | state       | Keep dot green permanently after filling                  | major  | Permanent green shows users their progress and prevents unfilling.                  | C5           |
| 7   | content     | Display fill counter labeled "Fills: 0"                   | minor  | The counter gives users feedback on how many dots they've filled so far.            | None         |
| 8   | layout      | Position fill counter at top of screen                    | minor  | Top placement keeps the counter visible without blocking the dots below.            | C7           |
| 9   | state       | Increment counter by one when any dot clicked             | major  | Incrementing the count tracks user progress through the filling challenge.          | C5           |
| 10  | content     | Update displayed fill count after each click              | major  | Updating the display keeps the visible count synchronized with actual progress.     | C9           |
| 11  | state       | Detect when all 12 dots are filled with green            | major  | Completion detection determines when the user has successfully finished the game.   | C6           |
| 12  | content     | Display "All Filled! Well done!" in bold when complete    | major  | The bold completion message celebrates finishing and signals the game is over.      | C11          |

## Justification

The circle-filling game works exactly as expected for clicking gameplay with fill tracking. Twelve circular dots display with white fill and gray outline positioned in three horizontal rows of 4 dots each. A fill counter labeled "Fills: 0" displays at the top of the screen. When users click any dot, that dot becomes filled with green color and remains filled permanently. The fill counter increments by one and the displayed count updates after each click. When all 12 dots are filled with green color, "All Filled! Well done!" message displays in bold text.
