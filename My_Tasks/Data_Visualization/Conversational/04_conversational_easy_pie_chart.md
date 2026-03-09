Category: Data Visualization

Prompt style: Conversational

Title: Weekly Activity Heatmap

Prompt: Need a weekly activity heatmap showing my productivity for 7 days. Display a row of 7 squares representing Monday through Sunday. Color each square based on tasks completed: white for 0 tasks, light green for 1-3 tasks, medium green for 4-6 tasks, and dark green for 7+ tasks. Use these values: Monday 5 tasks, Tuesday 2 tasks, Wednesday 8 tasks, Thursday 0 tasks, Friday 6 tasks, Saturday 3 tasks, Sunday 7 tasks. When I click a square, show the day name and task count below the heatmap. Also display the total tasks for the week below the heatmap as the sum of all days.

Required libraries: react, tailwindcss, recharts

## Rubric

| #   | ID          | Description                                                                                                    | Weight | Rationale                                                                               | Dependent On |
| --- | ----------- | -------------------------------------------------------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Render a row of 7 squares representing days of the week                                                        | major  | The squares create the heatmap grid to visualize daily activity levels.                 | None         |
| 2   | content     | Display task counts: Monday 5, Tuesday 2, Wednesday 8, Thursday 0, Friday 6, Saturday 3, Sunday 7              | major  | These specific values provide the actual task completion data for each day.             | C1           |
| 3   | visual      | Display white color for 0 tasks (Thursday)                                                                     | major  | White indicates no tasks completed that day.                                            | C2           |
| 4   | visual      | Display light green color for 1-3 tasks (Tuesday and Saturday)                                                 | major  | Light green indicates low activity level.                                               | C2           |
| 5   | visual      | Display medium green color for 4-6 tasks (Monday and Friday)                                                   | major  | Medium green indicates moderate activity level.                                         | C2           |
| 6   | visual      | Display dark green color for 7+ tasks (Wednesday and Sunday)                                                   | major  | Dark green indicates high activity level meeting or exceeding goals.                    | C2           |
| 7   | interaction | Show day name and task count below the heatmap when a square is clicked                                        | major  | Clicking reveals detailed information about the selected day.                           | C1           |
| 8   | content     | Display the clicked day's name and task count                                                                  | major  | Day name and count provide specific details about the selected square.                  | C7           |
| 9   | state       | Calculate total tasks as the sum of all daily task counts                                                      | major  | The total is computed by summing all 7 days of task completion.                         | C2           |
| 10  | content     | Display total tasks for the week below the heatmap                                                             | major  | The total shows overall weekly productivity.                                            | C9           |
| 11  | layout      | Position the total tasks below the heatmap                                                                     | minor  | Placing the total below separates summary information from the grid visualization.      | C10          |

## Justification

The weekly activity heatmap works exactly as expected with 7 squares representing Monday through Sunday. Each square displays in the correct color based on task count: Thursday shows white (0 tasks), Tuesday and Saturday show light green (2 and 3 tasks), Monday and Friday show medium green (5 and 6 tasks), and Wednesday and Sunday show dark green (8 and 7 tasks). When clicking any square, the day name and task count appear below the heatmap showing the details for that selected day. Below the heatmap, the total tasks for the week displays as 31, calculated as the sum of all 7 daily task counts.
