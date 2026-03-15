Category: Data_Visualization

Prompt style: Casual

Title: Energy Flow Sankey Diagram

Prompt: Need an energy flow diagram showing how power gets from three sources (Solar, Wind, Coal) to four consumption zones (Residential, Industrial, Commercial, Public). Show the flows as curved connecting bands where each band's width matches the energy amount going through it, with animated particles flowing along the curves to show direction. Sources on the left, zones on the right. Draw thin dotted connector lines from each flow band to a legend positioned directly below the diagram showing flow percentages. When I click a flow band, highlight it with a pulsing animation and show me the source, destination, flow amount, and whether it's high-efficiency (flow above 15% of total), medium-efficiency (8-15%), or low-efficiency (below 8%). Flows smaller than 3% should get grouped as "Other" to keep it clean. Start with some realistic sample data on load.

Required libraries: react, tailwindcss, lucide-react, recharts

## Rubric

| #   | ID          | Description                                                                                   | Weight | Rationale                                                                                                   | Dependent On |
| --- | ----------- | --------------------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display three source nodes on left side                                                       | major  | The three sources provide the foundation for understanding where energy originates.                         | None         |
| 2   | visual      | Display four zone nodes on right side                                                         | major  | The four zones show where energy is consumed, completing the flow visualization.                            | None         |
| 3   | visual      | Draw curved paths between sources and zones                                                   | major  | Curved paths distinguish Sankey diagrams from simple bar charts and improve visual clarity.                 | None         |
| 4   | visual      | Animate particles flowing along curved band paths                                             | major  | Animated particles provide dynamic visual feedback showing energy flow direction.                           | C3           |
| 5   | state       | Calculate band thickness proportional to flow percentage                                      | major  | Proportional thickness allows users to compare flow volumes visually at a glance.                           | None         |
| 6   | visual      | Draw thin dotted connector lines from bands to legend                                         | major  | Connector lines link flow bands to their legend entries, creating visual correspondence.                    | C3           |
| 7   | layout      | Position legend directly below the diagram                                                    | major  | Below positioning keeps the legend separate from the main flow visualization.                               | None         |
| 8   | content     | Display flow percentages in legend                                                            | minor  | Legend percentages provide precise values for each flow.                                                    | None         |
| 9   | state       | Group flows below 3% into single "Other" band                                                 | major  | Grouping minor flows reduces visual clutter while maintaining data completeness.                            | None         |
| 10  | state       | Load realistic sample data showing energy flows on initial render                             | minor  | Sample data enables users to immediately see the diagram working with realistic energy distribution.        | None         |
| 11  | interaction | Highlight clicked flow band with pulsing animation and show detail card                       | major  | Pulsing animation and detail card provide combined visual and informational feedback for the selected flow. | None         |
| 12  | content     | Show source, destination, and flow amount in detail card                                      | major  | The detail card gives users precise information about the specific flow they clicked.                       | None         |
| 13  | state       | Calculate efficiency rating based on flow percentage thresholds                               | major  | Efficiency ratings help users identify high-impact vs low-impact energy paths quickly.                      | None         |
| 14  | content     | Show efficiency as "high-efficiency", "medium-efficiency", or "low-efficiency" in detail card | major  | The three-tier efficiency system provides actionable categorization of flow importance.                     | C13          |

## Justification

The Energy Flow Sankey Diagram achieved 57% pass rate with six specific failures. The diagram correctly displays three source nodes on the left connected by curved bands with animated particles to four consumption zones on the right, with band widths proportional to flow percentages. When users click a flow band, a detail card appears showing source, destination, flow amount, and share of total. However, the model failed to draw thin dotted connector lines from flow bands to the legend. The legend appears embedded within the diagram instead of positioned directly below it. The legend displays only six flow percentages out of approximately twelve total flows, omitting roughly half including flows below 3% that should have been grouped as "Other". The clicked flow band's pulsing animation disappears immediately when the mouse leaves instead of persisting after click. Finally, the efficiency label displays as "High efficiency (> 15% of total)" instead of the required "high-efficiency" format.
