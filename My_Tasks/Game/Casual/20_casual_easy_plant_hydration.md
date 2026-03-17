Category: Game

Prompt style: Casual

Title: Plant Hydration Matcher

Prompt: Need a plant watering puzzle game. At the top, show three empty transparent containers arranged side by side: a cactus pot, a fern pot, and a succulent pot. Below them, display three buttons labeled "Cactus", "Fern", and "Succulent" in random order on each load. When a user clicks a button, fill the matching pot with the corresponding water level color: brown for Cactus, blue for Fern, and yellow for Succulent. Keep filled pots filled.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                    | Weight | Rationale                                                                  | Dependent On |
| --- | ----------- | -------------------------------------------------------------- | ------ | -------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display three empty transparent containers                     | major  | The transparent containers show users the target pots to fill.             | None         |
| 2   | layout      | Position containers at the top                                 | minor  | Top positioning creates clear visual separation from the buttons.          | C1           |
| 3   | visual      | Show cactus pot, fern pot, and succulent pot                   | major  | The three different pots identify which container corresponds to each button. | None         |
| 4   | layout      | Arrange the three containers side by side                      | minor  | Side-by-side arrangement makes it easy to see all three targets.           | C1           |
| 5   | visual      | Display three buttons                                          | major  | The buttons provide the controls for filling the pots.                     | None         |
| 6   | layout      | Position the three buttons below the containers                | minor  | Below positioning separates controls from target containers.               | C1, C5       |
| 7   | content     | Label the three buttons "Cactus", "Fern", and "Succulent"      | major  | The labels tell users which button fills which pot.                        | C5           |
| 8   | state       | Display the three buttons in random order on each load         | minor  | Random order varies the button layout each time for variety.               | C5           |
| 9   | interaction | Fill matching pot when corresponding button clicked            | major  | Clicking fills the correct pot based on button label matching plant type. | C7           |
| 10  | interaction | Fill cactus pot with brown when Cactus clicked                 | major  | Brown color provides visual feedback for the cactus water level match.     | None         |
| 11  | interaction | Fill fern pot with blue when Fern clicked                      | major  | Blue color provides visual feedback for the fern water level match.        | None         |
| 12  | interaction | Fill succulent pot with yellow when Succulent clicked          | major  | Yellow color provides visual feedback for the succulent water level match. | None         |
| 13  | state       | Keep filled pots filled after clicking                         | major  | Maintaining fill state ensures pots stay colored after interaction completes. | C10, C11, C12 |

## Justification

The Plant Hydration Matcher works as expected with click-to-fill mechanics. Three empty transparent containers display at the top arranged side by side: a cactus pot, a fern pot, and a succulent pot. Below them, three buttons display in random order labeled "Cactus", "Fern", and "Succulent". When users click the Cactus button, the cactus pot fills with brown and stays filled. When users click the Fern button, the fern pot fills with blue and stays filled. When users click the Succulent button, the succulent pot fills with yellow and stays filled.
