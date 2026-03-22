Category: Data_Visualization

Prompt style: Feature_List

Title: Daily Calorie Intake Tracker

Prompt: Build a daily calorie tracker that visualizes meal intake against limits. Display 5 horizontal bars representing Breakfast, Lunch, Snack, Dinner, Late Night, with realistic sample calorie counts. Load initial calorie data showing varied meal intake levels, with two meals meeting and three meals exceeding the 600 calorie limit per meal. When users click any bar, that bar displays a thumbs-up icon at the bottom if it stays within the limit (600 or fewer calories), or a warning icon if it exceeds the limit (above 600 calories), and the bar color changes to blue if within limit or red if exceeding limit.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                        | Weight | Rationale                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 5 horizontal bars                                                          | major  | Users need bars as the visual containers for displaying meal calorie counts.        | None         |
| 2   | content     | Display meal names Breakfast, Lunch, Snack, Dinner, Late Night                     | major  | Meal names help users identify which bar each represents.                           | None         |
| 3   | state       | Load initial calorie data with varied intake levels                                | major  | Loading calorie data initializes the bar values for visualization.                  | None         |
| 4   | state       | Load data with two meals meeting and three meals exceeding 600 calorie limit       | major  | Specific mix ensures both icons and colors will be tested.                          | None         |
| 5   | content     | Display sample calorie counts for each meal                                        | major  | Calorie counts show the exact intake value for each meal.                           | C3           |
| 6   | interaction | Display thumbs-up icon at bottom when bar clicked if within 600 calorie limit      | major  | Thumbs-up icon confirms that the meal successfully stayed within the calorie limit. | None         |
| 7   | interaction | Display warning icon at bottom when bar clicked if exceeds 600 calorie limit       | major  | Warning icon indicates the meal exceeded the calorie limit.                         | None         |
| 8   | visual      | Change bar color to blue when clicked if within 600 calorie limit                  | major  | Blue color helps users quickly identify meals that stayed within the 600 limit.     | C6           |
| 9   | visual      | Change bar color to red when clicked if exceeds 600 calorie limit                  | major  | Red color helps users spot meals that exceeded the 600 calorie limit.               | C7           |

## Justification

The daily calorie tracker works exactly as expected for visualizing meal intake with limit indicators. Five horizontal bars display representing Breakfast, Lunch, Snack, Dinner, Late Night with sample calorie counts. Initial calorie data loads with varied intake levels showing two meals meeting and three meals exceeding the 600 calorie limit. When users click any bar, that bar displays a thumbs-up icon at the bottom if it stays within the limit or a warning icon if it exceeds the limit, and the bar color changes to blue if within limit or red if exceeding limit.
