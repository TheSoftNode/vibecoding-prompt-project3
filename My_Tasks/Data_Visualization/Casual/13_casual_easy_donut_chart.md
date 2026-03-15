Category: Data Visualization

Prompt style: Casual

Title: Donut Chart with Center Text

Prompt: Need a donut chart showing how I spend my time on daily activities. Make it with five slices for Work, Sleep, Exercise, Leisure, and Other. Give each slice a different color and show the activity name on each slice. The center should show the total hours (24). When I click a slice, update the center to show that activity's exact hours and percentage. Load it with some realistic sample data.

Required libraries: react, tailwindcss, recharts, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display a donut chart with 5 slices                  | major  | The donut chart provides the visual structure for displaying time proportions. | None         |
| 2   | visual      | Apply a different color to each slice                | minor  | Different colors help users visually distinguish between activities.           | None         |
| 3   | content     | Display activity name on each slice                  | major  | Activity names help users identify which slice represents each activity.       | None         |
| 4   | layout      | Position activity names on the slices                | minor  | Positioning names on slices ensures immediate visibility without interaction.  | None         |
| 5   | content     | Display total hours (24) in the center initially     | major  | The initial center text provides the total time context for all activities.    | None         |
| 6   | layout      | Position total hours text in the center of the donut | minor  | Center positioning makes the total immediately visible to users.               | None         |
| 7   | state       | Load realistic sample data for the five activities   | minor  | Sample data enables users to see the chart working with realistic values.      | None         |
| 8   | interaction | Display exact hours for clicked activity in center   | major  | Exact hours give users precise time values for the selected activity.          | None         |
| 9   | interaction | Display percentage for clicked activity in center    | major  | The percentage shows the proportion of time for the selected activity.         | None         |

## Justification

The Donut Chart with Center Text achieved 88.89% pass rate with one failure. A donut chart displays with five colored slices representing Work, Sleep, Exercise, Leisure, and Other activities, each with a different color. The center initially displays "24hrs" indicating total hours. The chart loads with realistic sample data. When users click any slice, the center updates to show that activity's exact hours and percentage. However, the activity names on the slices are not clearly visible - some labels are cut off while others are not visible at all, making it difficult to identify which slice represents which activity.
