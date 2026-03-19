Category: Game

Prompt style: Feature_List

Title: Circle Filler

Prompt: Build a circle-filling game with these features: Display 12 circular dots positioned in three horizontal rows of 4 dots each. All dots initially use a white fill and a gray outline. When players click any dot, that dot becomes filled with green color and remains filled permanently. Display a fill counter labeled "Fills: 0" positioned at the top of the screen that increments by one each time players click any dot. When all 12 dots are filled with green color, display "All Filled! Well done!" message in bold text.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                           | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 12 circular dots                                  | major  | Showing dots gives players the objects they need to fill.                           | None         |
| 2   | layout      | Position dots in three horizontal rows of 4 each          | minor  | Arranging in rows creates an organized grid layout for the filling game.            | C1           |
| 3   | visual      | Display each dot with white fill initially                | minor  | Showing white fill makes the initial unfilled state visible to players.             | C1           |
| 4   | visual      | Display each dot with gray outline initially              | minor  | Showing gray outline defines the dot boundaries clearly.                            | C1           |
| 5   | interaction | Fill dot with green when clicked                          | major  | Clicking dot changes its color showing the filling action.                          | C1           |
| 6   | state       | Keep dot green permanently after filling                  | major  | Maintaining green color shows the dot stays filled and won't revert.                | C5           |
| 7   | content     | Display fill counter labeled "Fills: 0"                   | minor  | Showing counter tells players how many dots they've filled.                         | None         |
| 8   | layout      | Position fill counter at top of screen                    | minor  | Top positioning keeps counter visible while players fill dots below.                | C7           |
| 9   | state       | Increment counter by one when any dot clicked             | major  | Incrementing count tracks the total number of fills the player makes.               | C5           |
| 10  | content     | Update displayed fill count after each click              | major  | Updating display shows the current fill count in real time.                         | C9           |
| 11  | state       | Detect when all 12 dots are filled with green            | major  | Checking completion determines when the player has filled every dot.                | C6           |
| 12  | content     | Display "All Filled! Well done!" in bold when complete    | major  | Showing bold completion message makes it prominent and tells players they finished. | C11          |

## Justification

The circle-filling game works exactly as expected for clicking gameplay with fill tracking. Twelve circular dots display with white fill and gray outline positioned in three horizontal rows of 4 dots each. A fill counter labeled "Fills: 0" displays at the top of the screen. When players click any dot, that dot becomes filled with green color and remains filled permanently. The fill counter increments by one and the displayed count updates after each click. When all 12 dots are filled with green color, "All Filled! Well done!" message displays in bold text.
