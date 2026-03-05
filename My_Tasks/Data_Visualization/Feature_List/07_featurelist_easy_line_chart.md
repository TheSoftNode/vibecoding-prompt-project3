Category: Data Visualization

Prompt style: Feature List

Title: Line Chart with Data Points

Prompt: Build a line chart showing temperature over 7 days. Plot points for each day connected by lines. Display day labels on X-axis and temperature scale on Y-axis. Mark each data point with a circle. Show tooltip on point hover with day and temperature. Include chart title and axis labels. Use red line color.

Required libraries: react, tailwindcss, recharts

## Rubric

| ID | Description | Weight | Rationale | Dependent On |
|----|-------------|--------|-----------|--------------|
| content-1 | Display line connecting 7 data points | major | Line shows trend over time | None |
| visual-1 | Apply red color to line | major | Red provides visual identity | content-1 |
| visual-2 | Mark each point with circle | major | Circles highlight data locations | content-1 |
| content-2 | Display day labels on X-axis | major | Labels identify time periods | None |
| content-3 | Display temperature scale on Y-axis | major | Scale enables value reading | None |
| interaction-1 | Show tooltip with day and temp on point hover | major | Tooltip provides exact data | visual-2 |
| content-4 | Display chart title | major | Title identifies content | None |
| content-5 | Display axis labels | major | Labels describe axes | content-2 |
