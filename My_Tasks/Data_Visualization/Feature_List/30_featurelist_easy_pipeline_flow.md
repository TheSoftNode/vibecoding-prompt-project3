Category: Data_Visualization

Prompt style: Feature_List

Title: Organization Hierarchy Chart

Prompt: Build an organization hierarchy chart that visualizes company reporting structure. Display a tree structure with a CEO node labeled "CEO" positioned at the top of the chart, connected by straight lines to 3 manager nodes labeled "Manager A", "Manager B", "Manager C" positioned below the CEO node. When users click any node in the organizational chart, highlight that specific node in orange color and display the node's team size number showing how many team members report to that position. Only the clicked node should show its team size number. Keep the clicked node highlighted in orange until a different node is clicked.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                           | Weight | Rationale                                                                                 | Dependent On |
| --- | ----------- | --------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display CEO node                                                      | major  | The CEO node shows the top of the organizational structure.                               | None         |
| 2   | visual      | Display 3 manager nodes                                               | major  | The manager nodes show the reporting structure users need to explore.                     | None         |
| 3   | layout      | Connect manager nodes A, B, C to CEO node with lines                  | major  | Lines connecting managers to the CEO establish the reporting hierarchy visually.          | C1, C2       |
| 4   | content     | Display label "CEO" on CEO node                                       | minor  | The label helps users identify the top of the organization.                               | C1           |
| 5   | content     | Display labels "Manager A", "Manager B", "Manager C" on manager nodes | minor  | Manager labels help users tell the different nodes apart.                                 | C2           |
| 6   | layout      | Position CEO at top of chart                                          | minor  | Top positioning makes the CEO the starting point of the org structure.                    | C1           |
| 7   | layout      | Position manager nodes below CEO node                                 | minor  | Below positioning creates hierarchical relationship between CEO and managers.             | C1, C2       |
| 8   | interaction | Highlight clicked node in orange                                      | major  | Orange highlighting shows users which node they selected.                                 | None         |
| 9   | interaction | Calculate team size for clicked node                                  | major  | Team size calculation happens when users click, determining the node's team count.        | None         |
| 10  | interaction | Display team size number for clicked node                             | major  | Showing the team size on click is the core behavior that reveals org information.         | None         |
| 11  | state       | Show team size only on clicked node                                   | minor  | Showing team size only on the selected node enforces the exclusivity rule.                | C10          |
| 12  | state       | Keep clicked node highlighted until different node is clicked         | minor  | Maintaining the highlight shows which node is currently selected for team size display.   | C8           |

## Justification

The organization hierarchy chart achieved 83.33% pass rate with two failures. A CEO node labeled "CEO" appears at the top of the organizational chart. Three manager nodes labeled "Manager A", "Manager B", and "Manager C" display below the CEO arranged in a horizontal row. When users click any node, that node highlights in orange. Only the clicked node shows its team size. The clicked node stays highlighted in orange until a different node is clicked. However, the straight lines connecting the manager nodes do not reach the CEO node as required. Additionally, the team size number displays inside the node rather than next to it as required.
