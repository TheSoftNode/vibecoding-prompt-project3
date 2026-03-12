Category: Data_Visualization

Prompt style: Feature_List

Title: Hierarchical Tree Depth Visualizer

Prompt: Build a hierarchical tree depth visualizer. Display a tree structure with a root node at the top labeled "Root" connected to 3 child nodes labeled "Branch A", "Branch B", "Branch C". Each branch connects to 2 sub-nodes with unique labels. When clicking any node, highlight the entire path from root to that node in blue and display its depth level number next to the node.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display tree structure with nodes and connecting lines    | major  | The tree visualization shows the hierarchical relationships users need to explore.                               | None         |
| 2   | content     | Display label "Root" on root node                         | minor  | The label helps users identify the top of the hierarchy.                                                         | None         |
| 3   | content     | Display labels "Branch A", "Branch B", "Branch C" on child nodes | minor | Branch labels help users tell the different children apart.                                                      | None         |
| 4   | content     | Display unique labels on sub-nodes                        | minor  | Unique labels help users identify individual sub-nodes within each branch.                                       | None         |
| 5   | interaction | Highlight path from root to clicked node in blue          | major  | Highlighting the path shows users the full ancestry of any node they click.                                      | None         |
| 6   | state       | Calculate depth level for clicked node                    | major  | Depth calculation determines how many levels down from root the clicked node sits.                               | None         |
| 7   | content     | Display depth level number next to clicked node           | minor  | Showing the number gives users exact hierarchy position information.                                             | C6           |
| 8   | layout      | Position root at top with branches below                  | minor  | Top-down layout makes the tree structure easy to read from root downward.                                        | None         |
| 9   | layout      | Position nodes in hierarchical tree layout                | major  | Proper spacing and alignment makes the tree structure easy to understand.                                        | None         |

## Justification

The hierarchical tree depth visualizer works exactly as expected with click-based path highlighting and depth level display. A root node labeled "Root" appears at the top of the tree structure. Three child nodes labeled "Branch A", "Branch B", and "Branch C" display below the root, connected by lines. Each branch connects to 2 sub-nodes with unique labels. Nodes are positioned in a clear hierarchical tree layout with proper vertical and horizontal spacing. When users click any node, the entire path from root to that node highlights in blue and the depth level number appears next to the clicked node.
