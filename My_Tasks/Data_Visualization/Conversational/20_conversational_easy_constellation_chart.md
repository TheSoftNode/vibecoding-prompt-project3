Category: Data Visualization

Prompt style: Conversational

Title: Constellation Connect Chart

Prompt: I want to visualize my monthly productivity scores as a constellation. Plot five star points on a dark background representing January through May. Connect the stars with lines to form a constellation pattern. Display month labels "January", "February", "March", "April", "May" below each corresponding star. When I click a star, display that month's exact score at the bottom of the chart in large text. Load it with realistic sample productivity scores for the five months.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display a dark background                                | minor  | The dark background creates the night sky atmosphere for the constellation theme. | None         |
| 2  | visual      | Display five star points on the background               | major  | The star points represent the productivity data visually for each month. | None         |
| 3  | layout      | Position stars vertically based on productivity scores   | major  | Vertical positioning creates the data mapping where higher stars mean better performance. | C2, C6       |
| 4  | content     | Display month labels "January", "February", "March", "April", "May" for each star | major  | Month labels help users identify which time period each star represents. | None         |
| 5  | layout      | Position month labels below the star points              | minor  | Placing labels below keeps them associated with their stars while keeping the chart clean. | C4           |
| 6  | visual      | Display lines connecting the stars                       | major  | Connecting lines form the constellation pattern showing the progression across months. | C2           |
| 7  | state       | Load realistic sample productivity scores for the five months | major  | Loading sample data provides the initial values for the chart visualization. | None         |
| 8  | interaction | Display clicked star's score when star clicked           | major  | Clicking a star reveals the exact numeric value behind that data point. | None         |
| 9  | content     | Show score in large text                                 | major  | Large text makes the score easy to read when displayed. | C8           |
| 10 | layout      | Position score at bottom of chart                        | minor  | Bottom positioning separates the detail from the main constellation visualization. | C9           |

## Justification

The Constellation Connect Chart works exactly as expected. A dark background displays with five star points representing January through May. The chart loads with realistic sample productivity scores for the five months and positions stars vertically based on these score values. Month labels "January", "February", "March", "April", "May" display below each corresponding star point. Lines connect the stars to form a constellation pattern. When users click a star, that month's exact score displays at the bottom of the chart in large text.
