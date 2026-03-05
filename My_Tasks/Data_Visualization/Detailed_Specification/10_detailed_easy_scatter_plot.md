Category: Data Visualization

Prompt style: Detailed Specification

Title: Scatter Plot with Correlation

Prompt: Create a scatter plot showing the relationship between study hours and test scores for 10 students. Each point represents one student. Display study hours on X-axis (0-10 range) and test scores on Y-axis (0-100 range). Color points based on score: green for 80+, yellow for 60-79, red for below 60. Show tooltip on hover with student number, hours, and score. Include a trend line showing correlation. Add title and axis labels.

Required libraries: react, tailwindcss, recharts

## Rubric

| ID | Description | Weight | Rationale | Dependent On |
|----|-------------|--------|-----------|--------------|
| content-1 | Display 10 points representing students | major | Points are core scatter plot elements | None |
| content-2 | Position points by study hours (X) and score (Y) | major | XY positioning encodes data relationship | content-1 |
| content-3 | Display X-axis with 0-10 range for study hours | major | X-axis defines hours scale | None |
| content-4 | Display Y-axis with 0-100 range for scores | major | Y-axis defines score scale | None |
| visual-1 | Color points green when score ≥ 80 | major | Green indicates high performance | content-2 |
| visual-2 | Color points yellow when 60 ≤ score < 80 | major | Yellow indicates medium performance | content-2 |
| visual-3 | Color points red when score < 60 | major | Red indicates low performance | content-2 |
| interaction-1 | Show tooltip on point hover | major | Tooltip provides detailed data | content-1 |
| content-5 | Display student number, hours, score in tooltip | major | Complete info enables analysis | interaction-1 |
| visual-4 | Display trend line through points | major | Trend line shows correlation | content-2 |
| content-6 | Display chart title | major | Title identifies content | None |
| content-7 | Display axis labels | major | Labels describe axes | content-3 |
