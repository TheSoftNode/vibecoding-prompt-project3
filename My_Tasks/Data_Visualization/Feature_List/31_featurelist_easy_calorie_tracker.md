Category: Data_Visualization

Prompt style: Feature_List

Title: Daily Calorie Intake Tracker

Prompt: Build a daily calorie tracker that visualizes meal intake against limits. Display 5 vertical bars stacked horizontally representing Breakfast, Lunch, Snack, Dinner, Late Night with realistic sample calorie counts. Load initial calorie data showing varied meal intake levels with some meals meeting and some meals exceeding the 600 calorie limit per meal. Color bars that stayed within the limit (600 or fewer calories) in blue and bars that exceeded the limit in red. When users click any bar, that bar displays a thumbs-up icon at the bottom if it stayed within the limit or a warning icon if it exceeded the limit.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                  | Weight | Rationale                                                                          | Dependent On |
| --- | ----------- | ---------------------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 5 vertical bars                                                      | major  | Users need bars as the visual containers for displaying meal calorie counts.       | None         |
| 2   | layout      | Stack bars horizontally                                                      | minor  | Horizontal stacking makes it easy to compare intake across all meals at once.      | C1           |
| 3   | content     | Display meal names Breakfast, Lunch, Snack, Dinner, Late Night               | major  | Meal names help users identify which meal each bar represents.                     | None         |
| 4   | state       | Load initial calorie data with varied intake levels                          | major  | Loading calorie data initializes the bar values for visualization.                 | None         |
| 5   | visual      | Color bars with 600 or fewer calories blue                                   | major  | Blue color helps users quickly identify meals that stayed within the 600 limit.    | None         |
| 6   | visual      | Color bars above 600 calories red                                            | major  | Red color helps users spot meals that exceeded the 600 calorie limit.              | None         |
| 7   | interaction | Display a thumbs-up icon at the bottom if the bar stayed within limit when clicked | major  | Thumbs-up icon confirms that the meal successfully stayed within the calorie limit.| None         |
| 8   | interaction | Display the warning icon at the bottom if the bar exceeded limit when clicked | major  | Warning icon indicates the meal exceeded the calorie limit.                        | None         |

## Justification

The daily calorie tracker works exactly as expected for visualizing meal intake with limit indicators. Five vertical bars display stacked horizontally representing Breakfast, Lunch, Snack, Dinner, Late Night. Initial calorie data loads with varied intake levels showing some meals meeting and some meals exceeding the 600 calorie limit. Bars with 600 or fewer calories display in blue color while bars above 600 calories display in red color. When users click any bar, that bar displays a thumbs-up icon at the bottom if it stayed within the limit or a warning icon if it exceeded the limit.
