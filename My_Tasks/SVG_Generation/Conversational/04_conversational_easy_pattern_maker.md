Category: SVG Generation

Prompt style: Conversational

Title: Custom Stamp Seal Generator

Prompt: I want to create circular stamp seals. Show alphabet buttons labeled A through Z and a row of color swatches. Load the stamp with a default star icon in the center. When I click letter buttons, add each letter to an SVG circular seal with the text curved around the border. Clicking a color swatch changes the stamp color. Add a button labeled "Download SVG" to save it.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                        | Weight | Rationale                                                                                         | Dependent On |
| --- | ----------- | ------------------------------------------------------------------ | ------ | ------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display alphabet buttons A through Z                               | major  | Without the alphabet buttons, users have no way to select letters for their stamp.                | None         |
| 2   | content     | Display letter labels on alphabet buttons                          | major  | Letter labels tell users which character each button will add to the stamp.                       | C1           |
| 3   | visual      | Display a row of color swatches                                    | major  | Color swatches give users a visual way to pick their preferred stamp color.                       | None         |
| 4   | visual      | Display an SVG circular seal                                       | major  | The circular seal creates the foundation for the stamp design.                                    | None         |
| 5   | state       | Load the stamp with a default star icon in the center              | major  | Loading a default star provides initial content for the stamp.                                    | C4           |
| 6   | layout      | Position the star icon in the center of the circle                 | minor  | Centering the star makes it the focal point and maintains the classic stamp design.               | C5           |
| 7   | state       | Display letters curved around the circle border                    | major  | Curving letters around the border creates the authentic circular stamp seal look.                 | C8           |
| 8   | interaction | Add clicked letter to stamp when alphabet button is clicked        | major  | This interaction lets users build their custom text by clicking the letters they want.            | None         |
| 9   | interaction | Change stamp color when color swatch is clicked                    | major  | Color switching lets users personalize their stamp to match their preferences.                    | None         |
| 10  | content     | Label the download button "Download SVG"                           | minor  | The label clearly tells users what the button does so they know how to save their stamp.          | None         |
| 11  | interaction | Download the stamp as SVG file when Download SVG button is clicked | major  | Downloading lets users save and use their custom stamp outside the app.                           | None         |

## Justification

The custom stamp seal generator works exactly as expected. Alphabet buttons A through Z display with their letter labels. A row of color swatches appears for color selection. An SVG circular seal displays and loads with a default star icon positioned in the center. When users click letter buttons, each letter adds to the stamp with text curved around the circle border. Clicking a color swatch changes the stamp color. A button labeled "Download SVG" saves the stamp as an SVG file.
