Category: Simulation

Prompt style: Feature_List

Title: Soap Bubble Film Thinning

Prompt: Create a soap bubble film thinning visualization that demonstrates interference patterns during membrane degradation. Display a large circular bubble element centered on the screen with an iridescent surface showing rainbow interference colors. Animate the bubble surface colors to shift gradually and continuously, cycling through the interference spectrum from thick-film purples and blues at the start, transitioning through mid-thickness greens and yellows, and ending with thin-film grays just before the bubble pops. When the color cycle completes and the film becomes critically thin, animate the bubble popping and disappearing completely from view. After the bubble disappears, automatically spawn a new bubble to restart the thinning cycle so users can observe the phenomenon repeatedly.

Required libraries: react, tailwindcss, framer-motion

## Rubric

| #   | ID          | Description                                                                      | Weight | Rationale                                                                                                                       | Dependent On |
| --- | ----------- | -------------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display circular bubble element                                                  | major  | Circular shape represents soap bubble membrane stretched by surface tension into spherical form.                                | None         |
| 2   | layout      | Center bubble element on screen                                                  | minor  | Center positioning makes bubble prominent focal point of the thinning visualization.                                            | C1           |
| 3   | visual      | Display large size bubble element                                                | minor  | Large size makes interference color transitions clearly visible to users.                                                       | C1           |
| 4   | visual      | Display iridescent rainbow colors on bubble surface                              | major  | Rainbow iridescence represents light wave interference creating characteristic soap bubble appearance.                          | None         |
| 5   | state       | Animate colors shifting gradually across bubble surface                          | major  | Gradual shifting simulates continuous thinning where film thickness decreases steadily over time.                               | C4           |
| 6   | state       | Begin color sequence with purples and blues representing thick film              | major  | Purples and blues are interference colors produced when soap film is thickest at cycle start.                                   | C5           |
| 7   | state       | Transition colors through greens and yellows during middle thinning phase        | major  | Greens and yellows represent interference wavelengths appearing as film reaches intermediate thickness.                         | C6           |
| 8   | state       | End color sequence with grays representing critically thin film                  | major  | Grays indicate minimal interference when film becomes extremely thin just before rupture point.                                 | C7           |
| 9   | state       | Pop bubble when color cycle completes and film reaches critical thinness         | major  | Popping represents membrane rupture when surface tension can no longer maintain integrity.                                      | C8           |
| 10  | state       | Remove bubble from display completely after pop animation                        | major  | Complete removal shows bubble lifecycle ending with rupture and disappearance.                                                  | C9           |
| 11  | state       | Spawn new bubble automatically after previous bubble disappears                  | major  | Automatic respawn creates continuous demonstration cycle for repeated observation.                                              | C10          |
| 12  | state       | Restart color thinning sequence from thick-film colors when new bubble spawns    | major  | Restarting from thick-film colors shows each new bubble begins with maximum film thickness.                                     | C11          |

## Justification

The soap bubble film thinning visualization demonstrates thin-film interference physics during membrane degradation. A large circular bubble element appears centered on the screen displaying iridescent rainbow colors on its surface from light wave interference in the soap film. The bubble surface animates with colors shifting gradually and continuously to represent ongoing thinning. The color sequence begins with thick-film purples and blues, transitions through intermediate greens and yellows as thickness decreases, and ends with thin-film grays when the membrane becomes critically thin. When the color cycle completes at critical thinness, the bubble pops and disappears completely from view. Immediately after disappearing, a new bubble spawns automatically in the center, restarting the color thinning sequence from thick-film purples and blues to create a continuous repeating demonstration of the interference phenomenon.
