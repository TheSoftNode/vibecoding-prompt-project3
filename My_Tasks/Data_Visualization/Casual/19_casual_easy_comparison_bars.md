Category: Data_Visualization

Prompt style: Casual

Title: Side-by-Side Product Comparison

Prompt: Build a side-by-side product comparison chart with two columns labeled "Product A" and "Product B". Each column displays 3 horizontal rating bars: Quality (8/10), Price (6/10), Support (9/10), with each bar's width calculated as a percentage of its rating value out of 10. Color all Product A bars blue, Product B bars orange. Clicking any bar highlights its entire product column and displays "Selected: [product name]" text below.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display "Product A" and "Product B" labels            | major  | Users need to know which product they're looking at to make meaningful comparisons.                              | None         |
| 2   | content     | Display "Quality (8/10)" rating for both products     | major  | Specific rating values help users compare the actual scores between products.                                    | None         |
| 3   | content     | Display "Price (6/10)" rating for both products       | major  | Specific rating values help users compare the actual scores between products.                                    | None         |
| 4   | content     | Display "Support (9/10)" rating for both products     | major  | Specific rating values help users compare the actual scores between products.                                    | None         |
| 5   | state       | Calculate bar width as percentage of rating value     | major  | The bars need proportional sizing so users can quickly see which ratings are higher or lower at a glance.        | None         |
| 6   | visual      | Color all Product A bars blue                         | minor  | Different colors help users quickly distinguish which bars belong to which product.                              | None         |
| 7   | visual      | Color all Product B bars orange                       | minor  | Different colors help users quickly distinguish which bars belong to which product.                              | None         |
| 8   | interaction | Highlight product column when bar is clicked          | major  | The visual feedback shows users which product they've selected for comparison.                                   | None         |
| 9   | interaction | Display "Selected: [product name]" text below when bar is clicked | major  | The text confirmation ensures users know exactly which product is currently selected.                            | C8           |
| 10  | layout      | Position products side-by-side as columns             | minor  | Side-by-side positioning makes it easy to compare bars across the two products horizontally.                     | None         |

## Justification

The side-by-side product comparison works exactly as expected with interactive selection feedback. "Product A" displays on the left and "Product B" on the right. Each product shows 3 horizontal bars: "Quality 8/10", "Price 6/10", and "Support 9/10", with bar lengths proportional to the rating values out of 10. Product A bars are colored blue while Product B bars are orange. When users click on any bar, that entire product's column highlights with a light background color, and text at the bottom displays "Selected: Product A" or "Selected: Product B" to confirm the selection.
