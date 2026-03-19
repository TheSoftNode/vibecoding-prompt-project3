Category: Data_Visualization

Prompt style: Feature_List

Title: Step Counter Ladder

Prompt: Build a step counter ladder that visualizes daily walking progress. Display 6 horizontal bars stacked vertically like ladder rungs representing Sunday through Friday with step counts 8500 steps, 12000 steps, 6700 steps, 10200 steps, 9100 steps, 11500 steps. Each bar fills from left to right based on step count with the goal being 10000 steps. Color bars that reached the goal (10000+ steps) in green and bars below the goal in orange. Display the day name on the left edge of each bar and the step count on the right edge. When users click any bar, that bar displays a checkmark icon on the left side if it met the goal or an X icon if it did not meet the goal.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                  | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | ------------------------------------------------------------ | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display 6 horizontal bars                                    | major  | Users need bars as the visual containers for displaying daily step counts.     | None         |
| 2   | layout      | Stack bars vertically like ladder rungs                      | minor  | Ladder-style stacking makes it easy to scan progress across all days at once. | C1           |
| 3   | content     | Display day names: Sunday, Monday, Tuesday, Wednesday, Thursday, Friday | major  | Day names help users identify which day each bar represents.                   | None         |
| 4   | layout      | Position day names on left edge of bars                      | minor  | Left positioning associates each day label with the start of its progress bar. | C3           |
| 5   | content     | Display step counts: 8500, 12000, 6700, 10200, 9100, 11500   | major  | Step counts tell users the exact walking activity achieved each day.           | None         |
| 6   | layout      | Position step count on right edge of bar                     | minor  | Right positioning shows the final step count at the end of the progress bar.   | C5           |
| 7   | state       | Fill bar from left to right based on step count             | major  | Left-to-right filling creates a visual gauge showing progress toward the goal. | None         |
| 8   | visual      | Color bars with 10000+ steps green                           | major  | Green color helps users quickly identify days that met the 10000 step goal.    | None         |
| 9   | visual      | Color bars below 10000 steps orange                          | major  | Orange color helps users spot days that fell short of the 10000 step goal.     | None         |
| 10  | interaction | Display checkmark icon on left if bar met goal when clicked  | major  | Checkmark icon confirms the day successfully achieved the step goal.           | None         |
| 11  | interaction | Display X icon on left if bar did not meet goal when clicked | major  | X icon indicates the day did not reach the step goal.                          | None         |

## Justification

The step counter ladder works exactly as expected for visualizing daily walking progress with goal indicators. Six horizontal bars display stacked vertically like ladder rungs with day names "Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", and "Friday" positioned on the left edge of each bar. Step counts "8500 steps", "12000 steps", "6700 steps", "10200 steps", "9100 steps", and "11500 steps" display on the right edge of each bar. Each bar fills from left to right based on step count toward the 10000 step goal. Bars with 10000+ steps (Monday, Wednesday, Friday) display in green color while bars below 10000 steps (Sunday, Tuesday, Thursday) display in orange color. When users click any bar, that bar displays a checkmark icon on the left side if it met the goal or an X icon if it did not meet the goal.
