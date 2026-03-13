Category: Data_Visualization

Prompt style: Terse

Title: Energy Flow Sankey

Prompt: Sankey diagram showing energy flow. 3 sources on left: "Coal 40", "Wind 35", "Solar 25". 2 destinations on right: "Homes 60", "Industry 40". Show 6 colored flow bands connecting sources to destinations, with band width proportional to flow amount: Coal→Homes 30, Coal→Industry 10, Wind→Homes 25, Wind→Industry 10, Solar→Homes 5, Solar→Industry 20. Hovering over any flow band displays its exact value.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display "Coal 40" source label on left                | major  | The label shows the energy source name and total value.                                                          | None         |
| 2   | content     | Display "Wind 35" source label on left                | major  | The label shows the energy source name and total value.                                                          | None         |
| 3   | content     | Display "Solar 25" source label on left               | major  | The label shows the energy source name and total value.                                                          | None         |
| 4   | content     | Display "Homes 60" destination label on right         | major  | The label shows the destination name and total value received.                                                   | None         |
| 5   | content     | Display "Industry 40" destination label on right      | major  | The label shows the destination name and total value received.                                                   | None         |
| 6   | visual      | Display colored flow bands connecting sources to destinations | major | Flow bands visualize the energy distribution paths.                                                              | None         |
| 7   | state       | Calculate band width proportional to flow value       | major  | Proportional widths show relative flow amounts visually.                                                         | None         |
| 8   | visual      | Display Coal to Homes flow band with width 30         | major  | The band width represents 30 units flowing from coal to homes.                                                   | None         |
| 9   | visual      | Display Coal to Industry flow band with width 10      | minor  | The band width represents 10 units flowing from coal to industry.                                                | None         |
| 10  | visual      | Display Wind to Homes flow band with width 25         | major  | The band width represents 25 units flowing from wind to homes.                                                   | None         |
| 11  | visual      | Display Wind to Industry flow band with width 10      | minor  | The band width represents 10 units flowing from wind to industry.                                                | None         |
| 12  | visual      | Display Solar to Homes flow band with width 5         | minor  | The band width represents 5 units flowing from solar to homes.                                                   | None         |
| 13  | visual      | Display Solar to Industry flow band with width 20     | major  | The band width represents 20 units flowing from solar to industry.                                               | None         |
| 14  | interaction | Display exact value when hovering over flow band      | minor  | Hovering shows the precise flow amount for detailed inspection.                                                  | None         |
| 15  | layout      | Position sources on left side                         | minor  | Left positioning creates the standard left-to-right flow direction.                                              | None         |
| 16  | layout      | Position destinations on right side                   | minor  | Right positioning completes the left-to-right flow visualization.                                                | None         |

## Justification

The energy flow Sankey diagram works exactly as expected with proportional flow visualization and hover tooltips. Three source labels "Coal 40", "Wind 35", and "Solar 25" display on the left side. Two destination labels "Homes 60" and "Industry 40" display on the right side. Colored flow bands connect sources to destinations, with band widths proportional to the flow values. Coal splits into a 30-width band flowing to Homes and a 10-width band to Industry. Wind splits into a 25-width band to Homes and a 10-width band to Industry. Solar splits into a 5-width band to Homes and a 20-width band to Industry. Hovering over any flow band displays its exact value. The proportional widths visually communicate the energy distribution across sources and destinations.
