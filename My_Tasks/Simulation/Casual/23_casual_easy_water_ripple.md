Category: Simulation

Prompt style: Casual

Title: Water Ripple Propagation

Prompt: Need a water ripple simulator showing wave propagation. Show five concentric circular rings arranged around a center point labeled "Center", "Ring 1", "Ring 2", "Ring 3", "Ring 4" from innermost to outermost. Also show a "Drop Stone" button and a "Clear" button below the rings. When I click the Drop Stone button, the center point glows blue and ripples spread outward ring by ring, with each ring lighting up in blue sequentially from Ring 1 to Ring 4. When I click the Clear button, all rings return to their original gray color.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                | Weight | Rationale                                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display five concentric circular rings                     | major  | The rings provide the visual structure for ripple propagation.                                      | None         |
| 2   | layout      | Arrange rings around center point                          | minor  | Concentric arrangement creates the ripple pattern radiating from center.                            | C1           |
| 3   | content     | Display labels "Center", "Ring 1", "Ring 2", "Ring 3", "Ring 4" | major  | Labels identify each ring position in the propagation sequence.                                     | C1           |
| 4   | visual      | Display Drop Stone button                                  | major  | The button gives users control to trigger the ripple simulation.                                    | None         |
| 5   | layout      | Position Drop Stone button below rings                     | minor  | Bottom positioning keeps the button near the simulation area.                                       | C4           |
| 6   | visual      | Display Clear button                                       | major  | The button gives users control to reset the simulation.                                             | None         |
| 7   | layout      | Position Clear button below rings                          | minor  | Bottom positioning groups both controls together.                                                   | C6           |
| 8   | interaction | Glow center point blue when Drop Stone clicked             | major  | Blue glow shows the initial impact point that generates ripples.                                    | C4           |
| 9   | state       | Light up rings sequentially from Ring 1 to Ring 4          | major  | Sequential activation simulates ripples propagating outward through water.                          | C8           |
| 10  | visual      | Light up rings in blue color                               | major  | Blue color represents the water ripple wave passing through each ring.                              | C9           |
| 11  | interaction | Return all rings to gray when Clear clicked                | major  | Gray color resets the visual state for a fresh simulation.                                          | C6           |

## Justification

The water ripple propagation simulator works exactly as expected for wave visualization. Five concentric circular rings display arranged around a center point with labels "Center", "Ring 1", "Ring 2", "Ring 3", "Ring 4" from innermost to outermost. A Drop Stone button and a Clear button display below the rings. When users click the Drop Stone button, the center point glows blue and ripples spread outward ring by ring, with each ring lighting up in blue sequentially from Ring 1 to Ring 4. When users click the Clear button, all rings return to their original gray color.
