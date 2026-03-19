Category: Data_Visualization

Prompt style: Feature_List

Title: Step Counter Ladder

Prompt: Build a step counter ladder that visualizes daily walking progress. Display 6 horizontal bars stacked vertically like ladder rungs representing Sunday through Friday with realistic sample step counts. Load initial step data showing varied daily activity levels with some days meeting and some days missing the 10000 step goal. Each bar fills from left to right based on step count with the goal being 10000 steps. Color bars that reached the goal (10000+ steps) in green and bars below the goal in orange. Display the day name on the left edge of each bar and the step count on the right edge. When users click any bar, that bar displays a checkmark icon on the left side if it met the goal or an X icon if it did not meet the goal.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                  | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | ------------------------------------------------------------ | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display 6 horizontal bars                                    | major  | Users need bars as the visual containers for displaying daily step counts.     | None         |
| 2   | layout      | Stack bars vertically like ladder rungs                      | minor  | Ladder-style stacking makes it easy to scan progress across all days at once. | C1           |
| 3   | content     | Display day names: Sunday, Monday, Tuesday, Wednesday, Thursday, Friday | major  | Day names help users identify which day each bar represents.                   | None         |
| 4   | layout      | Position day names on the left edge of bars                  | minor  | Left positioning associates each day's label with the start of its progress bar. | C3           |
| 5   | state       | Load initial step data with varied activity levels          | major  | Loading step data initializes the bar values for visualization.               | None         |
| 6   | content     | Display step counts on bars                                  | major  | Step counts tell users the exact walking activity achieved each day.           | C5           |
| 7   | layout      | Position the step count on the right edge of the bar         | minor  | Right positioning shows the final step count at the end of the progress bar.   | C6           |
| 8   | visual      | Fill the bar from left to right based on the step count     | major  | Left-to-right filling creates a visual gauge showing progress toward the goal. | C5           |
| 9   | visual      | Color bars with 10000+ steps green                           | major  | The green color helps users quickly identify days that met the 10000-step goal. | None         |
| 10  | visual      | Color bars below 10000 steps orange                          | major  | Orange color helps users spot days that fell short of the 10000-step goal.     | None         |
| 11  | interaction | Display a checkmark icon on the left if the bar met the goal when clicked | major  | Checkmark icon confirms that the day successfully achieved the step goal.      | None         |
| 12  | interaction | Display the X icon on the left if the bar did not meet the goal when clicked | major  | The X icon indicates the day did not reach the step goal.                     | None         |

## Justification

The step counter ladder works exactly as expected for visualizing daily walking progress with goal indicators. Six horizontal bars display stacked vertically like ladder rungs with day names "Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", and "Friday" positioned on the left edge of each bar. Initial step data loads with varied activity levels showing some days meeting and some days missing the 10000 step goal. Step counts display on the right edge of each bar. Each bar fills from left to right based on step count toward the 10000 step goal. Bars with 10000+ steps display in green color while bars below 10000 steps display in orange color. When users click any bar, that bar displays a checkmark icon on the left side if it met the goal or an X icon if it did not meet the goal.
