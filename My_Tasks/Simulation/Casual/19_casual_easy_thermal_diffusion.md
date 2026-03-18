Category: Simulation

Prompt style: Casual

Title: Thermal Diffusion Spread

Prompt: Need a heat diffusion simulator showing temperature spread. Show three connected metal rods arranged in a Y-shape labeled "Rod A", "Rod B", "Rod C" radiating from a center junction point. Also show a "Start" button and a "Reset" button below the rods. When I click the Start button, the center junction glows red hot and heat gradually spreads outward from the center along each rod, changing from red to orange to yellow as it moves further out. When I click the Reset button, clear all heat colors and return the rods to their original state.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                | Weight | Rationale                                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display three rods                                         | major  | Showing three rods gives users the structures where heat will diffuse.                              | None         |
| 2   | layout      | Arrange rods in Y-shape from center junction               | minor  | Positioning rods in Y-shape creates the branching diffusion pattern from one source.                | C1           |
| 3   | content     | Display labels "Rod A", "Rod B", "Rod C"                   | major  | Showing labels identifies each rod in the thermal system.                                           | C1           |
| 4   | visual      | Display Start button below rods                            | major  | Showing start button gives users control to begin the diffusion simulation.                         | None         |
| 5   | visual      | Display Reset button below rods                            | major  | Showing reset button gives users control to clear the simulation.                                   | None         |
| 6   | interaction | Start center glowing red hot when Start clicked            | major  | Clicking start initiates the heat source that begins the diffusion animation.                       | C4           |
| 7   | state       | Spread heat outward from center along rods gradually       | major  | Moving heat outward simulates thermal diffusion through the metal rods.                             | C6           |
| 8   | state       | Change color from red to orange as heat spreads            | major  | Transitioning to orange shows temperature decreasing as distance from source increases.             | C7           |
| 9   | state       | Change color from orange to yellow at rod tips             | major  | Transitioning to yellow at tips shows furthest cooling point in the diffusion gradient.             | C8           |
| 10  | interaction | Clear all heat colors when Reset clicked                   | major  | Clicking reset removes all heat visualization from the rods.                                        | C5           |
| 11  | interaction | Return rods to original state when Reset clicked           | major  | Clicking reset restores rods to starting appearance before diffusion began.                         | C10          |

## Justification

The thermal diffusion simulator works as expected for button-controlled heat spreading animation. Three metal rods display arranged in a Y-shape from a center junction point with labels "Rod A", "Rod B", "Rod C". A Start button and a Reset button display below the rods. When users click the Start button, the center junction glows red hot and heat gradually spreads outward from the center along each rod, changing color from red to orange to yellow as it moves further out. When users click the Reset button, all heat colors clear and the rods return to their original state.
