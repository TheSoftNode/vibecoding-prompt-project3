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
| 4   | visual      | Display Start button                                       | major  | Showing start button gives users control to begin the diffusion simulation.                         | None         |
| 5   | layout      | Position Start button below rods                           | minor  | Placing start button below rods keeps controls near the simulation area.                            | C4           |
| 6   | visual      | Display Reset button                                       | major  | Showing reset button gives users control to clear the simulation.                                   | None         |
| 7   | layout      | Position Reset button below rods                           | minor  | Placing reset button below rods groups both controls together.                                      | C6           |
| 8   | interaction | Glow center red hot when Start clicked                     | major  | Clicking start initiates the heat source that begins the diffusion animation.                       | C4           |
| 9   | state       | Spread heat outward from center along rods gradually       | major  | Moving heat outward simulates thermal diffusion through the metal rods.                             | C8           |
| 10  | state       | Spread heat through all three colors red, orange, yellow   | major  | Progressing through the full color gradient shows the complete temperature range from hottest to coolest. | C9           |
| 11  | interaction | Clear all heat colors and return rods to original state when Reset clicked | major  | Clearing heat colors resets the visual state for a fresh simulation run.                            | C6           |

## Justification

The thermal diffusion simulator achieved 90.91% pass rate with one failure. Three metal rods display arranged in a Y-shape from a center junction point with labels "Rod A", "Rod B", "Rod C". A Start button and a Reset button display below the rods. When users click the Start button, the center junction glows red hot and heat gradually spreads outward from the center. However, the heat only spreads along two of the three rods instead of spreading along all three rods with the full red, orange, yellow color progression as required. When users click the Reset button, all heat colors clear and the rods return to their original state.
