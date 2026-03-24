Category: SVG_Generation

Prompt style: Feature_List

Title: Wave Pattern Generator

Prompt: Build a wave pattern generator that creates sine wave SVG paths. Display an SVG canvas showing a smooth wave line starting at the left edge and flowing across to the right edge. Below the canvas, show a slider labeled "Wave Height" that adjusts the amplitude of the wave from flat to tall. Next to that, display a second slider labeled "Wave Frequency" that controls how many wave cycles appear across the canvas. Include a color picker labeled "Wave Color" that changes the stroke color of the wave line in real-time.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                                  | Weight | Rationale                                                                                                  | Dependent On |
| --- | ----------- | -------------------------------------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display an SVG canvas                                                                        | major  | The SVG canvas provides the space for rendering the wave pattern.                                          | None         |
| 2   | visual      | Display a smooth wave line as an SVG path                                                    | major  | The wave line is the core visual element of the generator.                                                 | C1           |
| 3   | layout      | Position wave line starting at the left edge of the canvas                                   | minor  | Starting at the left edge ensures the wave begins at a consistent position.                                | C2           |
| 4   | layout      | Position wave line flowing across to the right edge of the canvas                            | minor  | Flowing to the right edge creates a complete wave pattern across the canvas.                               | C2           |
| 5   | visual      | Display a slider for wave height control                                                     | major  | The height slider lets users adjust the wave amplitude.                                                    | None         |
| 6   | content     | Display label "Wave Height" on the first slider                                              | minor  | Labeling clarifies this slider controls wave amplitude.                                                    | C5           |
| 7   | layout      | Position wave height slider below the canvas                                                 | minor  | Placing controls below separates the wave display from interaction controls.                               | C1, C5       |
| 8   | visual      | Display a slider for wave frequency control                                                  | major  | The frequency slider lets users adjust the number of wave cycles.                                          | None         |
| 9   | content     | Display label "Wave Frequency" on the second slider                                          | minor  | Labeling clarifies this slider controls wave cycle count.                                                  | C8           |
| 10  | layout      | Position wave frequency slider next to the wave height slider                                | minor  | Placing sliders side by side groups related wave controls together.                                        | C5, C8       |
| 11  | visual      | Display a color picker for wave color                                                        | major  | The color picker lets users customize the wave stroke color.                                               | None         |
| 12  | content     | Display label "Wave Color" on the color picker                                               | minor  | Labeling clarifies this picker controls the wave stroke color.                                             | C11          |
| 13  | interaction | Update wave amplitude when wave height slider changes                                        | major  | Adjusting amplitude creates waves ranging from flat to tall.                                               | C5           |
| 14  | interaction | Update wave cycle count when wave frequency slider changes                                   | major  | Adjusting frequency changes how many complete waves appear across the canvas.                              | C8           |
| 15  | interaction | Update wave stroke color in real-time when color picker changes                              | major  | Real-time color updates let users see the wave color change immediately.                                   | C11          |

## Justification

The wave pattern generator works as an interactive SVG wave creator. An SVG canvas displays showing a smooth wave line as an SVG path that starts at the left edge and flows across to the right edge of the canvas. Below the canvas, a slider labeled "Wave Height" appears that adjusts the amplitude of the wave from flat to tall. Next to that, a second slider labeled "Wave Frequency" displays that controls how many wave cycles appear across the canvas. A color picker labeled "Wave Color" appears that changes the stroke color of the wave line. When users adjust the wave height slider, the wave amplitude updates showing waves ranging from flat to tall. When users adjust the wave frequency slider, the number of complete wave cycles across the canvas changes. When users change the color picker, the wave stroke color updates in real-time.
