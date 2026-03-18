Category: Game

Prompt style: Casual

Title: Word Builder

Prompt: Need a word building game. Show 6 letter buttons displaying the letters G, A, M, E, S, and one random extra letter. When I click letters in order, they add to a word display area at the top. Display a "Check" button that validates if the built word matches the target word "GAMES". If correct, show "Correct!" in green. If wrong, show "Try Again!" in yellow. Display a "Clear" button that empties the word display and lets me start building again.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 6 letter buttons                             | major  | Showing letter buttons gives players the building blocks for word construction.              | None         |
| 2   | state       | Assign letters G, A, M, E, S and one random letter   | major  | Assigning specific letters ensures the target word can be built while the random letter adds variety. | None         |
| 3   | content     | Display letters on buttons                           | major  | Showing letters tells players what characters they can use to build words.                   | C2           |
| 4   | visual      | Display word display area at top                     | major  | Showing display area gives players a space to see their constructed word.                    | None         |
| 5   | layout      | Position word display at top of screen               | minor  | Top positioning keeps the word visible above the letter buttons.                             | C4           |
| 6   | interaction | Add clicked letter to word display                   | major  | Clicking button adds that letter to the word being built.                                    | C1           |
| 7   | content     | Show letters in word display in click order          | major  | Displaying letters in order shows the word the player is constructing.                       | C6           |
| 8   | visual      | Display "Check" button                               | major  | Showing check button gives players control to validate their built word.                     | None         |
| 9   | interaction | Validate if built word matches "GAMES" when checked  | major  | Clicking check compares the player's word to the target word.                                | C8           |
| 10  | state       | Compare built word to target word "GAMES"            | major  | Comparing determines if the player successfully built the correct word.                      | C9           |
| 11  | content     | Display "Correct!" in green when word matches        | major  | Showing correct message tells players they built the target word successfully.               | C10          |
| 12  | content     | Display "Try Again!" in yellow when word wrong       | major  | Showing try again message tells players their word doesn't match the target.                 | C10          |
| 13  | visual      | Display "Clear" button                               | major  | Showing clear button gives players control to restart their word building.                   | None         |
| 14  | interaction | Empty word display when "Clear" clicked              | major  | Clicking clear removes all letters letting players build a fresh word.                       | C13          |

## Justification

The word builder game works exactly as expected for sequential letter selection with validation. Six letter buttons display showing the letters G, A, M, E, S and one random extra letter assigned to each button. A word display area displays positioned at the top of the screen. When players click letters in order, each clicked letter adds to the word display showing letters in click order. A "Check" button displays and when clicked, validates if the built word matches the target word "GAMES" by comparing the two. If the word matches, "Correct!" displays in green. If wrong, "Try Again!" displays in yellow. A "Clear" button displays and when clicked, empties the word display letting players start building again.
