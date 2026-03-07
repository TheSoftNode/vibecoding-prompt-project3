Category: Data Visualization

Prompt style: Conversational

Title: Interactive Pie Chart

Prompt: Need a pie chart showing budget breakdown across 4 categories: Marketing, Operations, Development, and Sales. Each slice should have a different color and show the category name and percentage. When I hover over a slice, show a tooltip with the category name and exact dollar amount.

Required libraries: react, tailwindcss, recharts

## Rubric

| #   | ID          | Description                                                        | Weight | Rationale                                                                                       | Dependent On |
| --- | ----------- | ------------------------------------------------------------------ | ------ | ----------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Render a pie chart with 4 slices representing categories           | major  | The chart displays the budget data visually to show how spending is divided up.                 | None         |
| 2   | state       | Apply a different color to each of the 4 slices                    | major  | Different colors make categories easier to tell apart at a glance without reading every label.  | C1           |
| 3   | content     | Display category name on each slice                                | major  | Category names identify what each slice represents.                                             | C1           |
| 4   | content     | Display percentage value on each slice                             | major  | Percentages show how much of the total budget each category takes up.                           | C1           |
| 5   | layout      | Position the category name and percentage inside each slice        | minor  | Placing labels inside slices keeps the information directly connected to what it describes.     | C3           |
| 6   | interaction | Display a tooltip when user hovers over a slice                    | major  | The tooltip provides additional details on demand without cluttering the chart.                 | C1           |
| 7   | content     | Display category name in the tooltip                               | major  | Showing the category name in the tooltip confirms which slice is being hovered.                 | C6           |
| 8   | content     | Display exact dollar amount in the tooltip                         | major  | The dollar amount gives the precise budget value for the category.                              | C6           |

## Justification

The pie chart works exactly as expected with 4 slices showing the budget breakdown for Marketing, Operations, Development, and Sales. Each slice displays in a different color to tell the categories apart. The category name and percentage appear inside each slice showing what it represents and how much of the budget it takes up. When hovering over a slice, a tooltip appears displaying the category name and exact dollar amount for that category.
