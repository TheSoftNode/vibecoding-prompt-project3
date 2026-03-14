Category: Data_Visualization

Prompt style: Feature List

Title: Inventory Distribution Bubble Chart

Prompt: Create an inventory bubble chart plotting products by stock level (x-axis) and sales velocity (y-axis). Each bubble's area represents product value. Color bubbles by risk level based on stock-to-velocity ratio - red for critical, yellow for warning, green for healthy. Display product names inside bubbles. When clicking a bubble, highlight it and show a detail panel with name, stock, velocity, value, ratio in months, and risk category. Position bubbles without overlaps. Preload with sample product inventory data.

Required libraries: react, tailwindcss, lucide-react, recharts

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                 | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 10 bubbles for products A through J                      | major  | The ten bubbles establish the foundation for comparing inventory distribution across all products.        | None         |
| 2   | layout      | Position bubbles on x-axis by stock level (0-500 scale)          | major  | X-axis positioning by stock shows which products have high vs low inventory quantities.                   | C1           |
| 3   | layout      | Position bubbles on y-axis by velocity (0-100 scale)             | major  | Y-axis positioning by velocity reveals which products sell quickly vs slowly.                             | C1           |
| 4   | state       | Calculate bubble area proportional to dollar value               | major  | Area-based sizing (not diameter) ensures visual comparison matches value ratios accurately.               | None         |
| 5   | content     | Display product name inside each bubble                          | minor  | Names help users identify which bubble represents each product.                                           | None         |
| 6   | state       | Calculate stock-to-velocity ratio as stock divided by velocity   | major  | The ratio reveals how many months of inventory remain at current sales rates.                             | None         |
| 7   | visual      | Color bubbles red when ratio is less than 2 months               | major  | Red coloring alerts users to critically low inventory that may run out soon.                              | C6           |
| 8   | visual      | Color bubbles yellow when ratio is 2-4 months                    | major  | Yellow indicates moderate inventory levels that need monitoring.                                          | C6           |
| 9   | visual      | Color bubbles green when ratio is above 4 months                 | major  | Green signals healthy inventory levels with ample stock cushion.                                          | C6           |
| 10  | layout      | Position bubbles with no overlaps                                | major  | Non-overlapping bubbles ensure all products remain visible and identifiable.                              | C2, C3, C4   |
| 11  | interaction | Highlight clicked bubble with thick border                       | minor  | Thick border provides clear visual feedback about which bubble the user selected.                         | None         |
| 12  | content     | Display detail panel to the right when bubble clicked            | minor  | Right-side placement keeps details visible without covering the main chart.                               | C11          |
| 13  | content     | Show product name, stock, velocity, value in detail panel        | major  | Displaying all raw values gives users complete product information.                                       | C12          |
| 14  | state       | Calculate and display ratio in months with one decimal place     | major  | The precise ratio helps users make informed inventory reordering decisions.                               | C6           |
| 15  | content     | Display risk category (Critical/Warning/Healthy) in detail panel | major  | The risk category provides actionable guidance for inventory management.                                  | C7, C8, C9   |
| 16  | layout      | Position detail panel to the right of chart                      | minor  | Right positioning follows standard dashboard conventions for supplementary panels.                        | C12          |

## Justification

The Inventory Distribution Bubble Chart achieved 56% pass rate (9/16 criteria) with failures in sizing calculations and overlap prevention. The chart correctly displays 10 bubbles for Widgets A through J (C1 passed) positioned accurately on the x-axis by stock level (C2 passed) and y-axis by velocity (C3 passed), creating a scatter plot layout. However, the bubble sizing completely failed C4 - instead of making area proportional to dollar value, the model made diameter proportional, causing Widget E ($30K) to appear 4× larger in area than it should compared to Widget G ($5K) rather than 6× larger. Product names displayed inside bubbles (C5 passed). The stock-to-velocity ratio calculation worked correctly (C6 passed), computing months of inventory remaining. The color coding worked perfectly: Widget E (50÷90 = 0.56 months) appeared red for critical (C7 passed), Widget A (250÷60 = 4.17 months) appeared yellow for warning, and Widget G (480÷20 = 24 months) appeared green for healthy (C8, C9 passed). However, bubble positioning failed C10 catastrophically - Widgets C and E overlapped significantly (both having low stock levels around 50-100 units), making their names unreadable. Click interactions worked: clicking a bubble highlighted it with a thick border (C11 passed) and displayed a detail panel (C12 passed) showing name, stock, velocity, and value (C13 passed). The ratio displayed correctly as "Stock-to-Velocity: 4.2 months" with one decimal place (C14 passed) and the risk category showed appropriately as "Critical", "Warning", or "Healthy" (C15 passed). The detail panel positioned correctly on the right side of the chart (C16 passed). The area vs diameter calculation error (C4) and bubble overlap issue (C10) were the primary failures preventing higher scores.
