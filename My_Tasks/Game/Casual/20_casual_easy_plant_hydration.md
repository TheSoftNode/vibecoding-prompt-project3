Category: Game

Prompt style: Casual

Title: Plant Care Puzzle

Prompt: Need a plant watering memory game. Show three empty pots labeled "Cactus", "Fern", and "Succulent" arranged side by side. Below them, display three color buttons: brown, blue, and yellow. Players must remember which color waters which plant: brown for Cactus, blue for Fern, yellow for Succulent. When a player clicks a color button, that color fills the next unfilled pot from left to right only if the color matches the pot's plant type. When all three pots are filled correctly, display "You Win! Plants happy!" message.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                | Weight | Rationale                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display three empty pots                                   | major  | The pots show players the containers that need to be filled.                        | None         |
| 2   | content     | Label pots "Cactus", "Fern", and "Succulent"              | major  | Labels identify which plant type each pot contains for memory matching.            | C1           |
| 3   | layout      | Arrange three pots side by side                            | minor  | Side-by-side arrangement creates clear left-to-right fill order.                    | C1           |
| 4   | visual      | Display three color buttons                                | major  | Color buttons provide the controls for filling pots with water colors.             | None         |
| 5   | content     | Show brown, blue, and yellow button colors                 | major  | The three specific colors correspond to the three plant watering requirements.      | C4           |
| 6   | layout      | Position color buttons below the pots                      | minor  | Below positioning separates controls from target pots.                              | C1, C4       |
| 7   | state       | Track next unfilled pot from left to right                 | major  | Tracking the next pot determines which container receives the clicked color.        | None         |
| 8   | interaction | Fill next unfilled pot when color button clicked           | major  | Clicking a color fills the next pot in sequence creating the gameplay flow.         | C7           |
| 9   | state       | Check if clicked color matches pot's plant type            | major  | Matching logic determines if the player chose the correct water color.              | C8           |
| 10  | state       | Keep pot filled if color matches plant type                | major  | Correct matches stay filled, advancing the game toward completion.                  | C9           |
| 11  | state       | Check if all three pots are correctly filled               | major  | Checking completion determines when the win condition is met.                       | C10          |
| 12  | content     | Display "You Win! Plants happy!" when all pots filled      | major  | Win message provides feedback that the memory puzzle is completed successfully.     | C11          |

## Justification

The Plant Care Puzzle works as expected as a memory matching game with a win condition. Three empty pots display arranged side by side, labeled "Cactus", "Fern", and "Succulent" from left to right. Below them, three color buttons display: brown, blue, and yellow. Players must remember that brown waters Cactus, blue waters Fern, and yellow waters Succulent. The game tracks the next unfilled pot from left to right. When a player clicks a color button, the game checks if the clicked color matches the next pot's plant type. If the color matches (brown for Cactus, blue for Fern, yellow for Succulent), that color fills the pot and it stays filled. If the color doesn't match, nothing happens and the player must try again. When all three pots are correctly filled, the game checks completion and displays "You Win! Plants happy!" message.
