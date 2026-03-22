Category: Data_Visualization

Prompt style: Terse

Title: Pulse Bar Tracker

Prompt: Show four bars with different heights. Hover bar to pulse it. Display bar value at top.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                            | Weight | Rationale                                                                 | Dependent On |
| --- | ----------- | -------------------------------------- | ------ | ------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display four bars                      | major  | Four bars provide multiple data points for comparison.                    | None         |
| 2   | visual      | Display bars with different heights    | major  | Different heights visualize varying data values.                          | C1           |
| 3   | interaction | Detect bar hover                       | major  | Hover detection triggers pulse animation.                                 | None         |
| 4   | visual      | Apply pulse animation to hovered bar   | major  | Pulse animation highlights the bar users are inspecting.                  | C3           |
| 5   | content     | Load bar values                        | major  | Bar values provide the data to display.                                   | None         |
| 6   | content     | Display value for hovered bar          | major  | Showing value tells users the exact data amount.                          | C3           |
| 7   | layout      | Position value at top of screen        | minor  | Top positioning keeps value visible without blocking bars.                | C6           |

## Justification

The pulse bar tracker works as expected for interactive bar visualization. Four bars display with different heights representing varying data values. When users hover over a bar, that bar applies a pulse animation highlighting it. The system displays the hovered bar's value at the top of the screen showing the exact data amount for the inspected bar.
