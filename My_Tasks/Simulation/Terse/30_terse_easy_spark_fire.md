Category: Simulation

Prompt style: Terse

Title: Spark Fire Spread

Prompt: Click cell to ignite. Fire spreads to adjacent cells. Show spread count below grid.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                    | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | ---------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display grid of cells                          | major  | The grid provides the structure where fire spreads.                            | None         |
| 2   | visual      | Display cells in initial state                 | major  | Initial state shows cells before ignition.                                     | C1           |
| 3   | interaction | Ignite clicked cell                            | major  | Clicking ignites a cell to start the fire spread simulation.                   | None         |
| 4   | visual      | Show fire effect on ignited cell               | major  | Visual fire effect shows which cell was clicked.                               | C3           |
| 5   | state       | Spread fire to adjacent cells                  | major  | Spreading to adjacent cells simulates fire propagation.                        | C3           |
| 6   | visual      | Show fire effect on spread cells               | major  | Visual effect shows which cells caught fire.                                   | C5           |
| 7   | content     | Display spread count                           | major  | Showing count gives users feedback on how many cells caught fire.              | None         |
| 8   | layout      | Position spread count below grid               | minor  | Below positioning keeps the count near the simulation area.                    | C7           |
| 9   | state       | Increment count as fire spreads to each cell   | major  | Counting each spread tracks the simulation activity.                           | C7           |

## Justification

The spark fire spread simulator works exactly as expected for fire propagation visualization. A grid of cells displays in initial state. When users click a cell, it ignites showing a fire effect and fire spreads to adjacent cells showing fire effects on spread cells. A spread count displays positioned below the grid and increments as fire spreads to each cell tracking the simulation activity.
