Category: Simulation

Prompt style: Feature_List

Title: Gravity Well Orbiter

Prompt: Build a gravity simulation with these features:
- Display a fixed yellow sun at the center and a moving blue planet that orbits around it in an elliptical path
- Show a slider labeled "Orbital Speed" that controls how fast the planet moves along its orbit, updating the animation speed in real-time as the slider changes

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display circular sun element                              | major  | The sun is the gravitational center around which the orbital motion occurs.                                      | None         |
| 2   | content     | Display sun in yellow color                               | minor  | Yellow color makes the sun visually recognizable as a star rather than a planet.                                 | None         |
| 3   | layout      | Position sun at center of simulation area                 | major  | Centering the sun creates the proper orbital dynamics with the planet moving around it.                          | None         |
| 4   | visual      | Display circular planet element                           | major  | The planet is the orbiting body that demonstrates gravitational motion.                                          | None         |
| 5   | content     | Display planet in blue color                              | minor  | Blue color distinguishes the planet from the sun and makes it easy to track.                                     | None         |
| 6   | state       | Move planet along elliptical path around sun              | major  | Elliptical orbit shows realistic gravitational motion instead of a perfect circle.                               | None         |
| 7   | state       | Animate planet movement continuously                      | major  | Continuous animation demonstrates the ongoing orbital mechanics in real-time.                                    | None         |
| 8   | visual      | Display slider control                                    | major  | The slider provides the interface for adjusting the orbital speed parameter.                                     | None         |
| 9   | content     | Display label "Orbital Speed" on slider                   | minor  | Labeling clarifies that the slider controls how fast the planet orbits, not its size or distance.                | None         |
| 10  | state       | Store current orbital speed value from slider             | major  | Storing speed value is necessary to apply the correct animation rate to the planet's motion.                     | None         |
| 11  | interaction | Update planet animation speed when slider is dragged      | major  | Real-time speed updates let users interactively explore how different speeds affect orbital motion.              | C8           |
| 12  | layout      | Position slider below the simulation area                 | minor  | Placing the slider below keeps controls separate from the visual simulation space.                               | None         |

## Justification

The application achieved a 91.67% pass rate with one specific failure. A yellow circular sun displays at the center of the simulation area. A blue circular planet moves along an elliptical path around the sun with continuous animation. A slider labeled "Orbital Speed" appears on screen, storing the current speed value. As users drag the slider, the planet's animation speed updates in real-time, making the orbit faster or slower based on the slider position. However, the model failed to position the slider below the simulation area. Instead, the slider appears to the right side of the simulation or integrated into a control panel alongside it, not below as required. This positioning issue caused the failure despite all other functionality working correctly.
