Category: Data_Visualization

Prompt style: Feature_List

Title: Organization Hierarchy Chart

Prompt: Build an organization hierarchy chart that visualizes company reporting structure. Display a tree structure with a CEO node labeled "CEO" positioned at the top of the chart, connected by straight lines to 3 manager nodes labeled "Manager A", "Manager B", "Manager C" positioned below it in a horizontal row. When users click any node in the organizational chart, highlight that specific node in orange color and display its team size number next to it showing how many team members report to that position. Only the clicked node should show its team size number. Keep the clicked node highlighted in orange until a different node is clicked.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                   | Weight | Rationale                                                                           | Dependent On |
| --- | ----------- | ------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display CEO node and 3 manager nodes                          | major  | The nodes show the organizational structure users need to explore.                  | None         |
| 2   | layout      | Connect manager nodes A, B, C to CEO node with lines          | major  | Connecting managers to the CEO establishes the reporting hierarchy visually.        | None         |
| 3   | content     | Display label "CEO" on CEO node                               | minor  | The label helps users identify the top of the organization.                         | None         |
| 4   | content     | Display labels "Manager A", "Manager B", "Manager C" on manager nodes | minor  | Manager labels help users tell the different nodes apart.                           | None         |
| 5   | interaction | Highlight clicked node in orange                              | major  | Orange highlighting shows users which node they selected.                           | None         |
| 6   | interaction | Calculate team size for clicked node                          | major  | Team size calculation happens when users click, determining the node's team count.  | None         |
| 7   | interaction | Display team size number next to clicked node                 | major  | Showing the team size on click is the core behavior that reveals org information.   | None         |
| 8   | layout      | Position CEO at top with manager nodes below                  | minor  | Top-down layout makes the org structure easy to read from CEO downward.             | None         |
| 9   | state       | Keep clicked node highlighted until different node is clicked | minor  | Maintaining the highlight shows which node is currently selected for team size display. | None         |

## Justification

The organization hierarchy chart works exactly as expected for visualizing company structure. A CEO node labeled "CEO" appears at the top of the organizational chart. Three manager nodes labeled "Manager A", "Manager B", and "Manager C" display below the CEO. Lines connect each manager node to the CEO node. When users click any node, that node highlights in orange and displays its team size number next to it. Only the clicked node shows its team size. The clicked node stays highlighted in orange until a different node is clicked.
