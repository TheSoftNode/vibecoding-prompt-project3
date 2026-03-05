Category: Data Visualization

Prompt style: Terse

Title: Simple Bar Chart

Prompt: Bar chart with 5 data points. Each bar shows label and value. Hover shows tooltip with exact value. Color bars blue. Y-axis shows scale with grid lines. X-axis shows labels. Title at top.

Required libraries: react, tailwindcss, recharts

## Rubric

| ID | Description | Weight | Rationale | Dependent On |
|----|-------------|--------|-----------|--------------|
| content-1 | Display 5 bars representing data points | major | Bars are core chart visualization | None |
| visual-1 | Apply blue color to all bars | major | Blue provides consistent visual identity | content-1 |
| content-2 | Display label for each bar on X-axis | major | Labels identify data categories | content-1 |
| content-3 | Display value scale on Y-axis | major | Scale enables value reading | None |
| visual-2 | Display grid lines aligned with Y-axis scale | major | Grid lines aid value estimation | content-3 |
| interaction-1 | Show tooltip with exact value on bar hover | major | Tooltip provides precise data | content-1 |
| content-4 | Display chart title at top | major | Title identifies chart content | None |
| state-1 | Calculate Y-axis scale based on data range | major | Auto-scaling ensures all data fits | content-3 |
| visual-3 | Set bar height proportional to value | major | Height encoding represents quantitative data | content-1 |
