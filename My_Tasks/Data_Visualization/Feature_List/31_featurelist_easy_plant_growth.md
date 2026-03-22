Category: Data_Visualization

Prompt style: Feature_List

Title: Plant Growth Tracker

Prompt: Build a plant growth tracker that visualizes growth progress against targets. Display 5 vertical stems representing Basil, Mint, Sage, Thyme, Parsley, with realistic sample heights in centimeters. Load initial growth data showing varied stem heights, with at least one plant meeting and at least one exceeding the 15 cm target height. Color stems that stayed within the target (15 or fewer cm) in green and stems that exceeded the target in yellow. When users click any stem, that stem displays a sprout icon at the top if it stayed within the target, or a flower icon if it exceeds the target.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                        | Weight | Rationale                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------- | ------------ |
| 1   | layout      | Display 5 vertical stems                                                           | major  | Users need stems as the visual containers for displaying plant growth heights.      | None         |
| 2   | content     | Display plant names Basil, Mint, Sage, Thyme, Parsley                              | major  | Plant names help users identify which plant each stem represents.                   | None         |
| 3   | state       | Load initial growth data with varied stem heights                                  | major  | Loading growth data initializes the stem values for visualization.                  | None         |
| 4   | state       | Load data with at least one plant meeting and at least one exceeding 15 cm target  | major  | Mixed data ensures both green and yellow stems are visible for comparison.          | None         |
| 5   | content     | Display realistic sample heights in centimeters                                     | major  | Realistic heights provide believable plant growth data.                             | C3           |
| 6   | visual      | Color stems with 15 or fewer cm green                                              | major  | Green color helps users quickly identify plants that stayed within the 15 cm target.| C1, C4       |
| 7   | visual      | Color stems above 15 cm yellow                                                     | major  | Yellow color helps users spot plants that exceeded the 15 cm target.                | C1, C4       |
| 8   | interaction | Display a sprout icon at the top if the stem stayed within the target when clicked | major  | The sprout icon confirms that the plant successfully stayed within the growth target.| None         |
| 9   | interaction | Display the flower icon at the top if the stem exceeds the target when clicked     | major  | The flower icon indicates the plant exceeded the growth target.                     | None         |

## Justification

The plant growth tracker works exactly as expected for visualizing plant growth with target indicators. Five vertical stems display representing Basil, Mint, Sage, Thyme, Parsley with realistic sample heights in centimeters. Initial growth data loads with varied stem heights showing at least one plant meeting and at least one plant exceeding the 15 cm target. Stems with 15 or fewer cm display in green color while stems above 15 cm display in yellow color. When users click any stem, that stem displays a sprout icon at the top if it stayed within the target or a flower icon if it exceeds the target.
