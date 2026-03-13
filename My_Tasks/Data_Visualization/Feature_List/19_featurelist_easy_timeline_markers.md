Category: Data_Visualization

Prompt style: Feature_List

Title: Historical Event Timeline

Prompt: Build a historical event timeline. Display a horizontal line across the screen representing years from 2020 to 2025. Along the timeline, show 4 event markers positioned at their correct years: "Launch" at 2020, "Expansion" at 2021, "Milestone" at 2023, and "Today" at 2025. Each marker appears as a circle on the timeline with its label above. Below the timeline, display a dropdown menu labeled "Jump to Year" containing options for 2020, 2021, 2023, and 2025. When users select a year from the dropdown, the corresponding event marker on the timeline pulses with an animation to draw attention to that event.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display horizontal line representing years 2020-2025  | major  | The timeline line provides the base structure for showing events across time.                                    | None         |
| 2   | visual      | Display circle marker for "Launch" at 2020           | major  | The marker shows the first event's position on the timeline.                                                     | None         |
| 3   | visual      | Display circle marker for "Expansion" at 2021        | major  | The marker shows the second event's position on the timeline.                                                    | None         |
| 4   | visual      | Display circle marker for "Milestone" at 2023        | major  | The marker shows the third event's position on the timeline.                                                     | None         |
| 5   | visual      | Display circle marker for "Today" at 2025            | major  | The marker shows the fourth event's position on the timeline.                                                    | None         |
| 6   | content     | Display "Launch" label above 2020 marker             | minor  | The label identifies what happened at that point in time.                                                        | None         |
| 7   | content     | Display "Expansion" label above 2021 marker          | minor  | The label identifies what happened at that point in time.                                                        | None         |
| 8   | content     | Display "Milestone" label above 2023 marker          | minor  | The label identifies what happened at that point in time.                                                        | None         |
| 9   | content     | Display "Today" label above 2025 marker              | minor  | The label identifies what happened at that point in time.                                                        | None         |
| 10  | state       | Position markers at correct years along timeline     | major  | Accurate positioning shows when each event occurred chronologically.                                             | None         |
| 11  | content     | Display dropdown labeled "Jump to Year"              | major  | The dropdown and label give users the control to highlight specific events.                                      | None         |
| 12  | interaction | Pulse marker animation when year is selected from dropdown | major  | Selecting a year makes the corresponding marker pulse to draw attention.                                         | C11          |
| 13  | layout      | Position timeline horizontally across screen         | minor  | Horizontal layout creates the left-to-right chronological flow.                                                  | None         |
| 14  | layout      | Position event labels above markers                  | minor  | Placing labels above keeps them clearly associated with their markers.                                           | None         |
| 15  | layout      | Position dropdown below timeline                     | minor  | Putting the dropdown below separates navigation from the event display.                                          | None         |

## Justification

The historical event timeline works exactly as expected with interactive event highlighting. A horizontal line displays across the screen representing years from 2020 to 2025. Four circular event markers appear positioned at their correct years along the timeline: "Launch" at 2020, "Expansion" at 2021, "Milestone" at 2023, and "Today" at 2025, each with its label displayed above. Below the timeline, a dropdown menu labeled "Jump to Year" contains options for 2020, 2021, 2023, and 2025. When users select a year from the dropdown, the corresponding event marker on the timeline pulses with an animation to highlight that specific event.
