Category: Simulation

Prompt style: Conversational

Title: Magnetic Repulsion Field

Prompt: I need a magnetic field repulsion simulator. Display a large magnet labeled "North Pole" fixed at the center of the screen. Around it, display four smaller magnets labeled "N1", "N2", "N3", "N4" positioned at the four corners. When users click the "Activate" button, the four corner magnets start slowly drifting away from the center magnet in their respective directions, simulating north-north repulsion. Each magnet moves outward at the same speed. Include a "Reset" button that returns all corner magnets to their starting corner positions.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                | Weight | Rationale                                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display large center magnet                                | major  | Showing the center magnet establishes the fixed repulsion source in the field.                      | None         |
| 2   | content     | Display label "North Pole" on center magnet                | minor  | Showing the north pole label identifies the magnetic polarity causing repulsion.                    | C1           |
| 3   | layout      | Position center magnet at middle of screen                 | minor  | Centering the main magnet creates equal repulsion distance to all corners.                          | C1           |
| 4   | visual      | Display four smaller corner magnets                        | major  | Showing four corner magnets gives users the objects that will be repelled.                          | None         |
| 5   | content     | Display labels "N1", "N2", "N3", "N4" on corner magnets    | minor  | Showing labels identifies each corner magnet in the repulsion system.                               | C4           |
| 6   | layout      | Position four magnets at screen corners initially          | minor  | Placing magnets at corners establishes their starting positions before repulsion.                   | C4           |
| 7   | visual      | Display Activate button                                    | major  | Showing the activate button gives users a control to start the repulsion simulation.                | None         |
| 8   | interaction | Start outward drift when Activate button clicked           | major  | Clicking activate initiates the magnetic repulsion movement for all corner magnets.                 | C7           |
| 9   | state       | Move corner magnets away from center in their directions   | major  | Moving magnets outward simulates the north-north magnetic repulsion force.                          | C8           |
| 10  | state       | Move all magnets at same speed                             | major  | Using equal speed for all magnets shows uniform repulsion strength from the center.                 | C9           |
| 11  | state       | Drift corner magnets slowly away from center               | major  | Slow movement simulates gradual magnetic repulsion force over time.                                 | C9           |
| 12  | visual      | Display Reset button                                       | minor  | Showing the reset button gives users a control to restart the simulation.                           | None         |
| 13  | interaction | Return corner magnets to starting positions when Reset clicked | major | Clicking reset moves all magnets back to corners so users can run repulsion again.              | C12          |

## Justification

The magnetic repulsion simulator works as expected for animated field interaction. A large magnet labeled "North Pole" displays fixed at the center of the screen. Four smaller magnets labeled "N1", "N2", "N3", "N4" display positioned at the four corners. An activate button displays and when clicked, starts the four corner magnets drifting slowly away from the center magnet in their respective directions, simulating north-north repulsion. All magnets move outward at the same speed. A reset button displays and when clicked, returns all corner magnets to their starting corner positions.
