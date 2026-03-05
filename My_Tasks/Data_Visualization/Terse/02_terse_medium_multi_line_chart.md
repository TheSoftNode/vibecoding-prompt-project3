Category: Data Visualization

Prompt style: Terse

Title: Multi-Line Comparison Chart

Prompt: Line chart comparing three products' sales over 12 months. Three lines in different colors (blue, green, orange). Each line has data point markers. Toggle buttons show/hide individual lines. Y-axis shows sales in thousands. X-axis shows months. Hover tooltip shows month, product, exact value. Legend shows products with colors. Grid lines on both axes. Line for Product A starts at 10k Jan, peaks 45k July. Product B steady 20-30k. Product C grows 5k to 40k. Chart title and axis labels included.

Required libraries: react, tailwindcss, recharts, lucide-react

## Rubric

| ID | Description | Weight | Rationale | Dependent On |
|----|-------------|--------|-----------|--------------|
| content-1 | Display three lines for three products | major | Multiple lines enable comparison | None |
| visual-1 | Apply blue, green, orange colors to lines | major | Colors differentiate products | content-1 |
| visual-2 | Mark data points on each line | major | Markers highlight data locations | content-1 |
| content-2 | Display 12 months on X-axis | major | Time labels provide context | None |
| content-3 | Display sales scale (thousands) on Y-axis | major | Scale enables value reading | None |
| visual-3 | Display grid lines on both axes | major | Grids aid reading | content-2 |
| interaction-1 | Show tooltip on point hover with month, product, value | major | Tooltip provides details | visual-2 |
| layout-1 | Display legend with product names and colors | major | Legend maps colors to products | None |
| visual-4 | Display toggle buttons for each product | major | Toggles enable selective viewing | None |
| interaction-2 | Show/hide line when toggle clicked | major | Toggle controls visibility | visual-4 |
| state-1 | Pre-load Product A data: Jan 10k, peaks July 45k | major | Sample data provides initial render | None |
| state-2 | Pre-load Product B data: steady 20-30k | major | Consistent data shows flat trend | None |
| state-3 | Pre-load Product C data: grows 5k to 40k | major | Growing data shows upward trend | None |
| content-4 | Display chart title | major | Title identifies content | None |
| content-5 | Display axis labels | major | Labels describe axes | content-2 |
