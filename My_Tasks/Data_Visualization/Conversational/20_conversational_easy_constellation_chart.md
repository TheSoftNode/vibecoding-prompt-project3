Category: Data Visualization

Prompt style: Conversational

Title: Constellation Connect Chart

Prompt: I want to visualize my monthly productivity scores as a constellation. Plot five star points on a dark background representing January through May. Connect the stars with lines to form a constellation pattern. Display month labels "January", "February", "March", "April", "May" below each corresponding star. When I click a star, display that month's exact score at the bottom of the chart in large text. Load it with realistic sample productivity scores for the five months.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display a dark background                                | minor  | The dark background creates a night-sky atmosphere for the constellation theme. | None         |
| 2  | visual      | Display five star points on the background               | major  | The star points represent the productivity data visually for each month. | None         |
| 3  | visual      | Display lines connecting the stars                       | major  | Connecting lines form a constellation pattern that shows the progression across months. | None         |
| 4  | content     | Display month labels "January", "February", "March", "April", "May" for each star | major  | Month labels help users identify which time period each star represents. | None         |
| 5  | layout      | Position month labels below the star points              | minor  | Placing labels below keeps them associated with their stars while keeping the chart clean. | None         |
| 6  | state       | Load realistic sample productivity scores for the five months | major  | Loading sample data provides the initial values for the chart visualization. | None         |
| 7  | interaction | Display the clicked star's score when the star is clicked | major  | Clicking a star reveals the exact numeric value behind that data point. | None         |
| 8  | content     | Show score in large text                                 | major  | Large text makes the score easy to read when displayed. | C7           |
| 9  | layout      | Position score at the bottom of the chart                | minor  | Bottom positioning separates the detail from the main constellation visualization. | C8           |

## Justification

The Constellation Connect Chart works exactly as expected. A dark background displays with five star points representing January through May. Lines connect the stars to form a constellation pattern. Month labels "January", "February", "March", "April", "May" display below each corresponding star point. The chart loads with realistic sample productivity scores for the five months. When users click a star, that month's exact score displays in large text at the bottom of the chart.
