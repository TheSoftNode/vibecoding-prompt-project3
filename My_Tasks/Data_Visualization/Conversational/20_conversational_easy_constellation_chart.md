Category: Data Visualization

Prompt style: Conversational

Title: Constellation Connect Chart

Prompt: I want to visualize my monthly productivity scores as a constellation. Plot five star points on a dark background representing January through May. Connect the stars with lines to form a constellation pattern. Display month labels "January", "February", "March", "April", "May" below each corresponding star. When I click a star, display that month's exact score at the bottom of the chart in large text. Load it with realistic sample productivity scores for the five months.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display a dark background                                | minor  | The dark background creates a night sky feel that brings the star metaphor to life and helps users see their data as something more than just numbers. | None         |
| 2  | visual      | Display five star points on the background               | major  | Star points give users visual landmarks to anchor to, turning abstract productivity scores into something concrete they can look at and remember. | None         |
| 3  | layout      | Position stars vertically based on productivity scores   | major  | Higher stars mean better months and lower stars mean weaker ones, so users can see their ups and downs just by looking at the shape. | C2, C6       |
| 4  | content     | Display month labels "January", "February", "March", "April", "May" for each star | major  | Labeling each star tells users exactly which month they're looking at without having to guess. | None         |
| 5  | layout      | Position month labels below the star points              | minor  | Labels below the stars stay connected to what they describe while keeping the constellation itself uncluttered. | C4           |
| 6  | visual      | Display lines connecting the stars                       | major  | Connecting lines turn isolated points into a continuous journey, showing the story of how productivity changed over time. | C2           |
| 7  | state       | Load realistic sample productivity scores for the five months | major  | Sample data shows users what a real constellation looks like right away instead of starting with an empty chart. | None         |
| 8  | interaction | Display clicked star's score when star clicked           | major  | Clicking a star shows the actual number behind it for users who want the exact score instead of just the visual. | None         |
| 9  | content     | Show score in large text                                 | major  | Large text makes the number easy to read at a glance without straining. | C8           |
| 10 | layout      | Position score at bottom of chart                        | minor  | Placing the score at the bottom keeps it available when needed but out of the way of the main constellation view. | C9           |

## Justification

The Constellation Connect Chart works exactly as expected. A dark background displays with five star points representing January through May. The chart loads with realistic sample productivity scores for the five months and positions stars vertically based on these score values. Month labels "January", "February", "March", "April", "May" display below each corresponding star point. Lines connect the stars to form a constellation pattern. When users click a star, that month's exact score displays at the bottom of the chart in large text.
