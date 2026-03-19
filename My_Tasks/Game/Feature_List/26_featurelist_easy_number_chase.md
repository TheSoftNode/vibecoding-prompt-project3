Category: Game

Prompt style: Feature_List

Title: Number Chase

Prompt: Build a number chasing game with these features: Display numbers 1 through 5 scattered randomly on screen. Display a target number at the top showing which number to find (starting with 1). When players click the correct target number, hide that number and increment the target to the next number (1→2→3→4→5). Display a mistake counter labeled "Mistakes: 0" that increments each time a player clicks the wrong number. When all 5 numbers are clicked in order, display "Complete!" message in bold text to show the player finished the sequence.

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
| 10  | content     | Display mistake counter labeled "Mistakes: 0"        | major  | Showing mistake counter tells players how many wrong clicks they've made.                    | None         |
| 11  | state       | Increment mistake counter when wrong number clicked  | major  | Incrementing mistakes tracks errors when players click numbers out of sequence.              | C6           |
| 12  | content     | Update displayed mistake count after wrong click     | major  | Updating display shows the current error count in real time.                                 | C11          |
| 13  | state       | Detect when all 5 numbers clicked in order           | major  | Checking completion determines when the player finished the sequential chase.                | C7           |
| 14  | content     | Display "Complete!" message in bold when finished    | major  | Showing completion message tells players they successfully clicked all numbers in sequence.  | C13          |

## Justification

The number chase game works as expected for sequential number hunting with time tracking. Numbers 1 through 5 display scattered randomly across the screen. A target number displays at the top starting with 1. A timer labeled "Time: 0s" displays on screen. When players click a number, the game detects the click and checks if it matches the current target. If correct, the number hides, the target increments to the next number (1→2→3→4→5), and the displayed target updates. When the first correct number is clicked, the timer starts counting up from 0 and updates the displayed time as it progresses. When all 5 numbers are clicked in order, the game detects completion, stops the timer, and displays "Completed in [X]s!" message showing the final time.
