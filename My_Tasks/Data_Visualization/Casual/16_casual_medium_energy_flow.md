Category: Data_Visualization

Prompt style: Casual

Title: Energy Flow Sankey Diagram

Prompt: Need an energy flow diagram showing how power gets from three sources (Solar, Wind, Coal) to four consumption zones (Residential, Industrial, Commercial, Public). Show the flows as curved connecting bands where each band's width matches the energy amount going through it, with animated particles flowing along the curves to show direction. Sources on the left, zones on the right. Draw thin dotted connector lines from each flow band to a legend positioned directly below the diagram showing flow percentages. When I click a flow band, highlight it with a pulsing animation and show me the source, destination, flow amount, and whether it's high-efficiency (flow above 15% of total), medium-efficiency (8-15%), or low-efficiency (below 8%). Flows smaller than 3% should get grouped as "Other" to keep it clean. Start with some realistic sample data on load.

Required libraries: react, tailwindcss, lucide-react, recharts

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                 | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display three source nodes on left side                          | major  | The three sources provide the foundation for understanding where energy originates.                       | None         |
| 2   | visual      | Display four zone nodes on right side                            | major  | The four zones show where energy is consumed, completing the flow visualization.                          | None         |
| 3   | visual      | Draw curved paths between sources and zones                      | major  | Curved paths distinguish Sankey diagrams from simple bar charts and improve visual clarity.               | None         |
| 4   | visual      | Animate particles flowing along curved band paths                | major  | Animated particles provide dynamic visual feedback showing energy flow direction.                         | C3           |
| 5   | state       | Calculate band thickness proportional to flow percentage         | major  | Proportional thickness allows users to compare flow volumes visually at a glance.                         | None         |
| 6   | visual      | Draw thin dotted connector lines from bands to legend            | major  | Connector lines link flow bands to their legend entries, creating visual correspondence.                  | C3           |
| 7   | layout      | Position legend directly below the diagram                       | major  | Below positioning keeps the legend separate from the main flow visualization.                             | None         |
| 8   | content     | Display flow percentages in legend                               | minor  | Legend percentages provide precise values for each flow.                                                  | None         |
| 9   | state       | Group flows below 3% into single "Other" band                    | major  | Grouping minor flows reduces visual clutter while maintaining data completeness.                          | C5           |
| 10  | interaction | Highlight clicked flow band with pulsing animation               | major  | Pulsing animation provides strong visual feedback about which flow path the user selected.                | None         |
| 11  | content     | Display detail card with source, destination, and flow amount    | major  | The detail card gives users precise information about the specific flow they clicked.                     | C10          |
| 12  | state       | Calculate efficiency rating based on flow percentage thresholds  | major  | Efficiency ratings help users identify high-impact vs low-impact energy paths quickly.                    | C5           |
| 13  | content     | Show efficiency as "high-efficiency", "medium-efficiency", or "low-efficiency" in detail card | major  | The three-tier efficiency system provides actionable categorization of flow importance.                   | C12          |

## Justification

The Energy Flow Sankey Diagram achieved 46% pass rate (6/13 criteria) with cascading failures from complex visualization requirements. The diagram correctly displays three source nodes on the left and four zone nodes on the right (C1, C2 passed). However, the model failed C3 by drawing straight diagonal lines instead of curved paths, which caused C4 to fail automatically - without curved paths, the animated particles couldn't flow along curves and instead moved in straight lines. The band thickness calculation worked (C5 passed), but C6 failed catastrophically - the model drew no connector lines from flow bands to the legend, breaking the visual correspondence. The legend appeared but was positioned to the right of the diagram instead of directly below it (C7 failed). Flow percentages displayed in the legend (C8 passed). The grouping logic failed C9 - flows below 3% appeared as individual bands instead of being grouped into a single "Other" band. Click interactions partially worked: clicking highlighted the band but failed C10 by showing a simple yellow highlight instead of a pulsing animation. The detail card appeared showing source, destination, and flow amount (C11 passed). However, efficiency ratings failed C12 - the model calculated efficiency but used incorrect thresholds (treating flows above 10% as high-efficiency instead of above 15%). The efficiency labels failed C13 by displaying "High", "Medium", "Low" instead of the specified "high-efficiency", "medium-efficiency", "low-efficiency" format.
