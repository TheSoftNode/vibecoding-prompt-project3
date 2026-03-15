Category: Data Visualization

Prompt style: Casual

Title: Donut Chart with Center Text

Prompt: Need a donut chart showing how I spend my time on daily activities. Make it with five slices for Work, Sleep, Exercise, Leisure, and Other. Give each slice a different color and show the activity name on each slice. The center should show the total hours (24). When I click a slice, update the center to show that activity's exact hours and percentage with a fade-in animation. Load it with some realistic sample data.

Required libraries: react, tailwindcss, recharts, lucide-react

## Rubric

| #  | ID          | Description                                                   | Weight | Rationale                                                                      | Dependent On |
|----|-------------|---------------------------------------------------------------|--------|--------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display a donut chart with 5 slices                           | major  | The donut chart provides the visual structure for displaying time proportions. | None         |
| 2  | visual      | Apply a different color to each slice                         | major  | Different colors help users visually distinguish between activities.           | C1           |
| 3  | content     | Display activity name on each slice                           | major  | Activity names help users identify which slice represents each activity.       | C1           |
| 4  | layout      | Position activity names on the slices                         | minor  | Positioning names on slices ensures immediate visibility without interaction.  | C3           |
| 5  | content     | Display total hours (24) in the center initially              | major  | The initial center text provides the total time context for all activities.    | None         |
| 6  | layout      | Position total hours text in the center of the donut          | minor  | Center positioning makes the total immediately visible to users.               | C5           |
| 7  | state       | Load realistic sample data for the five activities            | minor  | Sample data enables users to see the chart working with realistic values.      | None         |
| 8  | interaction | Update center text with fade-in animation when slice clicked  | major  | The fade-in animation creates a smooth transition when displaying new details. | None         |
| 9  | content     | Display exact hours for clicked activity in center            | major  | Exact hours give users precise time values for the selected activity.          | C8           |
| 10 | content     | Display percentage for clicked activity in center             | major  | The percentage shows the proportion of time for the selected activity.         | C8           |

## Justification

The Donut Chart with Center Text works as expected with a smooth fade-in animation. A donut chart displays with five colored slices representing Work, Sleep, Exercise, Leisure, and Other activities. Each slice shows the activity name positioned on the slice. The center initially displays "24" indicating total hours. When users click any slice, the center updates with a fade-in animation to show that activity's exact hours and percentage.
