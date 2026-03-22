Category: Data_Visualization

Prompt style: Conversational

Title: Donut Chart Splitter

Prompt: Need a donut chart with three segments showing budget categories. Click segment to split it outward from center. Show category label and amount below chart.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                      | Weight | Rationale                                                                  | Dependent On |
| --- | ----------- | ------------------------------------------------ | ------ | -------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display donut chart                              | major  | Donut chart provides the circular visualization structure.                 | None         |
| 2   | visual      | Display three segments in donut chart            | major  | Three segments show different budget categories.                           | C1           |
| 3   | content     | Load budget category data                        | major  | Category data provides the values to visualize.                            | None         |
| 4   | interaction | Detect segment click                             | major  | Click detection triggers split animation.                                  | None         |
| 5   | visual      | Split clicked segment outward from center        | major  | Outward split highlights the selected segment.                             | C4           |
| 6   | content     | Display category label for clicked segment       | major  | Category label tells users which budget category is selected.              | C4           |
| 7   | content     | Display amount for clicked segment               | major  | Amount shows the budget value for the selected category.                   | C4           |
| 8   | layout      | Position label and amount below chart            | major  | Below positioning keeps information visible without blocking the chart.    | C6, C7       |

## Justification

The donut chart splitter works as expected for interactive budget visualization. A donut chart displays with three segments showing budget categories loaded from category data. When users click a segment, that segment splits outward from the center highlighting it. The system displays the category label and amount for the clicked segment positioned below the chart showing which budget category is selected and its value.
