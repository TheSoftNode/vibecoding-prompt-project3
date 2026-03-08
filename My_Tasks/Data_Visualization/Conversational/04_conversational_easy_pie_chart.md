Category: Data Visualization

Prompt style: Conversational

Title: Interactive Pie Chart

Prompt: Need a pie chart showing budget breakdown across 4 categories with these amounts: Marketing $5000, Operations $3000, Development $4000, and Sales $2000. Each slice should have a different color: Marketing in blue, Operations in green, Development in orange, and Sales in purple. Show the percentage on each slice. Display the total budget amount below the chart. When I hover over a slice, show a tooltip with the category name and exact dollar amount.

Required libraries: react, tailwindcss, recharts

## Rubric

| #   | ID          | Description                                                        | Weight | Rationale                                                                                       | Dependent On |
| --- | ----------- | ------------------------------------------------------------------ | ------ | ----------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Render a pie chart with 4 slices representing categories           | major  | The chart displays the budget data visually to show how spending is divided up.                 | None         |
| 2   | content     | Display budget amounts: Marketing $5000, Operations $3000, Development $4000, and Sales $2000 | major  | These specific amounts provide the actual budget values for each category.        | C1           |
| 3   | visual      | Display Marketing slice in blue, Operations slice in green, Development in orange, and Sales slice in purple | major  | Different colors for each category make them easier to tell apart at a glance.     | C1           |
| 4   | content     | Display percentage value on each slice                             | major  | Percentages show how much of the total budget each category takes up.                           | C1           |
| 5   | layout      | Position the percentage on each slice                              | minor  | Placing percentages on slices keeps the information directly connected to what it describes.    | C4           |
| 6   | state       | Calculate and display total budget amount as $14000                | major  | The total is computed automatically from the category amounts without user input.               | C2           |
| 7   | layout      | Position the total budget amount below the chart                   | minor  | Placing the total below the chart separates summary information from the visualization.         | C6           |
| 8   | interaction | Show a tooltip when user hovers over a slice                       | major  | Hovering reveals additional details on demand without cluttering the chart.                     | C1           |
| 9   | content     | Display the category names Marketing, Operations, Development, and Sales in the tooltip | major  | These specific category names identify which slice is being hovered.                  | C8           |
| 10  | content     | Display exact dollar amount in the tooltip                         | major  | The dollar amount gives the precise budget value for the category.                              | C8           |

## Justification

The pie chart works exactly as expected with 4 slices showing the budget breakdown for Marketing, Operations, Development, and Sales. Marketing displays in blue, Operations in green, Development in orange, and Sales in purple. The percentage appears on each slice showing how much of the budget it takes up. The total budget amount of $14000 displays below the chart. When hovering over a slice, a tooltip appears displaying the category name and exact dollar amount for that category.
