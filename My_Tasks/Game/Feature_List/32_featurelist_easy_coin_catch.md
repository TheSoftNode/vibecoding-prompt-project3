Category: Game

Prompt style: Feature_List

Title: Coin Catcher

Prompt: Build a coin catching reaction game with these features: Display a horizontal basket at the bottom of the screen with left and right arrow buttons on either side. When the game starts, coins fall from random horizontal positions at the top of the screen downward at a steady speed. Each coin shows either "1", "2", or "3" on it. When players click the left arrow, move the basket one position left. When players click the right arrow, move the basket one position right. When a falling coin reaches the basket's vertical position and horizontally overlaps the basket, the coin flashes green briefly and is removed. When a coin falls past the basket without being caught, remove that coin.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display horizontal basket at bottom                  | major  | The basket provides the catching target players control.                                     | None         |
| 2   | visual      | Display left and right arrow buttons beside basket   | major  | Arrow buttons give players the controls to move the basket.                                  | None         |
| 3   | state       | Generate coins falling from random top positions     | major  | Random positions create unpredictable catching challenges.                                   | None         |
| 4   | visual      | Display coins falling downward at steady speed       | major  | Falling motion creates the time pressure for catching.                                       | C3           |
| 5   | content     | Show "1", "2", or "3" on each coin                   | major  | Numbers identify each coin visually.                                                         | C3           |
| 6   | interaction | Move basket left when left arrow clicked             | major  | Left movement lets players position to catch coins on the left.                              | C2           |
| 7   | interaction | Move basket right when right arrow clicked           | major  | Right movement lets players position to catch coins on the right.                            | C2           |
| 8   | state       | Detect when coin reaches basket vertical position    | major  | Vertical detection determines the catch timing window.                                       | C4           |
| 9   | state       | Check if coin horizontally overlaps basket           | major  | Horizontal overlap determines if the basket caught the coin.                                 | C8           |
| 10  | visual      | Flash coin green briefly when caught                 | major  | Green flash provides visual feedback that the coin was caught.                               | C9           |
| 11  | interaction | Remove coin from screen when caught                  | major  | Removing caught coins clears them from the game.                                             | C9           |
| 12  | interaction | Remove coin when it falls past basket                | major  | Removing missed coins prevents screen clutter.                                               | C4           |

## Justification

The coin catcher game works exactly as expected for reaction-based catching. A horizontal basket displays at the bottom with left and right arrow buttons beside it. Coins fall from random horizontal positions at the top downward at steady speed. Each coin shows either "1", "2", or "3" on it. When players click the left arrow, the basket moves one position left. When players click the right arrow, the basket moves one position right. When a falling coin reaches the basket's vertical position and horizontally overlaps the basket, the coin flashes green briefly and is removed. When a coin falls past the basket without being caught, that coin is removed.
