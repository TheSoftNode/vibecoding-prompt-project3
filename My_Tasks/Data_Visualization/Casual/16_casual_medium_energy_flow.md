Category: Data_Visualization

Prompt style: Casual

Title: Energy Flow Sankey Diagram

Prompt: Need an energy flow diagram showing how power gets from three sources (Solar, Wind, Coal) to four consumption zones (Residential, Industrial, Commercial, Public). Show the flows as connecting bands where each band's width matches the energy amount going through it. Sources on the left, zones on the right. When I click a flow band, highlight it and show me the source, destination, flow amount, and efficiency rating. Tiny flows should get grouped as "Other" to keep it clean. Put a summary below showing where the selected source's energy goes. Start with some realistic sample data on load.

Required libraries: react, tailwindcss, lucide-react, recharts

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                 | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display three source nodes on left side                          | major  | The three sources provide the foundation for understanding where energy originates.                       | None         |
| 2   | visual      | Display four zone nodes on right side                            | major  | The four zones show where energy is consumed, completing the flow visualization.                          | None         |
| 3   | visual      | Draw curved paths between sources and zones                      | major  | Curved paths distinguish Sankey diagrams from simple bar charts and improve visual clarity.               | None         |
| 4   | state       | Calculate band thickness proportional to flow percentage         | major  | Proportional thickness allows users to compare flow volumes visually at a glance.                         | None         |
| 5   | content     | Display source percentages (Solar 45%, Wind 30%, Coal 25%)       | minor  | Source percentages help users understand the energy generation mix.                                       | None         |
| 6   | content     | Display zone percentages (Residential 35%, Industrial 40%, Commercial 20%, Public 5%) | minor  | Zone percentages show the distribution of energy consumption.                                             | None         |
| 7   | state       | Group flows below 3% into single "Minor Flows" band              | major  | Grouping minor flows reduces visual clutter while maintaining data completeness.                          | C4           |
| 8   | layout      | Position "Other" destination node at bottom                      | minor  | Bottom positioning for "Other" separates it from primary zones, indicating its special grouped nature.    | C7           |
| 9   | interaction | Highlight clicked flow band in yellow                            | major  | Yellow highlighting provides clear visual feedback about which flow path the user selected.               | None         |
| 10  | content     | Display detail card with source name, destination name, percentage | major  | The detail card gives users precise information about the specific flow they clicked.                     | C9           |
| 11  | state       | Calculate efficiency rating based on flow percentage thresholds  | major  | Efficiency ratings help users identify high-impact vs low-impact energy paths quickly.                    | C4           |
| 12  | content     | Show efficiency as "High" (>15%), "Medium" (8-15%), "Low" (<8%)  | major  | The three-tier efficiency system provides actionable categorization of flow importance.                   | C11          |
| 13  | content     | Display summary panel below diagram                              | minor  | The summary panel location keeps it visible without overlapping the main visualization.                   | None         |
| 14  | state       | Calculate total flows from selected source only                  | major  | Filtering to the selected source helps users analyze one source's distribution pattern in isolation.      | C9           |
| 15  | content     | Show percentage distribution across destinations for selected source | major  | Distribution percentages reveal how each source allocates its energy across consumption zones.            | C14          |
| 16  | content     | Display "Click any flow to see details" when nothing selected    | minor  | The placeholder text guides users on how to interact with the diagram initially.                          | None         |

## Justification

The Energy Flow Sankey Diagram achieved 56% pass rate (9/16 criteria) with failures concentrated in calculations and edge cases. The diagram correctly displays three source nodes on the left (Solar, Wind, Coal) and four zone nodes on the right (Residential, Industrial, Commercial, Public) with their labeled percentages. However, the model failed C3 by drawing straight diagonal lines instead of the curved paths that define Sankey visualizations, making it look more like a basic network diagram. The band thickness was inconsistent (C4 failed) - instead of being proportional to flow percentages, all bands appeared roughly equal width, preventing visual comparison of flow volumes. The model completely ignored C7 and C8, failing to group flows below 3% into a "Minor Flows" band or create an "Other" destination node at the bottom. Click interactions worked partially - clicking a band highlighted it in yellow (C9 passed) and showed a detail card with source, destination, and percentage (C10 passed), but the efficiency rating failed C11 and C12 by always showing "Medium" regardless of the actual flow percentage rather than applying the >15%, 8-15%, <8% thresholds correctly. The summary panel appeared below the diagram (C13 passed) and correctly displayed the placeholder text "Click any flow to see details" initially (C16 passed), but when a band was clicked, it failed C14 and C15 by showing all sources' flow totals instead of filtering to only the selected source and calculating its percentage distribution across destinations.
