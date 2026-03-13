Category: Data_Visualization

Prompt style: Conversational

Title: Battery Radial Gauge

Prompt: I'd like to display a battery level indicator as a radial gauge. Show a semicircular arc at the top labeled "Battery Level". The arc should fill from left to right with green color representing 75% charge. Below the arc, display the percentage value "75%" in large text. Add a slider underneath labeled "Adjust Level" that lets users drag to change the battery percentage from 0% to 100%. When the slider moves, update both the arc fill amount and the percentage text to match the new value.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display "Battery Level" label above arc              | minor  | The label tells users what the gauge represents.                                                                 | None         |
| 2   | visual      | Display semicircular arc at top                      | major  | The arc provides the visual gauge structure.                                                                     | None         |
| 3   | visual      | Fill arc with green color representing 75% charge    | major  | The green fill shows the initial battery level visually.                                                         | None         |
| 4   | content     | Display "75%" percentage text below arc              | major  | The percentage gives users the precise numerical value.                                                          | None         |
| 5   | content     | Display slider labeled "Adjust Level"                | major  | The slider and label give users the control to change battery level.                                             | None         |
| 6   | state       | Set slider range from 0% to 100%                     | minor  | The range defines the valid battery percentage values.                                                           | None         |
| 7   | interaction | Update arc fill when slider moves                    | major  | Moving the slider changes the visual gauge fill to match the new level.                                          | C5           |
| 8   | interaction | Update percentage text when slider moves             | major  | Moving the slider updates the numerical display to show the new value.                                           | C5           |
| 9   | layout      | Position arc at top of display                       | minor  | Placing the arc at the top creates clear visual hierarchy.                                                       | None         |
| 10  | layout      | Position percentage text below arc                   | minor  | Putting text below the arc keeps the numerical value near its visual representation.                             | None         |
| 11  | layout      | Position slider underneath percentage text           | minor  | Placing the slider below separates controls from the gauge display.                                              | None         |

## Justification

The battery radial gauge works exactly as expected with interactive level adjustment. A semicircular arc displays at the top labeled "Battery Level", filled with green color representing 75% charge. Below the arc, the percentage value "75%" displays in large text. Underneath, a slider labeled "Adjust Level" allows users to drag and change the battery percentage from 0% to 100%. When users move the slider, both the arc fill amount and the percentage text update in real-time to match the new value selected.
