Category: Game

Prompt style: Feature_List

Title: Echo Repeater

Prompt: Build a sound pattern memory game with these features: Display four colored sound buttons arranged horizontally labeled "Do", "Re", "Mi", "Fa" in blue, green, yellow, and red respectively. Display a "Play Pattern" button below them. When players click "Play Pattern", play back a random sequence of 3 sound buttons by flashing each button for half a second with a small gap between flashes. When players click sound buttons after the pattern plays, flash the clicked button. When the player clicks the 3 correct buttons in the exact same order as the pattern, display "Pattern Matched!" in green text. If the player clicks wrong buttons in wrong order, display "Try Again!" in red text.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display four sound buttons horizontally              | major  | The buttons provide the interface for pattern playback and player input.                     | None         |
| 2   | content     | Label buttons "Do", "Re", "Mi", "Fa"                 | major  | Labels identify each unique sound in the sequence.                                           | C1           |
| 3   | visual      | Color buttons blue, green, yellow, red respectively  | major  | Distinct colors help players track and remember each button position.                        | C1           |
| 4   | visual      | Display "Play Pattern" button below sound buttons    | major  | The button gives players control to start the pattern playback.                              | None         |
| 5   | state       | Generate random sequence of 3 sound buttons          | major  | Randomizing creates different memory challenges each round.                                  | None         |
| 6   | interaction | Flash each button in sequence when pattern plays     | major  | Flashing shows players which buttons form the pattern to remember.                           | C4           |
| 7   | state       | Flash each button for half a second with gaps        | minor  | Timed flashing creates a readable pattern rhythm.                                            | C6           |
| 8   | interaction | Flash clicked button when player clicks it           | major  | Flashing provides feedback that the click was registered.                                    | C1           |
| 9   | state       | Track player's clicked sequence order                | major  | Recording the order checks if it matches the pattern.                                        | C8           |
| 10  | state       | Compare player sequence to pattern sequence          | major  | Comparing determines if the player repeated the pattern correctly.                           | C9           |
| 11  | content     | Display "Pattern Matched!" in green when correct     | major  | Green message confirms the player matched the sequence.                                      | C10          |
| 12  | content     | Display "Try Again!" in red when incorrect           | major  | Red message tells the player their sequence was wrong.                                       | C10          |

## Justification

The echo repeater game works exactly as expected for sound pattern memory. Four colored sound buttons display horizontally labeled "Do", "Re", "Mi", "Fa" in blue, green, yellow, and red. A "Play Pattern" button displays below them. When players click "Play Pattern", a random sequence of 3 sound buttons plays back by flashing each button for half a second with gaps between flashes. When players click sound buttons after the pattern plays, each clicked button flashes. When the player clicks the 3 correct buttons in the exact same order, "Pattern Matched!" displays in green text. If the player clicks wrong buttons in wrong order, "Try Again!" displays in red text.
