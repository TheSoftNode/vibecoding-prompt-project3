Category: Data_Visualization

Prompt style: Conversational

Title: Battery Radial Gauge

Prompt: I'd like to build a battery level gauge as a semicircular arc labeled "Battery Level". The arc displays with green fill calculated to represent 75% charge, with the percentage value "75%" shown in large text below it. Add three preset buttons underneath: "Low (25%)", "Medium (50%)", "Full (100%)". When clicking any preset button, recalculate the arc fill to match that percentage and update the displayed text value.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display "Battery Level" label                        | minor  | The label helps users understand what the gauge is measuring.                                                    | None         |
| 2   | visual      | Display semicircular arc                             | major  | The arc provides the core visual structure for the gauge.                                                        | None         |
| 3   | state       | Calculate arc fill to represent 75% charge           | major  | The fill calculation converts the percentage into a visual representation users can see at a glance.             | None         |
| 4   | visual      | Fill arc with green color                            | minor  | Green color provides quick visual feedback about the battery status.                                             | None         |
| 5   | content     | Display "75%" percentage text below arc              | major  | The percentage number gives users the exact battery level.                                                       | None         |
| 6   | content     | Display "Low (25%)" button                           | major  | The preset button lets users quickly set the battery to low level.                                               | None         |
| 7   | content     | Display "Medium (50%)" button                        | major  | The preset button lets users quickly set the battery to medium level.                                            | None         |
| 8   | content     | Display "Full (100%)" button                         | major  | The preset button lets users quickly set the battery to full level.                                              | None         |
| 9   | interaction | Recalculate arc fill when button is clicked          | major  | Clicking a preset recalculates the arc fill to show the new battery level visually.                              | C6, C7, C8   |
| 10  | interaction | Update percentage text when button is clicked        | major  | Clicking a preset updates the text to display the new battery percentage.                                        | C6, C7, C8   |
| 11  | layout      | Position percentage text below arc                   | minor  | Placing the text below the arc keeps the numerical value near its visual representation.                         | None         |
| 12  | layout      | Position buttons underneath percentage text          | minor  | Placing buttons below separates the controls from the gauge display.                                             | None         |

## Justification

The battery radial gauge works exactly as expected with preset level controls. A semicircular arc displays labeled "Battery Level", with green fill calculated to represent 75% charge. Below the arc, the percentage value "75%" displays in large text. Underneath, three preset buttons appear: "Low (25%)", "Medium (50%)", and "Full (100%)". When users click any preset button, the arc fill recalculates to match that percentage and the displayed text value updates accordingly.
