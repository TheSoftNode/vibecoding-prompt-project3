Category: Data Visualization

Prompt style: Conversational

Title: Constellation Connect Chart

Prompt: I want to visualize my monthly productivity scores as a constellation. Plot five star points on a dark background representing January through May with scores 75, 85, 60, 90, 70. Connect the stars with lines to form a constellation pattern. Label each star with its month name below it. When I click a star, display that month's exact score in large text at the bottom of the chart. Load it with the sample data I mentioned.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display a dark background                                | minor  | The dark background creates the night sky effect for the constellation theme.      | None         |
| 2  | visual      | Display five star points on the background               | major  | The star points are essential visual elements that represent the data values.      | None         |
| 3  | content     | Label each star with month name below it                 | major  | Month labels tell users which time period each star represents.                    | C2           |
| 4  | layout      | Position month labels below the star points              | minor  | Positioning labels below keeps them associated with their corresponding stars.     | C3           |
| 5  | visual      | Display lines connecting the stars                       | major  | Connecting lines create the constellation pattern that links the data sequence.    | C2           |
| 6  | layout      | Connect stars to form a constellation pattern            | major  | The pattern arrangement creates the visual flow showing progression over months.   | C5           |
| 7  | state       | Load sample data for the five months with given scores   | major  | Loading sample data provides the initial values for visualization.                 | None         |
| 8  | state       | Plot stars based on loaded score values                  | major  | Plotting by score values accurately represents the data through star positioning.  | C7           |
| 9  | interaction | Display clicked month's score when star is clicked       | major  | Showing the score on click gives users detailed information about each data point. | None         |
| 10 | content     | Display score in large text at the bottom of the chart   | major  | Large text at the bottom makes the selected score easy to read.                    | C9           |

## Justification

The Constellation Connect Chart works as expected. A dark background displays with five star points representing January through May. Each star has its month name labeled below it. Lines connect the stars to form a constellation pattern. The chart loads with sample data showing scores 75, 85, 60, 90, 70, with stars plotted based on these values. When users click a star, that month's exact score displays in large text at the bottom of the chart.
