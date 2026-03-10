Category: Simulation

Prompt style: Casual

Title: Gas Diffusion Simulator

Prompt: Simulate gas molecules spreading from concentrated area to fill entire space. Start with 20 blue particles clustered in left half and 20 red particles in right half. Each particle moves randomly in any direction with constant speed. Particles bounce off walls when hitting edges. Color-code the background in 4 quadrants showing particle density - darker shading means more particles in that area. Update density shading every second based on particle positions. Display total particle count "40 particles" at the top.

Required libraries: react, tailwindcss, framer-motion, lucide-react

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                                         | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 20 blue particles                                        | major  | Blue particles visually represent one type of gas molecule in the simulation.                                                     | None         |
| 2   | layout      | Position blue particles clustered in left half of space          | minor  | Left-half clustering creates the initial concentrated area where blue gas starts.                                                 | None         |
| 3   | visual      | Display 20 red particles                                         | major  | Red particles visually represent the second type of gas molecule in the simulation.                                               | None         |
| 4   | layout      | Position red particles clustered in right half of space          | minor  | Right-half clustering creates the initial concentrated area where red gas starts.                                                 | None         |
| 5   | state       | Move each particle randomly in any direction with constant speed | major  | Random motion simulates the chaotic movement of gas molecules spreading through space.                                            | None         |
| 6   | state       | Bounce particles off walls when hitting edges                    | major  | Wall collisions keep particles contained within the space like gas molecules in a closed container.                               | None         |
| 7   | layout      | Divide background space into 4 quadrants                         | minor  | Four equal sections create a grid for comparing particle density across different regions.                                        | None         |
| 8   | visual      | Color-code each quadrant with darker shading for higher particle density | major  | Density-based shading creates a visual heatmap where darker colors show more concentrated areas.                                  | C7           |
| 9   | state       | Calculate particle count in each quadrant                        | major  | Counting particles per quadrant determines the density level for shading each area.                                               | None         |
| 10  | state       | Update density shading every second based on particle positions  | major  | Regular updates show how particle density changes over time as gases diffuse and mix.                                             | C9           |
| 11  | content     | Display total particle count "40 particles" at top               | major  | Showing the total count tells users how many gas molecules are in the simulation.                                                 | None         |
| 12  | interaction | Start simulation automatically when page loads                    | major  | Auto-start lets users immediately see the diffusion process without needing to click anything.                                    | None         |

## Justification

The gas diffusion simulator demonstrates how gas molecules spread from concentrated areas to fill available space through random motion. Twenty blue particles start clustered in the left half while 20 red particles start in the right half, with the total particle count "40 particles" displayed at the top. Each particle moves randomly in any direction at constant speed, simulating molecular motion. When particles hit the edges, they bounce off walls like gas molecules in a closed container. The background is color-coded into 4 quadrants with darker shading indicating higher particle density in that area. This density visualization updates every second based on current particle positions, creating a visual heatmap showing how the gases diffuse and mix over time.
