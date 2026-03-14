Category: Data_Visualization

Prompt style: Conversational

Title: Regional Sales Heatmap Grid

Prompt: I need a heatmap showing regional sales performance over time as a grid with regions as rows and months as columns. Color each cell based on how it compares to that region's average - green for above, red for below, yellow for close. Add three filter buttons to show all months, last 6, or last 3 - when filtering, recalculate each region's average from only visible months so colors always reflect performance against the current period's baseline. Show which region performs best and worst. Preload with sample regional sales data.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                 | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display grid with 6 rows for regions                             | major  | The six rows establish the regional structure for comparing performance across locations.                 | None         |
| 2   | visual      | Display 12 columns for months Jan-Dec initially                  | major  | Twelve columns provide the complete annual timeline for analyzing seasonal patterns.                      | None         |
| 3   | content     | Label rows as North, South, East, West, Central, Coastal         | minor  | Row labels help users identify which region each row represents.                                          | None         |
| 4   | content     | Label columns as Jan, Feb, Mar, Apr, May, Jun, Jul, Aug, Sep, Oct, Nov, Dec | minor  | Month labels help users identify the time period for each column.                                         | None         |
| 5   | content     | Display sales dollar amount as text inside each cell             | major  | Dollar amounts provide exact values that complement the color-coded visual comparison.                    | None         |
| 6   | state       | Calculate each region's average from its 12 monthly values       | major  | Per-region averages enable comparison of each month to that region's typical performance.                 | None         |
| 7   | visual      | Color cells green when above region's average                    | major  | Green coloring highlights above-average performance months for each region.                               | C6           |
| 8   | visual      | Color cells red when below region's average                      | major  | Red coloring draws attention to below-average performance that may need investigation.                    | C6           |
| 9   | visual      | Color cells yellow when within 5% of region's average            | major  | Yellow indicates near-average performance, providing a neutral middle category.                           | C6           |
| 10  | visual      | Use darker green shades for higher above-average amounts         | minor  | Shade intensity helps users distinguish slightly above-average from significantly above-average.          | C7           |
| 11  | visual      | Use darker red shades for lower below-average amounts            | minor  | Shade intensity shows severity of below-average performance at a glance.                                  | C8           |
| 12  | interaction | Display three filter buttons: All Months, Last 6 Months, Last 3 Months | minor  | Filter buttons let users focus on recent performance vs full annual trends.                               | None         |
| 13  | interaction | Redraw grid with only filtered months as columns when filter selected | major  | Redrawing with fewer columns focuses the view on the selected time period.                                | C12          |
| 14  | state       | Recalculate each region's average using only visible months      | major  | Recalculating averages from filtered data ensures colors reflect performance within the filtered period.  | C6, C13      |
| 15  | state       | Identify highest performing region by most months above its average | major  | Counting above-average months reveals which region most consistently exceeds expectations.                | C6, C14      |
| 16  | state       | Apply tie-breaker using first region in row order                | minor  | Tie-breaking ensures a definitive result when multiple regions have identical above-average month counts. | C15          |

## Justification

The Regional Sales Heatmap Grid achieved 50% pass rate (8/16 criteria) with failures concentrated in dynamic recalculation and color logic. The visualization correctly displays a 6×12 grid (C1, C2 passed) with rows labeled North, South, East, West, Central, Coastal (C3 passed) and columns labeled Jan through Dec (C4 passed). Each cell displays the sales dollar amount as text (C5 passed). The initial average calculation worked correctly, computing each region's average from its 12 monthly values (C6 passed). However, the color coding failed C7, C8, and C9 - instead of using the region's own average as the baseline, the model calculated a single global average across all regions and colored all cells relative to that global value. This meant North's March ($45K, above North's $42K average) appeared red because it fell below the global average of $48K. The shade intensity feature completely failed C10 and C11, with all green cells using the same shade and all red cells using the same shade regardless of how far above or below average they were. The three filter buttons displayed correctly (C12 passed), but the grid redraw failed C13 - selecting "Last 3 Months" kept all 12 columns visible and simply grayed out the first 9 columns instead of removing them and showing only Oct-Nov-Dec. The critical failure was C14: when filters changed, the model continued using the original 12-month average for color calculations instead of recalculating each region's average from only the visible months, making the filtered view's colors meaningless. The summary stats appeared below the grid but failed C15 - it identified "North - Highest Performing" when East actually had more months above its own average (7 months vs North's 6 months). The tie-breaker logic (C16) was untested since the fundamental counting error in C15 meant no tie occurred in the test case.
