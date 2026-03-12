Category: SVG_Generation

Prompt style: Feature_List

Title: Spiral Text Generator

Prompt: Build a spiral text generator. Display a text input field where users can type a message up to 50 characters. Below the input, show an SVG canvas displaying an Archimedean spiral path starting from the center. As users type in the input field, arrange each character along the spiral path in real-time, with each letter positioned at equal intervals along the curve and rotated to follow the spiral's tangent direction.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display text input field and SVG canvas                   | major  | The input and canvas give users the tools to create spiral text.                                                 | None         |
| 2   | visual      | Display Archimedean spiral path from center               | major  | The spiral path shows users the curve their text will follow.                                                    | None         |
| 3   | state       | Limit input to 50 characters maximum                      | minor  | The limit prevents text from getting too long and cramped on the spiral.                                         | None         |
| 4   | state       | Arrange each character along spiral path                  | major  | Character positioning creates the spiral text effect users expect to see.                                        | None         |
| 5   | state       | Position letters at equal intervals along curve           | major  | Equal spacing keeps the text readable and evenly distributed.                                                    | C4           |
| 6   | state       | Rotate each letter to follow spiral tangent direction     | major  | Rotation makes letters align with the curve instead of staying horizontal.                                       | C4           |
| 7   | interaction | Update spiral text in real-time as typing                 | major  | Real-time updates let users see the spiral forming with each keystroke.                                          | None         |
| 8   | layout      | Position SVG canvas below input field                     | minor  | Placing canvas below separates input from output display.                                                        | None         |
| 9   | layout      | Position spiral starting from center of canvas            | minor  | Starting from center creates the classic spiral effect expanding outward.                                        | None         |

## Justification

The spiral text generator works exactly as expected with real-time character positioning along a curved path. A text input field displays at the top where users can type a message. Below the input, an SVG canvas shows an Archimedean spiral path starting from the center and expanding outward. As users type in the input field, each character appears along the spiral path in real-time, positioned at equal intervals along the curve. Each letter rotates to follow the spiral's tangent direction, creating smooth curved text. The input limits messages to 50 characters maximum.
