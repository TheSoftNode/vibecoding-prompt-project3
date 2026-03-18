Category: Data_Visualization

Prompt style: Conversational

Title: Device Battery Monitor

Prompt: I need a battery level monitor for multiple devices. Display 4 horizontal battery bars stacked vertically showing: Phone at 85%, Tablet at 45%, Laptop at 20%, Watch at 95%. Each battery shows its device name on the left and percentage on the right. Fill the battery bar to match its percentage. Color batteries green above 60%, yellow between 30-60%, and red below 30%. When I click any battery bar, highlight it with a border to show it's selected.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 4 horizontal battery bars stacked vertically| major  | The battery bars provide the visualization for device charge levels.                         | None         |
| 2   | content     | Display device labels: Phone, Tablet, Laptop, Watch  | minor  | The labels identify which device each battery represents.                                    | None         |
| 3   | layout      | Position device name left of battery bar             | minor  | Left positioning clearly associates the label with its battery.                              | C2           |
| 4   | content     | Display percentages: 85%, 45%, 20%, 95%              | major  | The percentages show exact charge levels for all devices.                                    | None         |
| 5   | layout      | Position percentage right of battery bar             | minor  | Right positioning shows the numeric value alongside the visual bar.                          | C4           |
| 6   | state       | Fill battery bar to match percentage                 | major  | Fill level visually represents the charge amount.                                            | None         |
| 7   | state       | Determine color based on battery percentage          | major  | Color calculation categorizes charge levels as healthy, moderate, or critical.               | None         |
| 8   | visual      | Color battery green if above 60%                     | major  | Green indicates healthy charge levels.                                                       | C7           |
| 9   | visual      | Color battery yellow if between 30-60%               | major  | Yellow warns of moderate charge levels.                                                      | C7           |
| 10  | visual      | Color battery red if below 30%                       | major  | Red warns of critically low charge levels.                                                   | C7           |
| 11  | interaction | Highlight battery bar with border when clicked       | major  | Clicking a battery bar selects it to show which device users are focusing on.                | None         |

## Justification

The device battery monitor works exactly as expected for visualizing charge levels with color coding. Four horizontal battery bars display stacked vertically with device labels "Phone", "Tablet", "Laptop", and "Watch" positioned on the left of each bar and percentages "85%", "45%", "20%", and "95%" positioned on the right. Each battery bar fills to match its percentage value. The Phone at 85% and Watch at 95% color green (above 60%). The Tablet at 45% colors yellow (between 30-60%). The Laptop at 20% colors red (below 30%). When users click any battery bar, it highlights with a border showing it's selected.
