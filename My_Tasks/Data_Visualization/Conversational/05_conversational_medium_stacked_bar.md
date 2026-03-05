Category: Data Visualization

Prompt style: Conversational

Title: Stacked Bar Chart with Filters

Prompt: I need a stacked bar chart showing quarterly revenue breakdown by region (North, South, East, West). Each bar represents a quarter (Q1-Q4), stacked with four colored segments for regions. Include filter dropdown to view specific region only or all regions. Display total revenue number on top of each bar. Hover shows region name and amount. Legend maps colors to regions. Y-axis shows revenue scale. Add percentage labels on each stack segment showing its portion of quarterly total. Include chart title.

Required libraries: react, tailwindcss, recharts, lucide-react

## Rubric

| ID | Description | Weight | Rationale | Dependent On |
|----|-------------|--------|-----------|--------------|
| content-1 | Display 4 bars for Q1-Q4 | major | Bars represent time periods | None |
| visual-1 | Stack each bar with 4 colored segments for regions | major | Stacking shows composition | content-1 |
| content-2 | Display total revenue number on top of each bar | major | Total shows aggregate value | content-1 |
| visual-2 | Display percentage label on each stack segment | major | Percentages show proportions | visual-1 |
| state-1 | Calculate percentage as (region value / quarter total) × 100 | major | Percentage is derived proportion | visual-2 |
| interaction-1 | Show tooltip on segment hover with region and amount | major | Tooltip provides details | visual-1 |
| layout-1 | Display legend mapping colors to regions | major | Legend enables identification | None |
| visual-3 | Display filter dropdown with region options plus "All" | major | Filter enables focus | None |
| interaction-2 | Show only selected region when filter applied | major | Filtering isolates data | visual-3 |
| state-2 | Show all regions when "All" is selected | major | All option restores full view | interaction-2 |
| content-3 | Display Y-axis with revenue scale | major | Scale enables value reading | None |
| content-4 | Display chart title | major | Title identifies content | None |
