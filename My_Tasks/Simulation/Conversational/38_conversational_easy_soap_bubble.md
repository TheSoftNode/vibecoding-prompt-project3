Category: Simulation

Prompt style: Conversational

Title: Soap Bubble Film Thinning

Prompt: I want to see a soap bubble thinning simulation. Show a circular bubble that displays shifting rainbow interference patterns as the film gradually thins. The colors should cycle from thick-film purples and blues through greens and yellows to thin-film grays before the bubble pops and disappears.

Required libraries: react, tailwindcss, framer-motion

## Rubric

| #   | ID          | Description                                                                      | Weight | Rationale                                                                                                                       | Dependent On |
| --- | ----------- | -------------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display circular bubble element                                                  | major  | Circular shape represents soap bubble membrane stretched into spherical form.                                                   | None         |
| 2   | visual      | Display rainbow interference pattern colors on bubble surface                    | major  | Rainbow colors represent light interference in soap film creating iridescent appearance.                                        | None         |
| 3   | state       | Shift colors gradually over time on bubble surface                               | major  | Gradual color shifting simulates how interference patterns change as film thickness decreases.                                  | C2           |
| 4   | state       | Transition colors from thick-film purples and blues initially                    | major  | Purples and blues represent interference colors when soap film is thickest at beginning.                                        | C3           |
| 5   | state       | Progress colors through greens and yellows during middle phase                   | major  | Greens and yellows represent intermediate interference as film continues thinning.                                              | C4           |
| 6   | state       | End color sequence with thin-film grays before pop                               | major  | Grays represent minimal interference when film becomes extremely thin just before rupture.                                      | C5           |
| 7   | state       | Pop bubble after film thinning sequence completes                                | major  | Popping represents membrane rupture when film becomes too thin to maintain surface tension.                                     | C6           |
| 8   | state       | Remove bubble from display after pop                                             | major  | Removing bubble shows the complete lifecycle ending with rupture and disappearance.                                             | C7           |
| 9   | state       | Restart with new bubble after previous bubble disappears                         | minor  | Restarting cycle lets users see repeated thinning simulation without manual interaction.                                        | C8           |

## Justification

The soap bubble film thinning simulator demonstrates interference pattern physics during membrane degradation. A circular bubble element displays with rainbow interference colors on its surface representing light waves interacting in the soap film. Over time, colors shift gradually to simulate thinning effects. The sequence begins with thick-film purples and blues, progresses through intermediate greens and yellows, and ends with thin-film grays just before popping. When the color sequence completes and film reaches critical thinness, the bubble pops and disappears from the display. A new bubble then appears to restart the thinning cycle.
