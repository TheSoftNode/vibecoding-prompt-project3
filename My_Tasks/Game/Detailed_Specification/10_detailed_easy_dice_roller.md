Category: Game

Prompt style: Detailed Specification

Title: Dice Rolling Simulator

Prompt: Create a dice rolling simulator that allows users to roll between 1 and 6 dice at once. Display a dropdown to select number of dice (1-6). Show a Roll button that generates random values for each die. Display each die result as a large number in a box. Calculate and show the sum of all dice. Include a history section showing the last 5 rolls with timestamp, number of dice rolled, individual die values, and sum. Add a Clear History button. On initial load, display 1 die selected with no rolls yet.

Required libraries: react, tailwindcss

## Rubric

| ID            | Description                                                                 | Weight | Rationale                                                                      | Dependent On |
| ------------- | --------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| visual-1      | Display dropdown to select number of dice with options 1 through 6         | major  | Dice count selection enables variable complexity gameplay.                     | None         |
| visual-2      | Display a Roll button                                                       | major  | Roll button triggers dice randomization.                                       | None         |
| interaction-1 | Generate random value between 1 and 6 for each selected die when Roll is clicked | major  | Random generation creates unpredictable dice outcomes.                         | visual-2     |
| visual-3      | Display each die result as a large number in a box                          | major  | Individual die display shows granular roll results.                            | interaction-1 |
| content-1     | Display sum of all dice values                                              | major  | Sum provides aggregate outcome for multi-die rolls.                            | interaction-1 |
| state-1       | Calculate sum by adding all dice values together                            | major  | Sum calculation is a derived aggregate value.                                  | content-1    |
| layout-1      | Display a history section on the page                                       | major  | History section provides roll tracking area.                                   | None         |
| content-2     | Display last 5 rolls in history with timestamp, dice count, individual values, and sum | major  | Complete roll record enables performance review.                               | None         |
| state-2       | Add new roll to history when Roll button is clicked                         | major  | History accumulation tracks roll sequence.                                     | interaction-1 |
| state-3       | Limit history to show only 5 most recent rolls                              | major  | Five-item cap prevents unlimited history growth.                               | state-2      |
| visual-4      | Display a Clear History button                                              | major  | Clear button enables history reset.                                            | None         |
| interaction-2 | Remove all entries from history when Clear History button is clicked        | major  | History clearing provides fresh start functionality.                           | visual-4     |
| state-4       | Initialize with 1 die selected on page load                                 | major  | Default selection establishes initial render state.                            | None         |
