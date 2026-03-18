Category: Game

Prompt style: Feature_List

Title: Number Chase

Prompt: Build a number chasing game with these features: Display numbers 1 through 5 scattered randomly on screen. Display a target number at the top showing which number to find (starting with 1). When players click the correct target number, hide that number and increment the target to the next number (1→2→3→4→5). Display a timer labeled "Time: 0s" that starts counting up from 0 when the first number is clicked. When all 5 numbers are clicked in order, stop the timer and display "Completed in [X]s!" message showing the final time.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display numbers 1 through 5 on screen                | major  | Showing numbers gives players the targets they need to click in sequence.                    | None         |
| 2   | layout      | Scatter numbers randomly across screen               | minor  | Random positioning creates the hunting challenge for finding numbers.                        | C1           |
| 3   | content     | Display target number at top                         | major  | Showing target tells players which number they need to find and click next.                  | None         |
| 4   | state       | Start with target number 1                           | major  | Starting at 1 establishes the beginning of the sequential clicking challenge.                | None         |
| 5   | interaction | Detect number clicks from player                     | major  | Detecting clicks captures which numbers the player attempts to select.                       | C1           |
| 6   | state       | Check if clicked number matches current target       | major  | Checking match determines if the player clicked the correct sequential number.               | C5           |
| 7   | interaction | Hide number when correct target clicked              | major  | Hiding number shows it has been successfully found and removes it from play.                 | C6           |
| 8   | state       | Increment target to next number after correct click  | major  | Incrementing target progresses the sequence (1→2→3→4→5) for the player to follow.           | C6           |
| 9   | content     | Update displayed target number after increment       | major  | Updating display shows players which number they need to find next.                          | C8           |
| 10  | content     | Display timer labeled "Time: 0s"                     | major  | Showing timer tells players how long they're taking to complete the sequence.                | None         |
| 11  | state       | Start counting up from 0 when first number clicked   | major  | Starting timer on first click measures the time players take for the full sequence.          | C6           |
| 12  | content     | Update displayed time as timer counts up             | major  | Updating display shows players their elapsed time in real time.                              | C11          |
| 13  | state       | Detect when all 5 numbers clicked in order           | major  | Checking completion determines when the player finished the sequential chase.                | C7           |
| 14  | state       | Stop timer when sequence complete                    | major  | Stopping timer captures the final completion time for the challenge.                         | C13          |
| 15  | content     | Display "Completed in [X]s!" message with final time | major  | Showing completion message tells players their total time for clicking all numbers in order. | C14          |

## Justification

The number chase game works as expected for sequential number hunting with time tracking. Numbers 1 through 5 display scattered randomly across the screen. A target number displays at the top starting with 1. A timer labeled "Time: 0s" displays on screen. When players click a number, the game detects the click and checks if it matches the current target. If correct, the number hides, the target increments to the next number (1→2→3→4→5), and the displayed target updates. When the first correct number is clicked, the timer starts counting up from 0 and updates the displayed time as it progresses. When all 5 numbers are clicked in order, the game detects completion, stops the timer, and displays "Completed in [X]s!" message showing the final time.
