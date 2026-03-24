Category: Simulation

Prompt style: Casual

Title: Sand Avalanche

Prompt: Sand avalanche sim. Click to drop tan grains that pile up. Show grain counter at top. When pile gets too steep, grains slide down.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                              | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | -------------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display ground surface                                   | major  | Ground provides the base where sand grains accumulate.                         | None         |
| 2   | layout      | Position ground surface at bottom                        | minor  | Bottom positioning places ground where grains land.                            | C1           |
| 3   | visual      | Display sand grain elements                              | major  | Sand grains are the particles that create the avalanche effect.                | None         |
| 4   | visual      | Display sand grains in tan color                         | minor  | Tan color makes grains look like realistic sand.                               | C3           |
| 5   | content     | Display a grain counter                                  | major  | Grain counter shows how many grains have been dropped.                         | None         |
| 6   | layout      | Position grain counter at top                            | minor  | Top positioning keeps counter visible above the simulation.                    | C5           |
| 7   | interaction | Drop sand grains when clicked                            | major  | Clicking releases grains to start the simulation.                              | None         |
| 8   | state       | Move grains downward after drop                          | major  | Downward movement simulates gravity pulling grains to the ground.              | C7           |
| 9   | state       | Accumulate grains into a pile                            | major  | Piling up grains creates the unstable slope structure.                         | C8           |
| 10  | state       | Detect when pile gets too steep                          | major  | Steep slope detection triggers the avalanche behavior.                         | C9           |
| 11  | state       | Slide grains downward when pile gets too steep           | major  | Sliding grains simulates real sand avalanche physics.                          | C10          |
| 12  | state       | Increment grain counter each time grains are dropped     | major  | Counting dropped grains tracks simulation activity.                            | C5, C7       |

## Justification

The sand avalanche simulator works as a physics-based grain accumulation system. A ground surface displays at the bottom with tan-colored sand grain elements. A grain counter displays at the top. When users click, sand grains drop and move downward, falling to accumulate into a pile. The grain counter increments each time grains are dropped. As grains stack, the simulation detects when the pile gets too steep. When this happens, grains slide downward to simulate a real sand avalanche.
