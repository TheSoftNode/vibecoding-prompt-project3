Category: Simulation

Prompt style: Casual

Title: Smoke Particle Dispersion

Prompt: Need a smoke particle simulator showing how smoke rises and disperses. Show a gray smoking source at the bottom center of the screen like a small incense stick, with an "Emit" button and a "Clear" button positioned to the right of the source. When I click the Emit button, dark gray smoke particles start releasing upward from the source, rising slowly while gradually fading to lighter gray and becoming more transparent as they move higher, and spreading outward slightly as they disperse into the air. When I click the Clear button, remove all visible smoke particles from the screen instantly.

Required libraries: react, tailwindcss, framer-motion

## Rubric

| #   | ID          | Description                                                     | Weight | Rationale                                                                                                              | Dependent On |
| --- | ----------- | --------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display gray smoking source                                     | major  | The smoke source provides the emission point from which particles originate to begin the dispersion simulation.        | None         |
| 2   | layout      | Position smoking source at bottom center of screen              | minor  | Bottom center positioning establishes the low starting point for smoke to rise upward through the simulation space.   | C1           |
| 3   | visual      | Display Emit button                                             | major  | The emit button gives users control to start the particle emission and rising animation.                               | None         |
| 4   | content     | Label button "Emit"                                             | minor  | The label clearly identifies the button's purpose for releasing smoke particles.                                       | C3           |
| 5   | layout      | Position Emit button to the right of source                     | minor  | Placing the emit button to the right keeps it accessible while avoiding interference with the upward particle path.    | C3           |
| 6   | visual      | Display Clear button                                            | major  | The clear button allows users to remove particles and reset the simulation for a fresh observation.                    | None         |
| 7   | content     | Label button "Clear"                                            | minor  | The label clearly identifies the button's purpose for removing all smoke particles.                                    | C6           |
| 8   | layout      | Position Clear button to the right of source                    | minor  | Positioning the clear button to the right groups it with the emit button for logical control placement.                | C6           |
| 9   | interaction | Release dark gray smoke particles upward when Emit clicked      | major  | Clicking emit initiates the particle generation that demonstrates the smoke rising behavior.                           | C3           |
| 10  | state       | Move smoke particles upward slowly over time                    | major  | Upward motion simulates the buoyancy of warm smoke rising through cooler surrounding air.                              | C9           |
| 11  | state       | Fade particles from dark gray to lighter gray as they rise      | major  | The color transition from dark to light represents the smoke dissipating and mixing with air at higher altitudes.      | C10          |
| 12  | state       | Increase particle transparency as they move higher              | major  | Increasing transparency simulates the gradual disappearance of smoke as it becomes more diluted in the atmosphere.     | C10          |
| 13  | state       | Spread particles outward slightly during upward movement        | major  | Outward spreading represents the natural dispersion of smoke particles as they diffuse laterally through the air.      | C10          |
| 14  | interaction | Remove all visible smoke particles instantly when Clear clicked | major  | Clearing particles resets the visual state immediately so users can restart with a clean simulation space.             | C6           |

## Justification

The smoke particle dispersion simulator creates a realistic visualization of smoke physics and atmospheric dispersion. A gray smoking source displays at the bottom center of the screen resembling a small incense stick or smoldering object. To the right of the source, an Emit button and Clear button provide user controls. When users click the Emit button, dark gray smoke particles begin releasing upward from the source, moving slowly upward to simulate buoyancy. As particles rise, they gradually fade from dark gray to lighter gray while becoming increasingly transparent, representing the smoke dissipating and mixing with surrounding air. The particles also spread outward slightly during their upward journey, demonstrating natural lateral dispersion. When users click the Clear button, all visible smoke particles are removed from the screen instantly, providing a clean slate for the next emission cycle.
