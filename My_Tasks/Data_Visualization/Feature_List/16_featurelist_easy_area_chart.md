Category: Data Visualization

Prompt style: Conversational

Title: Area Chart for Sales Data

Prompt: Build an area chart showing monthly sales over 6 months. Display filled area below the line connecting data points in semi-transparent blue. Show month labels (Jan, Feb, Mar, Apr, May, Jun) along the bottom and sales values along the left side. As I hover over the area, track the hovered position and show tooltip displaying month and sales amount for that point. Include chart title "Monthly Sales" at the top.

Required libraries: react, tailwindcss, recharts

## Rubric

| #   | ID          | Description                                                                                     | Weight | Rationale                                                                               | Dependent On |
| --- | ----------- | ----------------------------------------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display filled area below the line connecting data points                                       | major  | The filled area gives the chart its characteristic shape and helps visualize the sales trend flowing across time. | None         |
| 2   | visual      | Fill area with semi-transparent blue color                                                       | major  | Semi-transparent blue makes the area visible while keeping any background elements readable. | C1           |
| 3   | content     | Display area connecting 6 monthly data points                                                   | major  | Six points capture the sales numbers for each month across the half-year timeframe.     | None         |
| 4   | content     | Display month labels: Jan, Feb, Mar, Apr, May, Jun                                              | major  | Showing the actual month names helps people quickly see which month each data point belongs to. | None         |
| 5   | layout      | Position month labels along the bottom                                                          | minor  | Putting the timeline along the bottom is how most time-based charts are laid out.       | None         |
| 6   | content     | Display sales values scale                                                                      | major  | The scale gives users a way to read the actual sales amounts from the chart.            | None         |
| 7   | layout      | Position sales scale along the left side                                                        | minor  | Placing values on the left is standard for charts since we read from left to right.     | None         |
| 8   | content     | Display chart title "Monthly Sales"                                                             | major  | The title tells viewers right away that they're looking at monthly sales information.   | None         |
| 9   | layout      | Position chart title at top                                                                     | minor  | Top positioning creates a clear header for the visualization.                           | None         |
| 10  | state       | Track hovered position on the area chart                                                         | major  | Keeping track of where the cursor is hovering lets us know which data point to show details for. | None         |
| 11  | interaction | Show tooltip with month and sales amount on hover                                                | major  | When you hover, the tooltip pops up with exact numbers so you don't have to guess from the chart. | C3           |

## Justification

The area chart displays monthly sales data over 6 months with a filled area below the line connecting data points. The area is filled with semi-transparent blue color. Month labels (Jan, Feb, Mar, Apr, May, Jun) display along the bottom and sales values scale displays along the left side. The chart title "Monthly Sales" appears at the top. As users hover over the area, the hovered position is tracked and a tooltip appears showing the month and sales amount for that specific data point.
