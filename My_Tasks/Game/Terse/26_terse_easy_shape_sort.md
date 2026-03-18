Category: Game

Prompt style: Terse

Title: Shape Sorter

Prompt: Three shapes fall randomly: circle, square, triangle. Press C for circle, S for square, T for triangle when shape reaches bottom. Correct adds 5 points. Wrong shows miss. Score displays top-left.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display falling shapes                               | major  | Showing shapes gives players the objects they need to sort.                                  | None         |
| 2   | state       | Generate random shapes from circle, square, triangle | major  | Randomizing shapes creates unpredictable sorting challenges each time.                       | None         |
| 3   | state       | Move shapes downward continuously                    | major  | Moving shapes downward creates the timing aspect of the sorting challenge.                   | C1           |
| 4   | visual      | Display bottom line as sorting target                | major  | Showing target line tells players where to time their key presses.                           | None         |
| 5   | layout      | Position bottom line at lower section                | minor  | Placing line at bottom creates the sorting zone for player input.                            | C4           |
| 6   | interaction | Detect C key press from player                       | major  | Detecting C key lets players sort circle shapes.                                             | None         |
| 7   | interaction | Detect S key press from player                       | major  | Detecting S key lets players sort square shapes.                                             | None         |
| 8   | interaction | Detect T key press from player                       | major  | Detecting T key lets players sort triangle shapes.                                           | None         |
| 9   | state       | Check if pressed key matches shape at bottom         | major  | Checking match determines if the player sorted the shape correctly.                          | C6, C7, C8   |
| 10  | state       | Add 5 points to score when correct                   | major  | Adding points rewards players for accurate shape sorting.                                    | C9           |
| 11  | content     | Display miss indicator when wrong key pressed        | major  | Showing miss tells players they pressed the wrong key for that shape.                        | C9           |
| 12  | content     | Display score counter                                | minor  | Showing score lets players track their sorting accuracy performance.                         | C10          |
| 13  | layout      | Position score in top-left corner                    | minor  | Top-left positioning keeps score visible without blocking the falling shapes.                | C12          |
| 14  | state       | Update displayed score after each correct sort       | major  | Updating score shows players their cumulative sorting performance in real time.              | C10          |

## Justification

The shape sorter game works as expected for keyboard-based sorting gameplay with scoring. Falling shapes display and move downward continuously. The game generates random shapes from circle, square, and triangle. A bottom line displays positioned at the lower section as the sorting target. When players press C, S, or T keys, the game detects the keypress and checks if the pressed key matches the shape at the bottom (C for circle, S for square, T for triangle). If correct, 5 points add to the score. If wrong, a miss indicator displays. A score counter displays in the top-left corner and updates after each correct sort showing the cumulative performance.
