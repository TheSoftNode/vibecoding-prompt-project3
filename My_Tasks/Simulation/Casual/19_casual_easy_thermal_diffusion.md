Category: Simulation

Prompt style: Casual

Title: Thermal Diffusion Spread

Prompt: Need a heat diffusion simulator showing temperature spread. Show three connected metal rods arranged in a Y-shape labeled "Rod A", "Rod B", "Rod C" radiating from a center junction point. Start with the center junction glowing red hot. Over time, the heat spreads outward from the center along each rod, changing from red to orange to yellow as it travels further from the source. After 8 seconds, all three rods reach maximum spread with yellow tips. Include a "Reheat" button that resets the center to red hot and restarts the diffusion animation.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                | Weight | Rationale                                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display three rods                                         | major  | Showing three rods gives users the structures where heat will diffuse.                              | None         |
| 2   | layout      | Arrange rods in Y-shape from center junction               | minor  | Positioning rods in Y-shape creates the branching diffusion pattern from one source.                | C1           |
| 3   | content     | Display labels "Rod A", "Rod B", "Rod C"                   | major  | Showing labels identifies each rod in the thermal system.                                           | C1           |
| 4   | state       | Start with center junction glowing red hot                 | major  | Starting center red establishes the initial heat source for diffusion.                              | None         |
| 5   | state       | Spread heat outward from center along rods over time       | major  | Moving heat outward simulates thermal diffusion through the metal rods.                             | C4           |
| 6   | state       | Change color from red to orange as heat spreads            | major  | Transitioning to orange shows temperature decreasing as distance from source increases.             | C5           |
| 7   | state       | Change color from orange to yellow at rod tips             | major  | Transitioning to yellow at tips shows furthest cooling point in the diffusion gradient.             | C6           |
| 8   | state       | Complete diffusion spread after 8 seconds                  | major  | Timing at 8 seconds controls the diffusion rate users observe.                                      | C5           |
| 9   | state       | Reach maximum spread with yellow tips after 8 seconds      | major  | Ending with yellow tips marks the completion state of the thermal diffusion.                        | C7, C8       |
| 10  | visual      | Display Reheat button                                      | minor  | Showing the reheat button gives users a control to restart the simulation.                          | None         |
| 11  | interaction | Reset center to red hot when Reheat clicked                | major  | Clicking reheat returns center to initial hot state so users can observe diffusion again.           | C10          |
| 12  | interaction | Restart diffusion animation when Reheat clicked            | major  | Clicking reheat triggers the spreading animation from the beginning.                                | C11          |

## Justification

The thermal diffusion simulator works as expected for animated heat spreading through connected structures. Three metal rods display arranged in a Y-shape from a center junction point with labels "Rod A", "Rod B", "Rod C". The simulation starts with the center junction glowing red hot. Over time, the heat spreads outward from the center along each rod, changing color from red to orange to yellow as it travels further from the source. After 8 seconds, all three rods reach maximum spread with yellow tips. A reheat button displays and when clicked, resets the center junction to red hot and restarts the diffusion animation.
