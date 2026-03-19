Category: Game

Prompt style: Feature_List

Title: Stack Balancer

Prompt: Build a block stacking balance game with these features: Display a horizontal balance beam in the center of the screen with a center pivot point marked. Display three block buttons labeled "Small" (1 kg), "Medium" (2 kg), and "Large" (3 kg) positioned below the beam. When players click a block button, add that block to a random position on either the left or right side of the beam with the block visually appearing on the beam. When the total weight difference between left and right sides exceeds 5 kg, display "Beam Collapsed!" message in red text.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display horizontal balance beam in center            | major  | The beam provides the visual foundation for the balancing mechanic.                          | None         |
| 2   | visual      | Mark center pivot point on beam                      | minor  | The pivot shows where the beam balances from.                                                | C1           |
| 3   | visual      | Display three block buttons below beam               | major  | The buttons give players the controls to add weight to the beam.                             | None         |
| 4   | content     | Label buttons "Small" (1 kg), "Medium" (2 kg), "Large" (3 kg) | major  | Labels tell players the weight value of each block choice.                                   | C3           |
| 5   | interaction | Add block to beam when button clicked                | major  | Clicking button adds weight creating the stacking challenge.                                 | C3           |
| 6   | state       | Place block at random position on left or right side | major  | Random placement creates unpredictable weight distribution.                                  | C5           |
| 7   | visual      | Display block visually on beam at placement position | major  | Showing blocks on the beam provides visual feedback of stacking.                             | C6           |
| 8   | state       | Calculate total weight on left and right sides       | major  | Weight calculation determines the balance state of the beam.                                 | C6           |
| 9   | content     | Display tilt indicator showing heavier side          | major  | The indicator tells players which direction the beam is leaning.                             | C8           |
| 10  | state       | Detect when weight difference exceeds 5 kg           | major  | Checking the threshold determines if the beam collapsed.                                     | C8           |
| 11  | content     | Display "Beam Collapsed!" in red when limit exceeded | major  | The red message tells players the beam failed from imbalance.                                | C10          |
| 12  | interaction | Disable all block buttons when beam collapses        | major  | Disabling buttons ends the game after collapse.                                              | C10          |

## Justification

The stack balancer game works exactly as expected for weight balancing challenges. A horizontal balance beam displays in the center with a center pivot point marked. Three block buttons display below labeled "Small" (1 kg), "Medium" (2 kg), and "Large" (3 kg). When players click a block button, that block adds to a random position on either the left or right side of the beam and the block displays visually on the beam at that position. A tilt indicator displays showing which side is heavier. When the weight difference exceeds 5 kg on either side, "Beam Collapsed!" message displays in red and all block buttons become disabled.
