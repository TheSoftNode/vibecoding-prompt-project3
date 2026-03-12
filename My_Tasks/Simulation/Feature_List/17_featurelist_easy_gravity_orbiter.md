Category: Simulation

Prompt style: Feature_List

Title: Gravity Well Orbiter

Prompt: Build a gravity simulation. Display a fixed yellow sun at the center and a moving blue planet that orbits around it in an elliptical path. Below the simulation, show a slider labeled "Orbital Speed" that controls how fast the planet moves along its orbit, updating the animation speed in real-time as the slider changes.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display circular sun element                              | major  | Players need a sun as the center point for the orbital motion.                                                   | None         |
| 2   | content     | Display sun in yellow color                               | minor  | Yellow makes the sun look like a star instead of just another planet.                                            | None         |
| 3   | layout      | Position sun at center of simulation area                 | major  | Centering the sun creates proper orbits with the planet circling around it.                                      | None         |
| 4   | visual      | Display circular planet element                           | major  | The planet is what users watch to see the orbital motion in action.                                              | None         |
| 5   | content     | Display planet in blue color                              | minor  | Blue helps users tell the planet apart from the yellow sun.                                                      | None         |
| 6   | state       | Move planet along elliptical path around sun              | major  | Elliptical paths show more realistic gravity physics than perfect circles.                                       | None         |
| 7   | state       | Animate planet movement continuously                      | major  | Continuous animation keeps the orbit going so users can see the motion pattern.                                  | None         |
| 8   | visual      | Display slider control                                    | major  | The slider gives users a way to adjust how fast the orbit moves.                                                 | None         |
| 9   | content     | Display label "Orbital Speed" on slider                   | minor  | The label tells users the slider controls orbit speed, not distance or size.                                     | None         |
| 10  | interaction | Update planet animation speed when slider is dragged      | major  | Real-time speed changes let users see how different speeds affect the orbit immediately.                         | C8           |
| 11  | layout      | Position slider below the simulation area                 | minor  | Putting the slider below keeps it out of the way of the orbiting planet.                                         | None         |

## Justification

The gravity well orbiter works exactly as expected with orbital animation and speed control. A yellow circular sun displays at the center of the simulation area. A blue circular planet moves continuously along an elliptical path around the sun with smooth animation. Below the simulation, a slider labeled "Orbital Speed" appears on screen. As users drag the slider, the planet's animation speed updates in real-time, making the orbit move faster or slower based on the slider position, demonstrating how orbital velocity affects the planet's movement.
