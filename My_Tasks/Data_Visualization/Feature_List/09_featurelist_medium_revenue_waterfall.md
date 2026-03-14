Category: Data_Visualization

Prompt style: Feature List

Title: Revenue Waterfall Chart

Prompt: Build a revenue waterfall chart visualizing monthly financial changes with an opening balance and several positive and negative changes leading to an ending balance. Display each change as a vertical bar positioned to show the running balance - bars for increases extend upward from the previous balance, bars for decreases extend downward. Color positive changes green, negative red, opening/ending blue. Draw connector lines between bars. Display amounts inside bars. Show net change as a summary label below, color-coded green or red. Display largest increase and decrease. Preload with sample monthly revenue data.

Required libraries: react, tailwindcss, lucide-react, recharts

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                 | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display opening balance bar starting at zero reaching $100K     | major  | The opening balance bar establishes the baseline for all subsequent financial changes.                    | None         |
| 2   | visual      | Display six change bars for Feb-Mar-Apr-May-Jun                  | major  | Six change bars visualize each month's financial impact on the running balance.                           | None         |
| 3   | visual      | Display ending balance bar from zero to final amount             | major  | The ending balance bar shows the cumulative result of all changes.                                        | None         |
| 4   | layout      | Position positive change bars floating at previous month's ending value | major  | Floating bars visually demonstrate how each change builds upon the previous balance.                      | C1, C2       |
| 5   | layout      | Position negative change bars floating at previous month's ending value | major  | Floating negative bars show declines from the current balance level.                                      | C1, C2       |
| 6   | visual      | Draw thin gray connector lines between consecutive bars          | minor  | Connector lines guide the eye through the flow from one month to the next.                                | C4, C5       |
| 7   | visual      | Color positive change bars green                                 | major  | Green coloring immediately identifies months with revenue growth.                                         | None         |
| 8   | visual      | Color negative change bars red                                   | major  | Red coloring draws attention to months with financial losses.                                             | None         |
| 9   | visual      | Color opening and ending balance bars blue                       | minor  | Blue distinguishes balance bars from change bars, clarifying the chart structure.                         | None         |
| 10  | content     | Display dollar amount centered inside each bar                   | major  | Centered amounts provide exact values that complement the visual bar heights.                             | None         |
| 11  | state       | Calculate net change as ending balance minus opening balance     | major  | Net change gives users the bottom-line financial impact over the entire period.                           | None         |
| 12  | content     | Display net change as "Net Change: +$X" or "Net Change: -$X"     | major  | The formatted label clearly communicates the overall financial direction.                                 | C11          |
| 13  | visual      | Color net change label green if positive, red if negative        | minor  | Color coding provides instant visual feedback about overall financial health.                             | C11          |
| 14  | state       | Identify largest single increase with month name                 | major  | Highlighting the largest increase reveals the most impactful positive month.                              | None         |
| 15  | state       | Identify largest single decrease with month name                 | major  | Highlighting the largest decrease identifies the month requiring the most attention.                      | None         |
| 16  | content     | Display largest increase and decrease in summary                 | major  | Showing extremes helps users quickly identify key financial events.                                       | C14, C15     |

## Justification

The Revenue Waterfall Chart achieved 56% pass rate (9/16 criteria) with failures in bar positioning and extreme value identification. The chart correctly displays an opening balance bar from zero to $100K (C1 passed), six monthly change bars (C2 passed), and an ending balance bar from zero to the final amount (C3 passed). However, the floating bar positioning completely failed C4 and C5 - instead of floating at the previous month's ending value, all bars started at zero like a standard bar chart. February's +$25K bar should have floated from $100K to $125K, but instead started at zero and reached $25K, destroying the waterfall flow visualization. Without correct floating, the connector lines (C6) were also meaningless, though the model did draw gray lines between bar tops. The color coding worked perfectly: positive changes appeared green (C7 passed), negative changes red (C8 passed), and opening/ending balances blue (C9 passed). Dollar amounts displayed centered inside each bar (C10 passed). The net change calculation worked correctly (C11 passed), showing "Net Change: +$60K" with proper formatting (C12 passed) and green coloring (C13 passed) since the ending balance ($160K) minus opening ($100K) equals +$60K. However, the extreme value identification failed C14 and C15 - the summary showed "Largest Increase: February +$25K" and "Largest Decrease: March -$15K" when April's +$40K was actually the largest increase, indicating the model compared absolute values without accounting for the sign. The display of extremes failed C16 as well, showing incorrect months. The fundamental floating bar positioning failure (C4, C5) meant this looked like a colored bar chart rather than a true waterfall diagram where users can trace the cumulative financial flow from January through June.
