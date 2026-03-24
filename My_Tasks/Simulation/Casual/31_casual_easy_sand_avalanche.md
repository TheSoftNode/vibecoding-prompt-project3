Category: Simulation

Prompt style: Casual

Title: Sand Avalanche

Prompt: Sand avalanche sim. Click to drop tan grains that pile up. Show grain counter at top. When pile gets too steep, grains slide down.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                              | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | -------------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display ground surface                                   | major  | Ground provides the base where sand grains accumulate.                         | None         |
| 2   | visual      | Display sand grain elements                              | major  | Sand grains are the particles that create the avalanche effect.                | None         |
| 3   | visual      | Display sand grains in tan color                         | minor  | Tan color makes grains look like realistic sand.                               | C2           |
| 4   | content     | Display a grain counter                                  | major  | Grain counter shows how many grains have been dropped.                         | None         |
| 5   | layout      | Position grain counter at top                            | minor  | Top positioning keeps counter visible above the simulation.                    | C4           |
| 6   | interaction | Drop sand grains when clicked                            | major  | Clicking releases grains to start the simulation.                              | None         |
| 7   | state       | Accumulate grains into a pile                            | major  | Piling up grains creates the unstable slope structure.                         | C6           |
| 8   | state       | Detect when pile gets too steep                          | major  | Steep slope detection triggers the avalanche behavior.                         | C7           |
| 9   | state       | Slide grains downward when pile gets too steep           | major  | Sliding grains simulates real sand avalanche physics.                          | C8           |

## Justification

The sand avalanche simulator works as a physics-based grain accumulation system. A ground surface displays with tan-colored sand grain elements. A grain counter displays at the top. When users click, sand grains drop and accumulate into a pile. As grains stack, the simulation detects when the pile gets too steep. When this happens, grains slide downward to simulate a real sand avalanche.
