Category: Game

Prompt style: Conversational

Title: Rock Paper Scissors Game

Prompt: I want to play rock paper scissors against the computer. Show me three buttons for Rock, Paper, and Scissors. When I click one, the computer randomly picks its choice and shows both choices on screen. Display who won the round or if it's a tie. Keep track of wins, losses, and ties with a scoreboard at the top.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| ID            | Description                                                                 | Weight | Rationale                                                                      | Dependent On |
| ------------- | --------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| visual-1      | Display three buttons labeled Rock, Paper, and Scissors                     | major  | Three choice buttons are the core interaction interface.                       | None         |
| interaction-1 | Trigger round when any choice button is clicked                             | major  | Button click initiates game round.                                             | visual-1     |
| state-1       | Generate random computer choice from Rock, Paper, or Scissors               | major  | Random selection creates unpredictable opponent behavior.                      | interaction-1 |
| content-1     | Display player's choice on screen                                           | major  | Player choice display confirms selection.                                      | interaction-1 |
| content-2     | Display computer's choice on screen                                         | major  | Computer choice display reveals opponent selection.                            | state-1      |
| state-2       | Determine round winner by comparing player and computer choices             | major  | Win condition logic implements game rules.                                     | state-1      |
| content-3     | Display "You win" message when player wins the round                        | major  | Win message provides round outcome feedback.                                   | state-2      |
| content-4     | Display "Computer wins" message when computer wins the round                | major  | Loss message provides round outcome feedback.                                  | state-2      |
| content-5     | Display "Tie" message when both choices are the same                        | major  | Tie message handles draw outcome.                                              | state-2      |
| content-6     | Display scoreboard showing wins, losses, and ties                           | major  | Scoreboard tracks cumulative game performance.                                 | None         |
| layout-1      | Position scoreboard at the top of the page                                  | major  | Top placement ensures scoreboard visibility.                                   | content-6    |
| state-3       | Increment wins count when player wins a round                               | major  | Win counter accumulation tracks player success.                                | state-2      |
| state-4       | Increment losses count when computer wins a round                           | major  | Loss counter accumulation tracks player defeats.                               | state-2      |
| state-5       | Increment ties count when round ends in a tie                               | major  | Tie counter accumulation tracks draw outcomes.                                 | state-2      |
