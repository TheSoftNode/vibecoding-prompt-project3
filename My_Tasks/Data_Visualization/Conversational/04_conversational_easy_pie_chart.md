Category: Data Visualization

Prompt style: Conversational

Title: Interactive Pie Chart

Prompt: Need a pie chart showing budget breakdown across 4 categories. Each slice should have a different color and display the category name and percentage. When I hover over a slice, it should enlarge slightly and show a tooltip with the exact dollar amount. Include a legend on the right side listing all categories with their corresponding colors.

Required libraries: react, tailwindcss, recharts

## Rubric

| #   | ID          | Description                                                       | Weight | Rationale                                                                                                                       | Dependent On |
| --- | ----------- | ----------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Render a pie chart with 4 slices representing categories         | major  | The pie chart is the core visualization element that displays the budget breakdown across the four categories.                  | None         |
| 2   | state       | Apply a different color to each of the 4 slices                  | major  | Color differentiation provides instant visual distinction between categories, allowing users to quickly identify different budget areas without reading labels. | C1           |
| 3   | content     | Display category name on each slice                              | major  | Category names provide essential identification so users know what budget area each slice represents.                           | C1           |
| 4   | content     | Display percentage value on each slice                           | major  | Percentage values quantify the proportional share of each category, enabling users to understand relative budget distribution.  | C1           |
| 5   | interaction | Enlarge slice when user hovers over it                           | major  | Visual enlargement provides immediate feedback confirming which slice the user is interacting with.                             | C1           |
| 6   | interaction | Show tooltip with exact dollar amount when user hovers over slice| major  | The tooltip reveals precise numerical values that complement the visual proportions shown in the chart.                         | C5           |
| 7   | visual      | Display a legend for the chart                                   | major  | The legend serves as a reference key that maps each color to its corresponding category name.                                   | None         |
| 8   | layout      | Position the legend on the right side of the chart               | minor  | Placing the legend to the right maintains a conventional chart layout that separates the visualization from the reference key.  | C7           |
| 9   | content     | List all 4 category names in the legend                          | major  | Listing all category names ensures users can identify every budget area shown in the chart.                                     | C7           |
| 10  | state       | Display colors in legend that match the corresponding slice colors| major  | Matching colors between legend and slices creates visual consistency that helps users connect the reference key to the chart data.| C9           |
