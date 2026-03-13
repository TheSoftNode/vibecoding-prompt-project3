Category: Quick_Tools

Prompt style: Conversational

Title: Recipe Ingredient Scaler

Prompt: I need a recipe scaler for adjusting ingredient amounts. Start with three ingredients: "Flour 2 cups", "Sugar 1 cup", and "Butter 0.5 cups". Below them, show the total cups calculated by adding all ingredients together, like "Total: 3.5 cups" in bold text. Above the ingredients, show three scale buttons: "Half (0.5x)", "Double (2x)", and "Triple (3x)". When I click a button, update all ingredient amounts to that scale. The total should always reflect the sum of the current ingredient amounts.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                       | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | ------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display "Flour 2 cups" ingredient initially          | major  | Showing the ingredient name and amount lets users see what they're scaling.     | None         |
| 2   | content     | Display "Sugar 1 cup" ingredient initially           | major  | Showing the ingredient name and amount lets users see what they're scaling.     | None         |
| 3   | content     | Display "Butter 0.5 cups" ingredient initially       | major  | Showing the ingredient name and amount lets users see what they're scaling.     | None         |
| 4   | content     | Display "Half (0.5x)" button                         | major  | The button gives users the control to scale down the recipe.                    | None         |
| 5   | content     | Display "Double (2x)" button                         | major  | The button gives users the control to scale up the recipe.                      | None         |
| 6   | content     | Display "Triple (3x)" button                         | major  | The button gives users the control to scale up the recipe further.              | None         |
| 7   | content     | Display "Total: 3.5 cups" initially                  | major  | Showing the total tells users how much the recipe makes in total.               | None         |
| 8   | visual      | Display total in bold text                           | minor  | Bold styling emphasizes the total as the key summary value.                     | None         |
| 9   | state       | Calculate total cups by adding all ingredients       | major  | The total calculation sums all ingredient amounts to show combined quantity.    | None         |
| 10  | interaction | Update all ingredient amounts when button is clicked | major  | Updated amounts show users the new quantities they need for the scaled recipe.  | None         |
| 11  | interaction | Update total display when button is clicked          | major  | The updated total reflects the sum of the new scaled amounts.                   | C9, C10      |
| 12  | layout      | Position scale buttons above ingredients             | minor  | Placing controls above the ingredient list creates clear top-down workflow.     | None         |
| 13  | layout      | Position total display below ingredients             | minor  | Placing the total below shows it as the result of adding the ingredients above. | None         |

## Justification

The Recipe Ingredient Scaler achieved 92.31% pass rate with one text formatting issue. Three ingredients display with their amounts: Flour 2 cups, Sugar, and Butter 0.5 cups. However, the model failed C2 by displaying "Sugar 1 cups" instead of "Sugar 1 cup" as specified in the prompt Below the ingredients, "Total: 3.5 cups" shows in bold text, correctly calculated by adding all ingredients together. Above the ingredients, three scale buttons appear: "Half (0.5x)", "Double (2x)", and "Triple (3x)". When users click a button, all ingredient amounts update to that scale, and the total always reflects the sum of the current ingredient amounts.
