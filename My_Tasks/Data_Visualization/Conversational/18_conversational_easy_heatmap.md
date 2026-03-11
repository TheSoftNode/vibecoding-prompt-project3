Category: Data_Visualization

Prompt style: Conversational

Title: Weekly Activity Heatmap

Prompt: I need a weekly activity heatmap showing productivity hours. Create a 7x24 grid representing days of the week (rows) and hours of the day (columns). Label rows "Mon" through "Sun" on the left. Label columns "12am", "6am", "12pm", "6pm" at the top. Fill each cell with a color intensity from white (0 hours) to dark green (4+ hours) based on random activity data. When I hover over a cell, show the exact hour count for that day and time.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                  | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ------------------------------------------------------------ | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 7x24 grid of cells                                   | major  | The 7x24 grid structure is the foundation showing all day-hour combinations for the week.                        | None         |
| 2   | content     | Display day labels "Mon" through "Sun" for rows              | major  | Day labels let users identify which row corresponds to each weekday.                                             | None         |
| 3   | layout      | Position day labels on the left side of grid                 | minor  | Left positioning of day labels creates the standard row header layout for reading the heatmap.                   | None         |
| 4   | content     | Display hour labels "12am", "6am", "12pm", "6pm" for columns | major  | Hour labels help users identify the time periods represented by each column.                                     | None         |
| 5   | layout      | Position hour labels at the top of grid                      | minor  | Top positioning of hour labels creates the standard column header layout for reading the heatmap.                | None         |
| 6   | state       | Generate random activity data for each cell                  | major  | Random data populates the heatmap so it has meaningful values to display.                                        | None         |
| 7   | visual      | Fill cells with white color for 0 hours activity             | major  | White cells show time periods with no activity, providing the baseline color.                                    | None         |
| 8   | visual      | Fill cells with dark green color for 4+ hours activity       | major  | Dark green cells show peak activity periods, providing the maximum intensity color.                              | None         |
| 9   | state       | Calculate color intensity based on activity hours            | major  | Color intensity mapping translates numeric hours into visual color gradients for quick pattern recognition.      | None         |
| 10  | visual      | Display gradient from white to dark green across cells       | major  | The gradient creates a visual spectrum showing activity levels at a glance without reading numbers.              | None         |
| 11  | interaction | Display tooltip with exact hour count on hover               | major  | Hover tooltips let users see precise activity values for any day-hour combination.                               | None         |
| 12  | content     | Display day and time information in tooltip                  | minor  | Including day and time context in the tooltip helps users understand exactly which period they're viewing.       | None         |

## Justification

The application achieved a 91.67% pass rate with one specific failure. A 7x24 grid of cells displays representing the full week. Rows are labeled "Mon" through "Sun" and columns are labeled "12am", "6am", "12pm", "6pm". Random activity data is generated for each cell. Cells are filled with colors ranging from white for 0 hours to dark green for 4+ hours, creating a gradient showing activity intensity. When hovering over any cell, a tooltip appears displaying the exact hour count along with the day and time information. However, the model failed to position day labels on the left side of the grid. Instead, day labels appear above the grid in a separate header row or to the right side, not on the left as required for standard heatmap row headers. This positioning issue caused the failure despite all other functionality working correctly.
