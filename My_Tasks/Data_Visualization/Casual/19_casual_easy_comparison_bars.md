Category: Data_Visualization

Prompt style: Casual

Title: Side-by-Side Product Comparison

Prompt: Need a comparison chart showing Product A (Quality 8/10, Price 6/10) and Product B (Quality 7/10, Price 9/10) side-by-side. Show each rating as a horizontal bar, with bars sized to match their ratings. Below each product, show the average calculated from its two ratings. Make Product A bars blue, Product B bars orange. When I click any bar, highlight that product in bold.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display "Product A" and "Product B" labels            | major  | Users need to know which product they're looking at to make meaningful comparisons.                              | None         |
| 2   | content     | Display "Quality 8/10" for Product A                  | major  | Specific rating values help users compare the actual scores between products.                                    | None         |
| 3   | content     | Display "Price 6/10" for Product A                    | major  | Specific rating values help users compare the actual scores between products.                                    | None         |
| 4   | content     | Display "Quality 7/10" for Product B                  | major  | Specific rating values help users compare the actual scores between products.                                    | None         |
| 5   | content     | Display "Price 9/10" for Product B                    | major  | Specific rating values help users compare the actual scores between products.                                    | None         |
| 6   | state       | Calculate average from Product A's two ratings        | major  | The average calculation summarizes Product A's overall performance.                                              | None         |
| 7   | state       | Calculate average from Product B's two ratings        | major  | The average calculation summarizes Product B's overall performance.                                              | None         |
| 8   | content     | Display average below Product A                       | major  | Showing the average helps users quickly compare overall product quality.                                         | None         |
| 9   | content     | Display average below Product B                       | major  | Showing the average helps users quickly compare overall product quality.                                         | None         |
| 10  | visual      | Color Product A bars blue                             | minor  | Blue color helps users quickly identify Product A's bars.                                                        | None         |
| 11  | visual      | Color Product B bars orange                           | minor  | Orange color helps users quickly identify Product B's bars.                                                      | None         |
| 12  | interaction | Highlight clicked product in bold                     | major  | Bold highlighting shows users which product they selected.                                                       | None         |
| 13  | layout      | Position products side-by-side                        | minor  | Side-by-side positioning makes it easy to compare bars horizontally.                                             | None         |

## Justification

The side-by-side product comparison works exactly as expected with interactive selection and calculated averages. "Product A" and "Product B" display side-by-side. Product A shows Quality 8/10 and Price 6/10 with an average calculated from the two ratings displayed below. Product B shows Quality 7/10 and Price 9/10 with its calculated average below. Each rating appears as a horizontal bar sized to match its rating. Product A bars are blue while Product B bars are orange. When users click any bar, that product highlights in bold.
