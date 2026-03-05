Category: Data Visualization

Prompt style: Casual

Title: Donut Chart with Center Text

Prompt: Donut chart showing time spent on activities. Five slices for Work, Sleep, Exercise, Leisure, Other. Different color each. Show percentage on slices. Center displays total hours (24). Hover shows activity and exact hours. Legend below.

Required libraries: react, tailwindcss, recharts, lucide-react

## Rubric

| ID | Description | Weight | Rationale | Dependent On |
|----|-------------|--------|-----------|--------------|
| content-1 | Display donut chart with 5 slices | major | Donut visualizes proportions | None |
| visual-1 | Apply different color to each slice | major | Colors differentiate categories | content-1 |
| content-2 | Display percentage on each slice | major | Percentages show proportions | content-1 |
| content-3 | Display total hours (24) in center | major | Center text shows sum | None |
| interaction-1 | Show tooltip with activity and hours on hover | major | Tooltip provides details | content-1 |
| layout-1 | Display legend below chart | major | Legend maps colors to activities | None |
| content-4 | List all activities in legend with colors | major | Legend enables identification | layout-1 |
