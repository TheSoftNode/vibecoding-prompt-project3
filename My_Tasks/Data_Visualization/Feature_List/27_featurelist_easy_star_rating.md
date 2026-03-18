Category: Data_Visualization

Prompt style: Feature_List

Title: Product Review Rating Breakdown

Prompt: Build a review rating breakdown visualization. Display 5 rows for star ratings from 5-star to 1-star. Each row shows the star count label (e.g., "5 Stars"), a horizontal bar showing the percentage of reviews, and the review count. Use data: 5-star (120 reviews, 60%), 4-star (50 reviews, 25%), 3-star (20 reviews, 10%), 2-star (8 reviews, 4%), 1-star (2 reviews, 1%). Color bars from green (5-star) gradually to red (1-star). Display average rating "4.3 out of 5" at the top.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display "4.3 out of 5" average rating at top         | major  | The average gives users a quick summary of overall ratings.                                  | None         |
| 2   | layout      | Position average rating at top                       | minor  | Top positioning makes the summary immediately visible.                                       | C1           |
| 3   | content     | Display "5 Stars" label in first row                 | minor  | The label identifies the highest rating category.                                            | None         |
| 4   | content     | Display "4 Stars" label in second row                | minor  | The label identifies the second rating category.                                             | None         |
| 5   | content     | Display "3 Stars" label in third row                 | minor  | The label identifies the middle rating category.                                             | None         |
| 6   | content     | Display "2 Stars" label in fourth row                | minor  | The label identifies the second-lowest rating category.                                      | None         |
| 7   | content     | Display "1 Star" label in fifth row                  | minor  | The label identifies the lowest rating category.                                             | None         |
| 8   | visual      | Display horizontal bar for 5-star reviews            | major  | The bar visualizes the proportion of 5-star reviews.                                         | None         |
| 9   | visual      | Display horizontal bar for 4-star reviews            | major  | The bar visualizes the proportion of 4-star reviews.                                         | None         |
| 10  | visual      | Display horizontal bar for 3-star reviews            | major  | The bar visualizes the proportion of 3-star reviews.                                         | None         |
| 11  | visual      | Display horizontal bar for 2-star reviews            | major  | The bar visualizes the proportion of 2-star reviews.                                         | None         |
| 12  | visual      | Display horizontal bar for 1-star reviews            | major  | The bar visualizes the proportion of 1-star reviews.                                         | None         |
| 13  | state       | Size 5-star bar to 60% width                         | major  | Bar size represents the percentage of total reviews.                                         | None         |
| 14  | state       | Size 4-star bar to 25% width                         | major  | Bar size represents the percentage of total reviews.                                         | None         |
| 15  | state       | Size 3-star bar to 10% width                         | major  | Bar size represents the percentage of total reviews.                                         | None         |
| 16  | state       | Size 2-star bar to 4% width                          | major  | Bar size represents the percentage of total reviews.                                         | None         |
| 17  | state       | Size 1-star bar to 1% width                          | major  | Bar size represents the percentage of total reviews.                                         | None         |
| 18  | content     | Display "120" review count for 5-star                | minor  | The count shows how many people gave this rating.                                            | None         |
| 19  | content     | Display "50" review count for 4-star                 | minor  | The count shows how many people gave this rating.                                            | None         |
| 20  | content     | Display "20" review count for 3-star                 | minor  | The count shows how many people gave this rating.                                            | None         |
| 21  | content     | Display "8" review count for 2-star                  | minor  | The count shows how many people gave this rating.                                            | None         |
| 22  | content     | Display "2" review count for 1-star                  | minor  | The count shows how many people gave this rating.                                            | None         |
| 23  | visual      | Color 5-star bar green                               | minor  | Green indicates excellent ratings.                                                           | None         |
| 24  | visual      | Color 4-star bar light green                         | minor  | Light green indicates good ratings.                                                          | None         |
| 25  | visual      | Color 3-star bar yellow                              | minor  | Yellow indicates neutral ratings.                                                            | None         |
| 26  | visual      | Color 2-star bar orange                              | minor  | Orange indicates poor ratings.                                                               | None         |
| 27  | visual      | Color 1-star bar red                                 | minor  | Red indicates the worst ratings.                                                             | None         |

## Justification

The product review rating breakdown works exactly as expected for visualizing rating distribution. At the top, "4.3 out of 5" displays showing the average rating. Below, five rows display from 5-star to 1-star. Each row shows the star label, a horizontal bar sized to match the percentage, and the review count. The 5-star row shows "5 Stars", a green bar at 60% width, and "120" reviews. The 4-star row shows "4 Stars", a light green bar at 25% width, and "50" reviews. The 3-star row shows "3 Stars", a yellow bar at 10% width, and "20" reviews. The 2-star row shows "2 Stars", an orange bar at 4% width, and "8" reviews. The 1-star row shows "1 Star", a red bar at 1% width, and "2" reviews.
