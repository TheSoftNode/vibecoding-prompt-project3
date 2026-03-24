Category: Simulation

Prompt style: Conversational

Title: Ink Drop in Water

Prompt: I need an ink drop diffusion effect. Click anywhere on a light blue water background to drop dark blue ink that spreads outward in expanding circles. Each ink drop fades gradually as it expands, creating that classic ink-in-water look.

Required libraries: react, tailwindcss, framer-motion

## Rubric

| #   | ID          | Description                                                                      | Weight | Rationale                                                                                                                       | Dependent On |
| --- | ----------- | -------------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display light blue background representing water                                 | major  | Light blue water provides the visual context that makes dark ink drops stand out and appear to diffuse through liquid.         | None         |
| 2   | interaction | Create new ink drop at click position when user clicks on water background       | major  | Click interaction lets users initiate diffusion events at any location they choose.                                             | None         |
| 3   | visual      | Display dark blue ink drop at click location                                     | major  | Dark blue ink creates clear visual contrast against light water background showing where diffusion begins.                      | C2           |
| 4   | state       | Expand ink drop outward from click point in circular shape                       | major  | Circular outward expansion simulates how real ink molecules spread through water from concentrated point to surrounding liquid. | C3           |
| 5   | state       | Animate expansion continuously with growing radius                               | major  | Continuous growth represents the ongoing diffusion process as ink molecules move through water over time.                       | C4           |
| 6   | state       | Fade ink opacity gradually as circle expands                                     | major  | Gradual fading simulates dilution where ink concentration decreases as molecules spread through more water volume.              | C4           |
| 7   | state       | Allow multiple ink drops to exist simultaneously from different clicks           | major  | Multiple simultaneous drops show that each click creates independent diffusion while previous drops continue spreading.         | None         |
| 8   | state       | Remove fully faded ink drops from display when opacity reaches zero or near-zero | minor  | Removing completed animations prevents invisible elements from accumulating and affecting performance.                          | C6           |

## Justification

The ink drop diffusion simulation creates realistic ink-in-water behavior with interactive drop placement. The screen displays a light blue background representing water. When users click anywhere on this background, a dark blue ink drop appears at the exact click position. The ink immediately begins expanding outward in a circular shape with continuously growing radius, simulating how ink molecules diffuse through water. As each circle expands, its opacity fades gradually to represent dilution of ink concentration throughout surrounding water. Users can click multiple times to create several ink drops simultaneously, each spreading independently from its click location. Once an ink drop becomes fully transparent, it is removed from the display.
