Category: SVG_Generation

Prompt style: Feature_List

Title: Spiral Text Generator

Prompt: Build a spiral text generator. Display a text input field where users can type a message up to 50 characters. Below the input, show an SVG canvas displaying an Archimedean spiral path starting from the center. As users type in the input field, arrange each character along the spiral path in real-time, with each letter positioned at equal intervals along the curve and rotated to follow the spiral's tangent direction. Display a character counter showing remaining characters out of 50.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display text input field                                  | major  | The input field is where users type the message they want to spiral.                                             | None         |
| 2   | visual      | Display SVG canvas below input                            | major  | The canvas is where the spiral text appears visually.                                                            | None         |
| 3   | visual      | Display Archimedean spiral path from center               | major  | The spiral path shows users the curve their text will follow.                                                    | None         |
| 4   | state       | Limit input to 50 characters maximum                      | minor  | The limit prevents text from getting too long and cramped on the spiral.                                         | None         |
| 5   | state       | Arrange each character along spiral path                  | major  | Character positioning creates the spiral text effect users expect to see.                                        | None         |
| 6   | state       | Position letters at equal intervals along curve           | major  | Equal spacing keeps the text readable and evenly distributed.                                                    | C5           |
| 7   | state       | Rotate each letter to follow spiral tangent direction     | major  | Rotation makes letters align with the curve instead of staying horizontal.                                       | C5           |
| 8   | interaction | Update spiral text in real-time as typing                 | major  | Real-time updates let users see the spiral forming with each keystroke.                                          | None         |
| 9   | state       | Calculate remaining characters out of 50                  | minor  | Counting down shows users how much space they have left for their message.                                       | None         |
| 10  | content     | Display character counter                                 | minor  | The counter displays the remaining characters so users know when to stop.                                        | C9           |
| 11  | layout      | Position spiral starting from center of canvas            | minor  | Starting from center creates the classic spiral effect expanding outward.                                        | None         |

## Justification

The spiral text generator works exactly as expected with real-time character positioning along a curved path. A text input field displays at the top where users can type a message. Below the input, an SVG canvas shows an Archimedean spiral path starting from the center and expanding outward. As users type in the input field, each character appears along the spiral path in real-time, positioned at equal intervals along the curve. Each letter rotates to follow the spiral's tangent direction, creating smooth curved text. The input limits messages to 50 characters maximum. A character counter displays showing the remaining characters out of 50, counting down with each keystroke.
