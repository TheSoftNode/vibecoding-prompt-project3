Category: Data Visualization

Prompt style: Conversational

Title: Interactive Pie Chart

Prompt: Need a pie chart showing budget breakdown across 4 categories: Marketing, Operations, Development, and Sales. Each slice should have a different color: Marketing in blue, Operations in green, Development in orange, and Sales in purple. Show the category name and percentage below the chart. When I hover over a slice, show a tooltip with the exact dollar amount.

Required libraries: react, tailwindcss, recharts

## Rubric

| #   | ID          | Description                                                        | Weight | Rationale                                                                                       | Dependent On |
| --- | ----------- | ------------------------------------------------------------------ | ------ | ----------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Render a pie chart with 4 slices representing categories           | major  | The chart displays the budget data visually to show how spending is divided up.                 | None         |
| 2   | content     | Display the category names Marketing, Operations, Development, and Sales | major  | These specific category names identify what each slice represents.                         | C1           |
| 3   | content     | Display percentage value for each category                         | major  | Percentages show how much of the total budget each category takes up.                           | C1           |
| 4   | layout      | Position the category names and percentages below the chart        | minor  | Placing the information below the chart keeps it organized and easy to read.                    | C2           |
| 5   | state       | Display Marketing slice in blue, Operations slice in green, Development slice in orange, and Sales slice in purple | major  | Different colors for each category make them easier to tell apart at a glance.     | C2           |
| 6   | interaction | Show a tooltip when user hovers over a slice                       | major  | Hovering reveals additional details on demand without cluttering the chart.                     | C1           |
| 7   | content     | Display exact dollar amount in the tooltip                         | major  | The dollar amount gives the precise budget value for the category.                              | C6           |
| 8   | visual      | Display a tooltip box                                              | major  | The tooltip box provides a container for showing the dollar amount information.                 | None         |

## Justification

The pie chart works exactly as expected with 4 slices showing the budget breakdown for Marketing, Operations, Development, and Sales. Marketing displays in blue, Operations in green, Development in orange, and Sales in purple. The category names and percentages appear below the chart showing what each category represents and how much of the budget it takes up. When hovering over a slice, a tooltip box appears displaying the exact dollar amount for that category.
