Category: Data Visualization

Prompt style: Conversational

Title: Constellation Connect Chart

Prompt: I want to visualize my monthly productivity scores as a constellation. Plot five star points on a dark background representing January through May. Connect the stars with lines to form a constellation pattern. Display month labels "January", "February", "March", "April", "May" below each corresponding star. When I click a star, display that month's exact score at the bottom of the chart in large text. Load it with realistic sample productivity scores for the five months.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display a dark background                                | minor  | The dark background creates the night sky effect for the constellation theme.      | None         |
| 2  | visual      | Display five star points on the background               | major  | The star points are essential visual elements that represent the data values.      | None         |
| 3  | content     | Display month labels "January", "February", "March", "April", "May" for each star | major  | Month labels tell users which time period each star represents.                    | None         |
| 4  | layout      | Position month labels below the star points              | minor  | Positioning labels below keeps them associated with their corresponding stars.     | C3           |
| 5  | visual      | Display lines connecting the stars                       | major  | Connecting lines create the constellation pattern that links the data sequence.    | C2           |
| 6  | state       | Load realistic sample productivity scores for the five months | major  | Loading sample data provides the initial values for visualization.                 | None         |
| 7  | interaction | Display clicked month's score when star is clicked       | major  | Showing the score on click gives users detailed information about each data point. | None         |
| 8  | layout      | Position score in large text at the bottom of the chart  | minor  | Large text at the bottom makes the score prominent and easy to read.              | C7           |

## Justification

The Constellation Connect Chart works as expected. A dark background displays with five star points representing January through May. Month labels display below each corresponding star. Lines connect the stars to form a constellation pattern. The chart loads with realistic sample productivity scores, with stars plotted based on these values. When users click a star, that month's exact score displays at the bottom of the chart in large text.
