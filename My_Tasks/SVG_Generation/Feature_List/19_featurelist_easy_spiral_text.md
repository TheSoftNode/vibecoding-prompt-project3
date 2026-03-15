Category: SVG_Generation

Prompt style: Feature_List

Title: Spiral Text Generator

Prompt: Build a spiral text generator. Display a text input field with placeholder text "Type your message..." where users can type a message. Below the input, show an SVG canvas with a spiral path starting from the center. As users type in the input field, arrange each character along the spiral path in real-time, with letters spiraling outward from the center.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                  | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | -------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display a text input field                            | major  | The input field allows users to type their message for the spiral.         | None         |
| 2   | content     | Display placeholder text "Type your message..." in input field | minor  | The placeholder guides users on what to enter.                             | None         |
| 3   | visual      | Display an SVG canvas                                 | major  | The SVG canvas provides the space to render the spiral text.               | None         |
| 4   | visual      | Display a spiral path starting from center            | major  | The spiral path shows users the curve their text will follow.              | None         |
| 5   | layout      | Position SVG canvas below input field                 | minor  | Placing canvas below separates input from output display.                  | C3           |
| 6   | layout      | Position spiral starting from center of canvas        | major  | Starting from center creates the classic spiral effect expanding outward.  | C4           |
| 7   | state       | Arrange each character along spiral path              | major  | Character positioning creates the spiral text effect users expect to see.  | None         |
| 8   | state       | Display letters spiraling outward from center         | major  | Letters spiraling outward create the visual effect of text following the curve. | None         |
| 9   | interaction | Update spiral text in real-time as typing             | major  | Real-time updates let users see the spiral forming with each keystroke.    | None         |

## Justification

The spiral text generator works exactly as expected with real-time character positioning along a curved path. A text input field displays at the top with placeholder text "Type your message..." where users can type a message. Below the input, an SVG canvas shows a spiral path starting from the center and expanding outward. As users type in the input field, each character appears along the spiral path in real-time, with letters spiraling outward from the center.
