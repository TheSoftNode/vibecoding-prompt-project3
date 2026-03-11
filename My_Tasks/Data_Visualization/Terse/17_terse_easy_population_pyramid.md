Category: Data Visualization

Prompt style: Terse

Title: Animated Population Pyramid

Prompt: Population pyramid. Age groups 0-10, 11-20, 21-30, 31-40, 41-50, 51-60, 61-70, 71-80, 81-90, 91-100. Male bars left (blue), female bars right (pink). Animate bars growing from zero to full width on load. Hover shows exact count.

Required libraries: react, tailwindcss, recharts

## Rubric

| #   | ID          | Description                                              | Weight | Rationale                                                                                                    | Dependent On |
| --- | ----------- | -------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display 10 age group labels vertically centered         | major  | Age labels are essential for users to identify which demographic segment each bar represents.                | None         |
| 2   | visual      | Display male bars extending left from center in blue    | major  | Blue male bars extending left create the distinctive left half of the population pyramid structure.          | None         |
| 3   | visual      | Display female bars extending right from center in pink | major  | Pink female bars extending right complete the pyramid by showing the female population distribution.         | None         |
| 4   | content     | Display age group ranges in format "X-Y" for each row   | minor  | Showing ranges like "0-10" or "51-60" clarifies the exact age span each bar represents.                     | None         |
| 5   | layout      | Align male and female bars symmetrically around center   | minor  | Symmetric alignment around the center creates the classic pyramid shape for easy comparison.                 | None         |
| 6   | state       | Animate bars from zero width to data width on page load  | major  | Animation on load draws attention to the data and makes the visualization more engaging and memorable.       | None         |
| 7   | interaction | Display tooltip with exact population count on hover     | major  | Hover tooltips let users see precise numbers instead of estimating from bar length alone.                    | None         |
| 8   | layout      | Position age labels between left and right bars         | minor  | Centering labels between bars makes them equally accessible for reading both male and female data.          | None         |
| 9   | content     | Display "Male" label above left side bars               | minor  | A "Male" label clarifies which side represents male population without relying solely on color.              | None         |
| 10  | content     | Display "Female" label above right side bars            | minor  | A "Female" label ensures users understand which side is female, improving accessibility beyond color coding. | None         |

## Justification

The application achieved an 88.89% pass rate with one specific failure. The population pyramid displays 10 age groups (0-10 through 91-100) with age labels vertically centered. Male bars extend left from center in blue and female bars extend right in pink, creating the symmetric pyramid structure. Age group ranges appear in "X-Y" format for each row. "Male" and "Female" labels appear above their respective sides. On page load, bars animate from zero width to their full data width. Hovering over any bar displays a tooltip showing the exact population count for that age group and gender. However, the model failed to position age labels between the left and right bars. Instead, labels appear on the far left outside the male bars, not centered between the two sides as required. This positioning issue caused the failure despite all other functionality working correctly.
