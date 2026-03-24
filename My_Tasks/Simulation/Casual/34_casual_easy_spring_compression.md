Category: Simulation

Prompt style: Casual

Title: Spring Oscillation Motion

Prompt: Want a spring compression simulator showing oscillation physics. Display a vertical coiled spring attached to a fixed ceiling mount at the top with a red weight ball hanging from the bottom end. Below the spring, show a "Pull" button and a "Stop" button. When I click the Pull button, the weight gets pulled down stretching the spring longer, then releases and bounces up and down in a damping oscillation where each bounce gets smaller until it settles back to rest. When I click the Stop button, immediately freeze all motion and hold the spring in its current position.

Required libraries: react, tailwindcss, framer-motion

## Rubric

| #   | ID          | Description                                                | Weight | Rationale                                                                                                               | Dependent On |
| --- | ----------- | ---------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display vertical coiled spring                             | major  | The coiled spring provides the elastic element that demonstrates oscillation physics.                                   | None         |
| 2   | visual      | Display fixed ceiling mount at top                         | major  | The ceiling mount establishes the fixed anchor point from which the spring system hangs.                                | None         |
| 3   | layout      | Attach spring to ceiling mount at top                      | minor  | Attaching the spring to the ceiling creates the realistic constraint needed for proper oscillation behavior.            | C1, C2       |
| 4   | visual      | Display red weight ball at bottom of spring                | major  | The weight ball provides the mass that creates oscillating motion when the spring is displaced.                         | None         |
| 5   | layout      | Attach weight ball to bottom end of spring                 | minor  | Attaching the weight to the spring bottom creates the physical connection needed for energy transfer during oscillation.| C1, C4       |
| 6   | visual      | Display Pull button                                        | major  | The pull button gives users control to initiate the spring oscillation simulation.                                      | None         |
| 7   | visual      | Display Stop button                                        | major  | The stop button allows users to freeze the motion for examination at any point in the oscillation cycle.                | None         |
| 8   | layout      | Position Pull and Stop buttons below spring                | minor  | Placing buttons below the spring keeps controls accessible while maintaining clear view of the oscillating system.      | C6, C7       |
| 9   | interaction | Stretch spring longer when Pull clicked                    | major  | Clicking pull displaces the spring downward to store potential energy for the subsequent oscillation.                   | C6           |
| 10  | state       | Bounce weight up and down in oscillation after release     | major  | Oscillating motion demonstrates the energy conversion between potential and kinetic energy in the spring system.        | C9           |
| 11  | state       | Reduce bounce amplitude with each cycle showing damping    | major  | Decreasing amplitude simulates realistic energy dissipation through air resistance and internal friction.               | C10          |
| 12  | interaction | Freeze all motion immediately when Stop clicked            | major  | Freezing motion on stop allows users to halt the simulation at any moment for detailed observation.                     | C7           |

## Justification

The spring oscillation simulator demonstrates fundamental physics of harmonic motion with damping. A vertical coiled spring displays attached to a fixed ceiling mount at the top, with a red weight ball hanging from the bottom end. Below the spring system, a Pull button and Stop button provide user controls. When users click the Pull button, the weight is pulled down stretching the spring to a longer length, then releases and begins bouncing up and down in oscillation. Each successive bounce has smaller amplitude than the previous, demonstrating realistic damping as the system loses energy and eventually settles back to its resting position. When users click the Stop button at any time during the oscillation, all motion freezes immediately and the spring holds its current position.
