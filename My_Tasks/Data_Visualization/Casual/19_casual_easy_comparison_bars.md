Category: Data_Visualization

Prompt style: Casual

Title: Side-by-Side Product Comparison

Prompt: Show me a comparison chart for two products. Put "Product A" on the left and "Product B" on the right. For each product, display 3 horizontal bars showing ratings: "Quality 8/10", "Price 6/10", "Support 9/10". Make each bar's length match its rating number out of 10. Color Product A bars blue and Product B bars orange. When someone clicks on any bar, highlight that entire product's column in a light background color and show which product was selected with text at the bottom saying "Selected: Product A" or "Selected: Product B".

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display "Product A" label on left                     | major  | The label identifies the first product being compared.                                                           | None         |
| 2   | content     | Display "Product B" label on right                    | major  | The label identifies the second product being compared.                                                          | None         |
| 3   | content     | Display "Quality 8/10" bar for Product A              | major  | The rating shows Product A's quality score.                                                                      | None         |
| 4   | content     | Display "Price 6/10" bar for Product A                | major  | The rating shows Product A's price score.                                                                        | None         |
| 5   | content     | Display "Support 9/10" bar for Product A              | major  | The rating shows Product A's support score.                                                                      | None         |
| 6   | content     | Display "Quality 8/10" bar for Product B              | major  | The rating shows Product B's quality score.                                                                      | None         |
| 7   | content     | Display "Price 6/10" bar for Product B                | major  | The rating shows Product B's price score.                                                                        | None         |
| 8   | content     | Display "Support 9/10" bar for Product B              | major  | The rating shows Product B's support score.                                                                      | None         |
| 9   | state       | Scale bar length to match rating value out of 10     | major  | Proportional lengths let users visually compare ratings.                                                         | None         |
| 10  | visual      | Color Product A bars blue                             | minor  | Blue color distinguishes Product A's bars.                                                                       | None         |
| 11  | visual      | Color Product B bars orange                           | minor  | Orange color distinguishes Product B's bars.                                                                     | None         |
| 12  | interaction | Highlight product column when bar is clicked          | major  | Clicking a bar highlights the entire product to show selection.                                                  | None         |
| 13  | interaction | Display "Selected: Product A" or "Selected: Product B" text | major  | The selection text confirms which product the user clicked.                                                      | C12          |
| 14  | layout      | Position Product A on left side                       | minor  | Left positioning creates the side-by-side comparison layout.                                                     | None         |
| 15  | layout      | Position Product B on right side                      | minor  | Right positioning completes the side-by-side comparison layout.                                                  | None         |

## Justification

The side-by-side product comparison works exactly as expected with interactive selection feedback. "Product A" displays on the left and "Product B" on the right. Each product shows 3 horizontal bars: "Quality 8/10", "Price 6/10", and "Support 9/10", with bar lengths proportional to the rating values out of 10. Product A bars are colored blue while Product B bars are orange. When users click on any bar, that entire product's column highlights with a light background color, and text at the bottom displays "Selected: Product A" or "Selected: Product B" to confirm the selection.
