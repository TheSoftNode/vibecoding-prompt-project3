Category: Web_Application

Prompt style: Casual

Title: Color Palette Builder

Prompt: Color palette builder with 5 empty slots. Click a slot to pick a color using a color picker. Each filled slot shows the hex code below it. Lock button on each slot prevents it from changing. Generate button randomizes all unlocked slots to new random colors.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 5 empty color slots                          | major  | The slots provide spaces where users build their color palette.                              | None         |
| 2   | interaction | Open color picker when slot is clicked               | major  | Clicking a slot lets users choose a specific color for that position.                        | None         |
| 3   | visual      | Fill slot with selected color                        | major  | Showing the selected color visually confirms the choice.                                     | C2           |
| 4   | content     | Display hex code below filled slot                   | minor  | The hex code gives users the color value for use in design tools.                            | C3           |
| 5   | visual      | Display lock button on each slot                     | major  | Lock buttons give users control over which colors stay fixed during generation.              | None         |
| 6   | state       | Track locked state for each slot                     | major  | Tracking lock state determines which slots change when generating new colors.                | None         |
| 7   | visual      | Display Generate button                              | major  | The Generate button triggers randomization of unlocked colors.                               | None         |
| 8   | interaction | Randomize unlocked slots when Generate clicked       | major  | Clicking Generate creates new random colors for unlocked slots only.                         | C7           |
| 9   | state       | Keep locked slots unchanged during generation        | major  | Preserving locked colors lets users build palettes around specific color choices.            | C6, C8       |
| 10  | content     | Update hex codes after randomization                 | minor  | Updating hex codes shows the new values for the randomized colors.                           | C8           |

## Justification

The color palette builder works exactly as expected for creating color schemes. Five empty color slots display horizontally. When users click a slot, a color picker opens allowing them to select a color. The slot fills with the selected color and displays its hex code below. Each slot has a lock button that users can toggle to lock that color. A Generate button displays below the slots. When users click Generate, all unlocked slots randomize to new random colors while locked slots remain unchanged. The hex codes update to show the new values for randomized colors.
