Category: Data Visualization

Prompt style: Conversational

Title: Area Chart for Sales Data

Prompt: Build an area chart showing monthly sales over 6 months. Display filled area below the line connecting data points in blue color at 50% opacity. Show month labels (Jan, Feb, Mar, Apr, May, Jun) on X-axis at the bottom and sales scale (0 to 1000) on Y-axis on the left side. As I hover over the area, track the hovered position and show tooltip displaying month and sales amount for that point. Include chart title "Monthly Sales" centered at top.

Required libraries: react, tailwindcss, recharts

## Rubric

| #   | ID          | Description                                                                                     | Weight | Rationale                                                                               | Dependent On |
| --- | ----------- | ----------------------------------------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display filled area below the line connecting data points                                       | major  | The filled area gives the chart its characteristic shape and helps visualize the sales trend flowing across time. | None         |
| 2   | visual      | Fill area with blue color at 50% opacity                                                        | major  | Using semi-transparent blue means the area stands out but doesn't completely hide grid lines underneath that help with reading values. | C1           |
| 3   | content     | Display area connecting 6 monthly data points                                                   | major  | Six points capture the sales numbers for each month across the half-year timeframe.     | None         |
| 4   | content     | Display month labels: Jan, Feb, Mar, Apr, May, Jun on X-axis                                    | major  | Showing the actual month names helps people quickly see which month each data point belongs to. | None         |
| 5   | layout      | Position X-axis with month labels at bottom                                                     | minor  | Putting the timeline along the bottom is how most time-based charts are laid out.       | None         |
| 6   | content     | Display sales scale from 0 to 1000 on Y-axis                                                    | major  | The 0 to 1000 range gives users a way to figure out the actual dollar amounts from looking at the chart height. | None         |
| 7   | layout      | Position Y-axis with sales scale on left side                                                   | minor  | Placing values on the left is standard for charts since we read from left to right.     | None         |
| 8   | content     | Display chart title "Monthly Sales"                                                             | major  | The title tells viewers right away that they're looking at monthly sales information.   | None         |
| 9   | layout      | Position chart title centered at top                                                            | minor  | Centering the title at the top looks balanced and professional as a header.             | None         |
| 10  | state       | Track hovered position on the area chart                                                         | major  | Keeping track of where the cursor is hovering lets us know which data point to show details for. | None         |
| 11  | interaction | Show tooltip with month and sales amount on hover                                                | major  | When you hover, the tooltip pops up with exact numbers so you don't have to guess from the chart. | C3           |

## Justification

The area chart displays monthly sales data over 6 months with a filled area below the line connecting data points. The area is filled with blue color at 50% opacity. Month labels (Jan, Feb, Mar, Apr, May, Jun) display on the X-axis at the bottom and sales scale (0 to 1000) displays on the Y-axis on the left side. The chart title "Monthly Sales" appears centered at the top. As users hover over the area, the hovered position is tracked and a tooltip appears showing the month and sales amount for that specific data point.
