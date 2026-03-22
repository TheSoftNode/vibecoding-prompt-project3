Category: Web Application

Prompt style: Featurelist

Title: City Skyline Population

Prompt: Build a web app called "City Skyline Population" with five cities: New York, Atlanta, Nashville, Chicago, and Houston. Show five dark blue bars standing upright from left to right, with each city name under its bar and the population number above it. Include an Edit button on the page. When I click a bar, that bar should become bigger to 120% of its normal height, change from dark blue to green, and stay that way until I click a different bar, then the first one should go back to its normal height and dark blue color. Clicking the Edit button should open an edit page for the selected city with exactly two fields: city name and population, plus a Save button. In the form, the city name should only be one of those five cities, and there should be clear error messages when something is wrong. The form should not submit until everything is filled in correctly.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                        | Weight | Rationale                                                                     | Dependent On |
| --- | ----------- | ------------------------------------------------------------------ | ------ | ----------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 5 dark blue bars standing upright                          | major  | Users need bars as the visual containers for displaying city populations.     | None         |
| 2   | layout      | Arrange bars from left to right                                    | minor  | Left to right arrangement makes it easy to compare populations across cities. | C1           |
| 3   | content     | Display city names: New York, Atlanta, Nashville, Chicago, Houston | major  | City names help users identify which bar represents which city.               | None         |
| 4   | layout      | Position city names under bars                                     | minor  | Under positioning associates each city label with its bar.                    | C3           |
| 5   | content     | Display population numbers                                         | major  | Population numbers tell users the exact population for each city.             | None         |
| 6   | layout      | Position population numbers above bars                             | minor  | Above positioning shows the population count at the top of each bar.          | C5           |
| 7   | visual      | Display Edit button on the page                                    | major  | Edit button provides navigation to the edit page.                             | None         |
| 8   | interaction | Scale clicked bar to 120% of normal height                         | major  | 120% scaling provides visual feedback showing which city is selected.         | None         |
| 9   | visual      | Change clicked bar color from dark blue to green                   | major  | Green color indicates the currently selected city.                            | None         |
| 10  | state       | Keep bar scaled and green until different bar clicked              | major  | Persistent selection state maintains which city is active.                    | C8, C9       |
| 11  | visual      | Revert previous bar to normal height when new bar clicked          | major  | Reverting height ensures only one city is selected at a time.                 | C8           |
| 12  | visual      | Revert previous bar to dark blue when new bar clicked              | major  | Reverting color ensures only one city shows green at a time.                  | C9           |
| 13  | interaction | Navigate to edit page when Edit button clicked                     | major  | Navigation to edit page lets users modify city information.                   | C10          |
| 14  | visual      | Display city name field on edit page                               | major  | City name field lets users select which city to edit.                         | None         |
| 15  | visual      | Display population field on edit page                              | major  | Population field lets users enter new population data.                        | None         |
| 16  | visual      | Display Save button on edit page                                   | major  | Save button lets users submit the edited city information.                    | None         |
| 17  | state       | Restrict city name field to five cities only                       | major  | Restriction ensures only valid city names can be selected.                    | C14          |
| 18  | visual      | Display error messages when something is wrong                     | major  | Error messages inform users what needs to be corrected.                       | C17          |
| 19  | state       | Prevent form submission until everything is filled in correctly    | major  | Submission prevention ensures only correct data is saved.                     | C17          |

## Justification

The City Skyline Population web app works as a multi-page application with bar chart visualization, city selection, and form-based editing. Five dark blue bars display standing upright arranged from left to right representing New York, Atlanta, Nashville, Chicago, and Houston. City names position under their bars and population numbers position above bars. An Edit button displays on the page. When users click a bar, that bar scales to 120% of normal height and changes from dark blue to green, staying that way until a different bar is clicked, then the previous bar reverts to normal height and dark blue color. Clicking the Edit button navigates to an edit page for the selected city with two fields: city name and population, plus a Save button. The city name field restricts to only the five cities and error messages display when something is wrong. The form prevents submission until everything is filled in correctly.
