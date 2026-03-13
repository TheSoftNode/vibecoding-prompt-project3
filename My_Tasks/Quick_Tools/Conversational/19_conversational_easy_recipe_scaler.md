Category: Quick_Tools

Prompt style: Conversational

Title: Recipe Ingredient Scaler

Prompt: I need a recipe scaler for adjusting ingredient amounts. Start with three ingredients already filled in: "Flour 2 cups", "Sugar 1 cup", and "Butter 0.5 cups". Above them, show four preset scale buttons in a row: "Half (0.5x)" in light gray, "Normal (1x)" in blue, "Double (2x)" in light gray, and "Triple (3x)" in light gray. When I click any scale button, all the ingredient amounts should adjust to match that scale. Highlight the clicked button in blue while changing the others back to light gray.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display "Flour 2 cups" ingredient initially           | major  | Showing the ingredient name and amount lets users see what they're scaling.                                      | None         |
| 2   | content     | Display "Sugar 1 cup" ingredient initially            | major  | Showing the ingredient name and amount lets users see what they're scaling.                                      | None         |
| 3   | content     | Display "Butter 0.5 cups" ingredient initially        | major  | Showing the ingredient name and amount lets users see what they're scaling.                                      | None         |
| 4   | content     | Display "Half (0.5x)" button                          | major  | The button gives users the control to scale down the recipe.                                                     | None         |
| 5   | content     | Display "Normal (1x)" button                          | major  | The button gives users the control to return to original amounts.                                                | None         |
| 6   | content     | Display "Double (2x)" button                          | major  | The button gives users the control to scale up the recipe.                                                       | None         |
| 7   | content     | Display "Triple (3x)" button                          | major  | The button gives users the control to scale up the recipe further.                                               | None         |
| 8   | visual      | Display "Normal (1x)" button in blue initially        | minor  | Blue color shows users the recipe is at its original scale.                                                      | C5           |
| 9   | visual      | Display "Half (0.5x)" button in light gray initially  | minor  | Gray color shows this scale option is not currently selected.                                                    | C4           |
| 10  | visual      | Display "Double (2x)" button in light gray initially  | minor  | Gray color shows this scale option is not currently selected.                                                    | C6           |
| 11  | visual      | Display "Triple (3x)" button in light gray initially  | minor  | Gray color shows this scale option is not currently selected.                                                    | C7           |
| 12  | state       | Adjust ingredient amounts to match scale when button clicked | major  | The adjusted amounts reflect the selected scale size for the recipe.                                             | C1, C2, C3   |
| 13  | interaction | Update all ingredient displays when button is clicked | major  | Updated displays show users the new quantities they need for the scaled recipe.                                  | C12          |
| 14  | interaction | Highlight clicked button in blue when clicked         | major  | Blue highlighting confirms which scale the user just selected.                                                   | C4, C5, C6, C7 |
| 15  | interaction | Change other buttons to light gray when button clicked | major  | Gray color on unselected buttons clarifies which scale is active.                                                | C14          |
| 16  | layout      | Position buttons in a row above ingredients           | minor  | Placing controls above the ingredient list creates clear top-down workflow.                                      | None         |

## Justification

The Recipe Ingredient Scaler works exactly as expected with preset scale buttons. Three ingredients are already filled in: "Flour 2 cups", "Sugar 1 cup", and "Butter 0.5 cups". Above them, four preset scale buttons appear in a row: "Half (0.5x)" in light gray, "Normal (1x)" in blue, "Double (2x)" in light gray, and "Triple (3x)" in light gray. When users click any button, all the ingredient amounts adjust to match that scale. The clicked button highlights in blue while the others change back to light gray.
