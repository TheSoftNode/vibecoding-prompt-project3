Category: Data Visualization

Prompt style: Conversational

Title: Interactive Pie Chart

Prompt: I need a pie chart showing budget breakdown across 4 categories. Each slice should have a different color and show the category name and percentage. When I hover over a slice, make it slightly bigger and show a tooltip with the exact amount. Include a legend on the right listing all categories with their colors.

Required libraries: react, tailwindcss, recharts, lucide-react

## Rubric

| ID | Description | Weight | Rationale | Dependent On |
|----|-------------|--------|-----------|--------------|
| content-1 | Display pie chart with 4 slices representing categories | major | Slices are core chart visualization | None |
| visual-1 | Apply different color to each slice | major | Color differentiation enables category distinction | content-1 |
| content-2 | Display category name on each slice | major | Labels identify slice content | content-1 |
| content-3 | Display percentage on each slice | major | Percentages quantify proportions | content-1 |
| state-1 | Calculate percentage as (category value / total) × 100 | major | Percentage is derived proportion | content-3 |
| interaction-1 | Enlarge slice on hover | major | Visual feedback confirms hover target | content-1 |
| interaction-2 | Show tooltip with exact amount on hover | major | Tooltip provides precise value | interaction-1 |
| layout-1 | Display legend on right side | major | Legend maps colors to categories | None |
| content-4 | List all categories in legend with matching colors | major | Legend entries enable identification | layout-1 |
