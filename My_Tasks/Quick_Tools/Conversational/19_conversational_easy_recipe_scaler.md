Category: Quick_Tools

Prompt style: Conversational

Title: Recipe Ingredient Scaler

Prompt: I need a recipe scaler that helps me adjust ingredient amounts. Show three preset ingredients: "Flour 2 cups", "Sugar 1 cup", and "Butter 0.5 cups". Above the ingredients, display a multiplier slider ranging from 0.5x to 3x, starting at 1x. As I drag the slider, recalculate and update all three ingredient amounts in real-time based on the multiplier. Display the current multiplier value next to the slider as "Scale: Xx" where X is the current multiplier.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display "Flour 2 cups" ingredient initially           | major  | Preset ingredients give users immediate example data to work with.                                               | None         |
| 2   | content     | Display "Sugar 1 cup" ingredient initially            | major  | Preset ingredients give users immediate example data to work with.                                               | None         |
| 3   | content     | Display "Butter 0.5 cups" ingredient initially        | major  | Preset ingredients give users immediate example data to work with.                                               | None         |
| 4   | visual      | Display multiplier slider above ingredients           | major  | The slider provides the control mechanism for scaling all ingredients.                                           | None         |
| 5   | state       | Set slider range from 0.5x to 3x                      | major  | The range allows both reducing and increasing recipe amounts within practical cooking limits.                    | None         |
| 6   | state       | Set slider initial value to 1x                        | minor  | Starting at 1x shows the original recipe before any scaling.                                                     | None         |
| 7   | content     | Display "Scale: 1x" text next to slider initially     | major  | The label shows users the exact multiplier being applied.                                                        | None         |
| 8   | state       | Recalculate Flour amount when slider moves            | major  | Real-time calculation lets users see how scaling affects each ingredient immediately.                            | C5           |
| 9   | state       | Recalculate Sugar amount when slider moves            | major  | Real-time calculation lets users see how scaling affects each ingredient immediately.                            | C5           |
| 10  | state       | Recalculate Butter amount when slider moves           | major  | Real-time calculation lets users see how scaling affects each ingredient immediately.                            | C5           |
| 11  | interaction | Update Flour display when slider moves                | major  | Showing updated amounts helps users understand the scaled recipe quantities.                                     | C8           |
| 12  | interaction | Update Sugar display when slider moves                | major  | Showing updated amounts helps users understand the scaled recipe quantities.                                     | C9           |
| 13  | interaction | Update Butter display when slider moves               | major  | Showing updated amounts helps users understand the scaled recipe quantities.                                     | C10          |
| 14  | interaction | Update "Scale: Xx" text when slider moves             | major  | The changing multiplier value confirms which scale factor is currently applied.                                  | None         |
| 15  | layout      | Position slider above ingredients list                | minor  | Placing the control above the results creates clear top-to-bottom flow.                                          | None         |

## Justification

The Recipe Ingredient Scaler works exactly as expected with real-time ingredient scaling. Three preset ingredients display: "Flour 2 cups", "Sugar 1 cup", and "Butter 0.5 cups". Above the ingredients, a multiplier slider appears ranging from 0.5x to 3x, initialized at 1x. Next to the slider, "Scale: 1x" displays the current multiplier value. As users drag the slider, all three ingredient amounts recalculate and update in real-time based on the multiplier. The "Scale: Xx" text updates to show the current multiplier as the slider moves.
