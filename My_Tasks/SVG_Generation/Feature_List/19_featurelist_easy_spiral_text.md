Category: SVG_Generation

Prompt style: Feature_List

Title: Spiral Text Generator

Prompt: Build a spiral text generator. Display a heading "Spiral Text Generator" at the top. Below that, display a text input field with placeholder text "Type your message..." where users can type a message. Below the input, show an SVG canvas. Load the input field with sample text "HELLO" on initial render. As users type in the input field, arrange each character along a spiral pattern in real-time, with letters spiraling outward from the center of the canvas.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                  | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | -------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display heading "Spiral Text Generator" at the top    | minor  | The heading tells users what tool they are using.                          | None         |
| 2   | visual      | Display a text input field                            | major  | The input field allows users to type their message for the spiral.         | None         |
| 3   | content     | Display placeholder text "Type your message..." in input field | minor  | The placeholder guides users on what to enter.                             | None         |
| 4   | visual      | Display an SVG canvas                                 | major  | The SVG canvas provides the space to render the spiral text.               | None         |
| 5   | layout      | Position SVG canvas below input field                 | minor  | Placing canvas below separates input from output display.                  | C4           |
| 6   | state       | Load the input field with sample text "HELLO" on initial render | major  | Loading sample text provides initial content for users to see the spiral effect immediately. | None         |
| 7   | layout      | Position letters spiraling outward from center        | major  | Positioning letters in a spiral pattern creates the visual flow outward from the center. | None         |
| 8   | interaction | Update spiral text in real-time as typing             | major  | Real-time updates let users see the spiral forming with each keystroke.    | None         |

## Justification

The spiral text generator works exactly as expected with real-time character positioning along a spiral pattern. A heading "Spiral Text Generator" displays at the top. Below that, a text input field appears with placeholder text "Type your message..." and loads with sample text "HELLO" on initial render. Below the input, an SVG canvas displays. The letters from "HELLO" appear positioned spiraling outward from the center of the canvas. As users type in the input field, the spiral text updates in real-time with each keystroke.
