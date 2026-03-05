Category: Game

Prompt style: Feature List

Title: Tic Tac Toe with AI Opponent

Prompt: Build a tic-tac-toe game against computer AI. Display a 3x3 grid of clickable cells. Player is X, computer is O. Player clicks empty cell to place X. Computer automatically places O in a random empty cell after player moves. Detect win conditions: three in a row horizontally, vertically, or diagonally. Detect draw when board is full with no winner. Display "You win!", "Computer wins!", or "Draw!" message. Highlight winning three cells in green. Show score tracking wins, losses, and draws across multiple games. Include difficulty selector with Easy (random moves), Medium (blocks player wins), and Hard (optimal minimax strategy). Display whose turn it is. Reset button clears board for new round while keeping score. On load, show empty board with Easy difficulty selected.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| ID        | Description                                                                                         | Weight | Rationale                                                                          | Dependent On |
| --------- | --------------------------------------------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------- | ------------ |
| layout-1  | Display 3x3 grid of clickable cells                                                                 | major  | Grid structure creates the game board.                                             | None         |
| interaction-1 | Place X in cell when player clicks empty cell                                                   | major  | Player move is primary interaction.                                                | layout-1     |
| state-1   | Track which cells contain X, O, or are empty                                                        | major  | Board state tracking is core game data.                                            | None         |
| state-2   | Generate random empty cell for computer O placement after player moves                              | major  | Computer move automation creates opponent behavior.                                | interaction-1 |
| interaction-2 | Place O in selected cell immediately after player places X                                      | major  | Computer response creates turn-based gameplay.                                     | state-2      |
| state-3   | Check for three X's in a row horizontally                                                           | major  | Horizontal win detection implements win condition.                                 | None         |
| state-4   | Check for three X's in a row vertically                                                             | major  | Vertical win detection implements win condition.                                   | None         |
| state-5   | Check for three X's in a row diagonally                                                             | major  | Diagonal win detection implements win condition.                                   | None         |
| state-6   | Check for three O's in a row horizontally, vertically, or diagonally                                | major  | Computer win detection mirrors player win conditions.                              | None         |
| content-1 | Display "You win!" message when player achieves three in a row                                      | major  | Win message confirms player victory.                                               | state-3      |
| content-2 | Display "Computer wins!" message when computer achieves three in a row                              | major  | Loss message confirms computer victory.                                            | state-6      |
| state-7   | Detect draw when all 9 cells are filled with no winner                                              | major  | Draw detection checks full board without win condition.                            | state-1      |
| content-3 | Display "Draw!" message when board is full with no winner                                           | major  | Draw message handles tie outcome.                                                  | state-7      |
| visual-1  | Highlight winning three cells in green color                                                        | major  | Green highlighting visually identifies winning pattern.                            | state-3      |
| content-4 | Display scoreboard showing wins, losses, and draws                                                  | major  | Score tracking provides cross-game performance history.                            | None         |
| state-8   | Increment wins count when player wins                                                               | major  | Win accumulation tracks player victories.                                          | state-3      |
| state-9   | Increment losses count when computer wins                                                           | major  | Loss accumulation tracks player defeats.                                           | state-6      |
| state-10  | Increment draws count when game ends in draw                                                        | major  | Draw accumulation tracks tie outcomes.                                             | state-7      |
| visual-2  | Display difficulty selector with Easy, Medium, and Hard options                                     | major  | Difficulty selection enables challenge customization.                              | None         |
| state-11  | Use random move selection when Easy difficulty is active                                            | major  | Easy AI uses simplest strategy.                                                    | state-2      |
| state-12  | Block player winning moves when Medium difficulty is active                                         | major  | Medium AI implements defensive strategy checking for player threats.               | state-2      |
| state-13  | Use minimax algorithm for optimal moves when Hard difficulty is active                              | major  | Hard AI implements perfect play strategy.                                          | state-2      |
| content-5 | Display whose turn it is (Player or Computer)                                                       | major  | Turn indicator shows current game state.                                           | None         |
| state-14  | Alternate turn indicator between Player and Computer after each move                                | major  | Turn tracking manages game flow.                                                   | content-5    |
| visual-3  | Display Reset button                                                                                | major  | Reset enables new round initiation.                                                | None         |
| interaction-3 | Clear board when Reset is clicked                                                                | major  | Board clearing resets game state for new round.                                    | visual-3     |
| state-15  | Preserve score counts when board is reset                                                           | major  | Score persistence maintains cross-game statistics.                                 | interaction-3 |
| state-16  | Initialize with empty board and Easy difficulty on page load                                        | major  | Default state establishes initial render condition.                                | None         |
