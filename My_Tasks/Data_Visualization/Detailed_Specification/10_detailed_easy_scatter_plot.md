Category: Data Visualization

Prompt style: Detailed Specification

Title: Lollipop Chart for Rankings

Prompt: Create a lollipop chart showing top 8 programming languages by popularity score. Each language has a stem line from the axis to a circle marker. Display language names on Y-axis and popularity scores on X-axis with range 0 to 100. Color all circle markers blue. Calculate and display the average popularity score as a vertical reference line across the chart. Add a "Show Above Average Only" toggle button that filters the chart to display only languages with scores above the average when enabled. When clicking a marker, highlight it with a bold border and display that language's exact score in a detail box below the chart. Keep the marker highlighted and score displayed until a different marker is clicked. Add chart title "Top Programming Languages 2024" and axis labels.

Required libraries: react, tailwindcss, recharts

## Rubric

| #   | ID      | Description                                            | Weight | Rationale                                                                               | Dependent On |
| --- | ------- | ------------------------------------------------------ | ------ | --------------------------------------------------------------------------------------- | ------------ |
| 1   | visual  | Display 8 stem lines connecting markers to Y-axis      | major  | Stem lines create the lollipop structure connecting axis to data points.                | None         |
| 2   | visual  | Display circle markers for each language               | major  | Circle markers represent the data values visually for each language.                    | None         |
| 3   | layout  | Position circle markers at end of each stem            | minor  | Positioning circles at stem ends creates the complete lollipop structure.               | C1, C2       |
| 4   | content | Display 8 programming language names                   | major  | Language names help users identify which language each lollipop represents.             | None         |
| 5   | layout  | Position language names on Y-axis                      | minor  | Y-axis positioning creates categorical ranking structure.                               | C4           |
| 6   | content | Display X-axis with 0 to 100 range                     | major  | X-axis range defines the popularity scale for measuring language scores.                | None         |
| 7   | layout  | Position each marker according to its popularity score | major  | Horizontal positioning encodes the score value for each language.                       | C2           |
| 8   | visual      | Color all markers blue                                 | minor  | Blue color provides consistent visual identity for all data points.                     | None         |
| 9   | state       | Calculate average popularity score from all languages  | major  | Computing the average provides a statistical benchmark for comparing individual scores.  | None         |
| 10  | visual      | Display vertical reference line for average score      | major  | The reference line visually marks the average value across the chart.                    | C9           |
| 11  | layout      | Position reference line at calculated average value    | minor  | Positioning the line at the average score shows the statistical benchmark visually.      | C9, C10      |
| 12  | visual      | Display "Show Above Average Only" toggle button        | major  | The toggle button provides the control for filtering languages by average threshold.     | None         |
| 13  | interaction | Filter chart to above-average languages when toggled   | major  | Toggling filters the visible data to show only high-performing languages.                | C9, C12      |
| 14  | state       | Hide below-average languages when toggle is enabled    | major  | Maintaining filter state updates the chart to display only relevant subset of data.      | C13          |
| 15  | interaction | Highlight marker with bold border when clicked         | major  | Clicking highlights the marker to show which language is selected.                       | None         |
| 16  | interaction | Display exact score in detail box below chart          | major  | Showing the exact score provides precise numerical data for the selected language.       | C15          |
| 17  | state       | Keep marker highlighted until different marker clicked | major  | Maintaining highlight state shows which language remains selected for examination.       | C15          |
| 18  | state       | Keep score displayed until different marker clicked    | major  | Maintaining score display state shows the selected language's data persistently.         | C16          |
| 19  | content     | Display chart title "Top Programming Languages 2024"   | major  | The title identifies what data the chart shows and its time context.                     | None         |
| 20  | content     | Display axis labels                                    | minor  | Axis labels clarify what each axis represents for easy interpretation.                   | C5, C6       |
