Category: Data_Visualization

Prompt style: Feature_List

Title: Daily Calorie Intake Tracker

Prompt: Build a daily calorie tracker that visualizes meal intake against limits. Display 5 horizontal bars representing Breakfast, Lunch, Snack, Dinner, Late Night, with realistic sample calorie counts. Load initial calorie data showing varied meal intake levels, with some meals meeting and some meals exceeding the 600 calorie limit per meal. Color bars that stayed within the limit (600 or fewer calories) in blue and bars that exceeded the limit in red. When users click any bar, that bar displays a thumbs-up icon at the bottom if it stays within the limit, or a warning icon if it exceeds the limit.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                        | Weight | Rationale                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------- | ------------ |
| 1   | layout      | Display 5 horizontal bars                                                          | major  | Users need bars as the visual containers for displaying meal calorie counts.        | None         |
| 2   | content     | Display meal names Breakfast, Lunch, Snack, Dinner, Late Night                     | major  | Meal names help users identify which meal each bar represents.                      | None         |
| 3   | state       | Load initial calorie data with varied intake levels                                | major  | Loading calorie data initializes the bar values for visualization.                  | None         |
| 4   | state       | Load data with at least one meal meeting and at least one exceeding 600 calorie limit | major  | Mixed data ensures both blue and red bars are visible for comparison.               | None         |
| 5   | content     | Display realistic sample calorie counts                                            | major  | Realistic calorie counts provide believable meal intake data.                       | C3           |
| 6   | visual      | Color bars with 600 or fewer calories blue                                         | major  | Blue color helps users quickly identify meals that stayed within the 600 limit.     | C1, C4       |
| 7   | visual      | Color bars above 600 calories red                                                  | major  | Red color helps users spot meals that exceeded the 600 calorie limit.               | C1, C4       |
| 8   | interaction | Display a thumbs-up icon at the bottom if the bar stayed within the limit when clicked | major  | The thumbs-up icon confirms that the meal successfully stayed within the calorie limit. | None         |
| 9   | interaction | Display the warning icon at the bottom if the bar exceeds the limit when clicked   | major  | The warning icon indicates the meal exceeded the calorie limit.                     | None         |

## Justification

The daily calorie tracker works exactly as expected for visualizing meal intake with limit indicators. Five horizontal bars display representing Breakfast, Lunch, Snack, Dinner, Late Night with realistic sample calorie counts. Initial calorie data loads with varied intake levels showing at least one meal meeting and at least one meal exceeding the 600 calorie limit. Bars with 600 or fewer calories display in blue color while bars above 600 calories display in red color. When users click any bar, that bar displays a thumbs-up icon at the bottom if it stayed within the limit or a warning icon if it exceeds the limit.
