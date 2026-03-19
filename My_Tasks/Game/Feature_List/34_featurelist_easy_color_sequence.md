Category: Game

Prompt style: Feature_List

Title: Color Sequencer

Prompt: Build a color sequence memory game with these features: Display a target sequence bar at the top showing 4 empty slots. Display five color buttons below labeled "Red", "Blue", "Green", "Yellow", "Purple" in their respective colors. Display a "Generate Sequence" button below the color buttons. When players click "Generate Sequence", randomly select 4 colors and display them as filled circles in the target sequence slots from left to right. Display an input sequence bar below the target showing 4 empty slots. When players click color buttons after a sequence is generated, add that color as a filled circle to the next empty input slot from left to right. When all 4 input slots are filled, compare the input sequence to the target sequence. If they match exactly in order, display "Sequence Match!" in green text. If they don't match, display "Try Again!" in red text and clear all input slots back to empty.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display target sequence bar at top with 4 slots      | major  | The target bar shows the pattern players need to match.                                      | None         |
| 2   | visual      | Display five color buttons below                     | major  | Color buttons provide the input controls for building sequences.                             | None         |
| 3   | content     | Label buttons "Red", "Blue", "Green", "Yellow", "Purple" | major  | Labels identify each color choice.                                                           | C2           |
| 4   | visual      | Color each button in its respective color            | major  | Colors provide visual association with the labels.                                           | C2           |
| 5   | visual      | Display "Generate Sequence" button below colors      | major  | The button lets players create a new pattern to match.                                       | None         |
| 6   | state       | Randomly select 4 colors when button clicked         | major  | Random selection creates different memory challenges.                                        | C5           |
| 7   | visual      | Display selected colors as filled circles in target slots | major  | Filled circles show the sequence pattern visually.                                           | C6           |
| 8   | layout      | Fill target slots from left to right                 | minor  | Left-to-right order establishes the sequence direction.                                      | C7           |
| 9   | visual      | Display input sequence bar below target with 4 slots | major  | The input bar shows where the player's choices appear.                                       | None         |
| 10  | interaction | Add clicked color to next empty input slot           | major  | Adding colors lets players build their matching attempt.                                     | C2           |
| 11  | layout      | Fill input slots from left to right                  | minor  | Left-to-right filling maintains consistent sequence order.                                   | C10          |
| 12  | state       | Detect when all 4 input slots filled                 | major  | Checking fullness determines when to evaluate the match.                                     | C10          |
| 13  | state       | Compare input sequence to target sequence in order   | major  | Comparing determines if the player matched the pattern.                                      | C12          |
| 14  | content     | Display "Sequence Match!" in green when match        | major  | Green message confirms successful pattern matching.                                          | C13          |
| 15  | content     | Display "Try Again!" in red when mismatch            | major  | Red message tells the player their sequence was wrong.                                       | C13          |
| 16  | interaction | Clear all input slots to empty when mismatch         | major  | Clearing lets players attempt the sequence again.                                            | C13          |

## Justification

The color sequencer game works exactly as expected for sequence memory challenges. A target sequence bar displays at the top with 4 empty slots. Five color buttons display below labeled "Red", "Blue", "Green", "Yellow", "Purple" in their respective colors. A "Generate Sequence" button displays below the color buttons. An input sequence bar displays below the target with 4 empty slots. When players click "Generate Sequence", 4 random colors are selected and display as filled circles in the target sequence slots from left to right. When players click color buttons after a sequence is generated, that color adds as a filled circle to the next empty input slot from left to right. When all 4 input slots are filled, the input sequence is compared to the target. If they match exactly in order, "Sequence Match!" displays in green. If they don't match, "Try Again!" displays in red and all input slots clear back to empty.
