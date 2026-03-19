Category: Data_Visualization

Prompt style: Casual

Title: Temperature Gauge Strip

Prompt: Need a temperature gauge showing 5 cities displayed as vertical thermometer strips. Show New York at 72°F, London at 55°F, Tokyo at 68°F, Sydney at 81°F, and Dubai at 95°F. Each thermometer fills from bottom to top based on temperature with red color for hot (above 80°F), orange for warm (60-80°F), and blue for cool (below 60°F). Display city name below each thermometer and temperature value at the top. When I click any thermometer, show that city's name in bold at the bottom of the screen.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display 5 vertical thermometer strips                | major  | The thermometer strips provide the visual structure for temperature display.   | None         |
| 2   | content     | Display city names: New York, London, Tokyo, Sydney, Dubai | minor  | City names identify which location each thermometer represents.                | None         |
| 3   | layout      | Position city names below thermometers               | minor  | Bottom positioning associates each name with its thermometer.                  | C2           |
| 4   | content     | Display temperatures: 72°F, 55°F, 68°F, 81°F, 95°F   | major  | Temperature values show the exact readings for each city.                      | None         |
| 5   | layout      | Position temperature values at top of thermometers   | minor  | Top positioning shows the numeric value above the visual gauge.                | C4           |
| 6   | state       | Fill thermometer from bottom to top based on temperature | major  | Fill level visually represents the temperature amount.                       | None         |
| 7   | visual      | Color hot thermometers (above 80°F) red              | major  | Red color indicates hot temperatures for Sydney and Dubai.                     | None         |
| 8   | visual      | Color warm thermometers (60-80°F) orange             | major  | Orange color indicates warm temperatures for New York and Tokyo.               | None         |
| 9   | visual      | Color cool thermometers (below 60°F) blue            | major  | Blue color indicates cool temperatures for London.                             | None         |
| 10  | interaction | Show city name in bold at bottom when clicked        | major  | Bold text shows which city thermometer users selected.                         | None         |
| 11  | layout      | Position clicked city name at bottom of screen       | minor  | Bottom placement separates the selection feedback from the gauges.             | C10          |

## Justification

The temperature gauge strip works exactly as expected for visualizing city temperatures with color-coded thermometers. Five vertical thermometer strips display with city names "New York", "London", "Tokyo", "Sydney", and "Dubai" positioned below each thermometer. Temperature values "72°F", "55°F", "68°F", "81°F", and "95°F" display at the top of each thermometer. Each thermometer fills from bottom to top based on its temperature value. Sydney and Dubai thermometers display in red color (above 80°F), New York and Tokyo thermometers display in orange color (60-80°F), and London thermometer displays in blue color (below 60°F). When users click any thermometer, that city's name displays in bold text at the bottom of the screen.
