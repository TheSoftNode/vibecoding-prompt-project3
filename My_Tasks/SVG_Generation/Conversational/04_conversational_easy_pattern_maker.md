Category: SVG Generation

Prompt style: Conversational

Title: Custom Stamp Seal Generator

Prompt: I want to create circular stamp seals. Show alphabet buttons labeled A through Z and a row of color swatches. When I click letter buttons, add each letter to an SVG circular seal with the text curved around the border and a star in the center. Clicking a color swatch changes the stamp color. Add a button labeled "Download SVG" to save it.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                        | Weight | Rationale                                                            | Dependent On |
| --- | ----------- | ------------------------------------------------------------------ | ------ | -------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display alphabet buttons A through Z                               | major  | The alphabet buttons let users select letters for the stamp.         | None         |
| 2   | content     | Display letter labels on alphabet buttons                          | major  | Letter labels show users which character each button represents.     | C1           |
| 3   | visual      | Display a row of color swatches                                    | major  | Color swatches let users customize the stamp appearance.             | None         |
| 4   | visual      | Display an SVG circular seal with star in center                   | major  | The circular seal provides the stamp structure.                      | None         |
| 5   | layout      | Position the star icon in the center of the circle                 | minor  | Center placement creates the focal point of the stamp.               | C4           |
| 6   | interaction | Add clicked letter to stamp when alphabet button is clicked        | major  | Clicking letter buttons builds the stamp text.                       | None         |
| 7   | state       | Calculate curved text path positioning around the circle border    | major  | Computing positions places each character correctly along the curve. | C6           |
| 8   | visual      | Display letters curved around the circle border                    | major  | Curved text creates the authentic stamp seal appearance.             | C7           |
| 9   | interaction | Change stamp color when color swatch is clicked                    | major  | Clicking swatches updates the stamp appearance.                      | None         |
| 10  | content     | Label the download button "Download SVG"                           | minor  | The label identifies the export function.                            | None         |
| 11  | interaction | Download the stamp as SVG file when Download SVG button is clicked | major  | Clicking saves the generated stamp.                                  | None         |

## Justification

The custom stamp seal generator works exactly as expected. Alphabet buttons A through Z display with their letter labels. A row of color swatches appears for color selection. An SVG circular seal displays with a star positioned in the center. When users click letter buttons, each letter adds to the stamp with text curved around the circle border. Clicking a color swatch changes the stamp color. A button labeled "Download SVG" saves the stamp as an SVG file.
