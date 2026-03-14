Category: Data_Visualization

Prompt style: Conversational

Title: Quarterly Sales Performance Multi-Ring Chart

Prompt: I need to visualize quarterly sales performance for three products using concentric rings - inner ring for Q1, middle for Q2, outer for Q3. Each ring divides into segments where each product's arc size shows its share of that quarter's sales. The three products should align across all rings. Color segments green if sales went up from the previous quarter, red if down, and gray for Q1. Below the chart, show a performance summary with each product's Q1-to-Q3 growth and which had the most steady performance. Preload with sample quarterly sales data.

Required libraries: react, tailwindcss, lucide-react, recharts

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                 | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display three concentric rings (inner Q1, middle Q2, outer Q3)   | major  | The three rings establish the quarterly timeline structure for comparing performance over time.           | None         |
| 2   | content     | Label rings as Q1, Q2, Q3                                        | minor  | Labels help users identify which quarter each ring represents.                                            | None         |
| 3   | state       | Calculate arc angles based on product's percentage of quarter total | major  | Percentage-based angles allow visual comparison of market share within each quarter.                      | None         |
| 4   | visual      | Divide each ring into three segments for products A, B, C        | major  | Three segments per ring show each product's market share in that quarter.                                 | None         |
| 5   | layout      | Align product segments across rings at same starting angle       | major  | Alignment enables users to trace one product's performance across quarters easily.                        | C4           |
| 6   | state       | Compare each product's sales to previous quarter                 | major  | Quarter-over-quarter comparison determines the color coding that highlights trends.                       | None         |
| 7   | visual      | Color Q1 segments gray (no prior quarter)                        | major  | Gray Q1 segments indicate there's no baseline for comparison yet.                                         | None         |
| 8   | visual      | Color segments green if sales increased from previous quarter    | major  | Green coloring immediately highlights positive growth trends for quick identification.                    | C6           |
| 9   | visual      | Color segments red if sales decreased from previous quarter      | major  | Red coloring draws attention to declining performance that may need intervention.                         | C6           |
| 10  | content     | Display performance summary below chart                          | minor  | The summary panel provides detailed metrics without cluttering the visual representation.                 | None         |
| 11  | state       | Calculate growth rate as percentage change from Q1 to Q3         | major  | Q1-to-Q3 growth shows overall quarterly progression for each product line.                                | None         |
| 12  | content     | Show growth rate for each product in summary                     | major  | Displaying growth rates gives users precise performance metrics for decision-making.                      | C11          |
| 13  | state       | Calculate variance in quarterly sales for each product           | major  | Variance measurement identifies which products have stable vs volatile sales patterns.                    | None         |
| 14  | state       | Identify product with smallest variance as most consistent       | major  | The smallest variance indicates the most predictable and stable product performance.                      | C13          |
| 15  | content     | Display most consistent product in summary                       | major  | Highlighting consistency helps users identify reliable revenue sources.                                   | C14          |
| 16  | state       | Apply tie-breaker using higher Q3 sales when variances equal     | minor  | Tie-breaking ensures a definitive result even when multiple products have identical variance.             | C14          |

## Justification

The Quarterly Sales Performance Multi-Ring Chart achieved 56% pass rate (9/16 criteria) with failures in calculations and alignment. The visualization correctly displays three concentric rings labeled Q1, Q2, Q3 from inner to outer (C1, C2 passed) with each ring divided into three segments for Products A, B, and C (C4 passed). However, the arc angle calculation failed C3 - instead of sizing segments proportionally to each product's percentage of that quarter's total, all segments appeared equal at 120 degrees (one third of the circle) regardless of actual sales values. This meant Product A's Q1 segment (which should be 33% or 120°) appeared the same size as Product C's Q1 segment (which should be 42% or 150°). The alignment failed C5 catastrophically - Product A started at 0° in Q1, 45° in Q2, and 90° in Q3, making it impossible to trace a product's performance across quarters visually. The coloring logic worked partially: Q1 segments were correctly gray (C7 passed), but the increase/decrease detection failed C8 and C9 - Product A decreased from Q2 ($55K) to Q3 ($48K) but showed green instead of red, indicating the model compared to Q1 instead of the previous quarter. The performance summary appeared below the chart (C10 passed) and correctly calculated Q1-to-Q3 growth rates (C11, C12 passed): Product A +20%, Product B +40%, Product C +20%. However, the variance calculation failed C13 - the summary showed "Product B - Most Consistent" when Product A actually had the smallest variance ($10.4K vs Product B's $12.2K variance). The tie-breaker logic was untested since no tie occurred, but the fundamental variance calculation error suggests C14, C15, and C16 implementation would also be problematic.
