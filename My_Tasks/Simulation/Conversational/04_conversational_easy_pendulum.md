Category: Simulation

Prompt style: Conversational

Title: Simple Pendulum Simulation

Prompt: I want a swinging pendulum. Drag the bob to set starting angle, release to swing continuously. Restart button labeled "Reset" positioned at the bottom resets to center.

Required libraries: react, tailwindcss, framer-motion

## Rubric

| #   | ID          | Description                                                                                     | Weight | Rationale                                                                                                                                                         | Dependent On |
| --- | ----------- | ----------------------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Render a pendulum with a visible bob and string                                                 | major  | The bob and string are the main visual elements that represent the physical pendulum being simulated.                                                             | None         |
| 2   | interaction | Allow dragging the bob to set the starting angle                                                | major  | Dragging gives users interactive control to position the pendulum at different angles before releasing it to swing.                                               | None         |
| 3   | interaction | Release the bob to start swinging when drag ends                                                | major  | Releasing initiates the physics simulation based on the angle the user set by dragging.                                                                           | None         |
| 4   | state       | Calculate continuous swinging motion using physics equations for pendulum oscillation            | major  | Physics calculations are essential for creating realistic back-and-forth pendulum motion that continues swinging.                                                 | None         |
| 5   | visual      | Animate the bob swinging smoothly and continuously based on calculated physics                   | major  | Smooth continuous animation brings the computed physics to life visually so users can see the pendulum motion in action.                                          | None         |
| 6   | content     | Display restart button labeled "Reset"                                                           | major  | The "Reset" label clearly identifies the button's purpose for users.                                                                                              | None         |
| 7   | visual      | Display the restart button                                                                       | major  | The restart button provides a clear way for users to reset the simulation.                                                                                        | None         |
| 8   | layout      | Position the restart button at the bottom                                                        | minor  | Bottom placement keeps the button accessible without interfering with the pendulum.                                                                               | None         |
| 9   | interaction | Reset pendulum to center position when restart button is clicked                                | major  | Clicking restart returns the pendulum to its initial centered state so users can start fresh with a new swing.                                                    | C7           |

## Justification

The pendulum simulation works exactly as expected with a visible bob and string. Dragging the bob sets the starting angle, and releasing it initiates smooth continuous swinging motion calculated using physics equations. The pendulum swings back and forth continuously in realistic oscillating motion. At the bottom, the restart button labeled "Reset" resets the pendulum to the center position when clicked, stopping all motion and returning it to the initial state.
