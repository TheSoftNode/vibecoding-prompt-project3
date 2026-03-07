Category: Data Visualization

Prompt style: Conversational

Title: Interactive Pie Chart

Prompt: Need a pie chart showing budget breakdown across 4 categories. Each slice should have a different color and show the category name and percentage. When I hover over a slice, show a tooltip with the exact dollar amount. Include a legend on the right side listing all categories with their colors.

Required libraries: react, tailwindcss, recharts

## Rubric

| #   | ID          | Description                                                       | Weight | Rationale                                                                                                                       | Dependent On |
| --- | ----------- | ----------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Render a pie chart with 4 slices representing categories         | major  | The chart displays the budget data visually so you can see how spending is divided up.                  | None         |
| 2   | state       | Apply a different color to each of the 4 slices                  | major  | Different colors let you tell the categories apart at a glance without needing to read every label. | C1           |
| 3   | content     | Display category name on each slice                              | major  | You need to know what each slice actually represents.                           | C1           |
| 4   | content     | Display percentage value on each slice                           | major  | Percentages show how much of the total budget each category takes up.  | C1           |
| 5   | interaction | Show tooltip with exact dollar amount when user hovers over slice| major  | Hovering gives you the actual dollar value, which is more useful than just seeing the slice size.                         | C1           |
| 6   | visual      | Display a legend for the chart                                   | major  | The legend shows which color goes with which category.                                   | None         |
| 7   | layout      | Position the legend on the right side of the chart               | minor  | Putting the legend on the right keeps it out of the way but still easy to check.  | C6           |
| 8   | content     | List all 4 category names in the legend                          | major  | All categories need to appear in the legend so nothing gets left out.                                     | C6           |
| 9   | state       | Display colors in legend that match the corresponding slice colors| major  | Legend colors have to match the slices or you won't know which is which.| C8           |
