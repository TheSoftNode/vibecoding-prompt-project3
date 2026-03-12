Category: Data_Visualization

Prompt style: Feature_List

Title: Hierarchical Tree Depth Visualizer

Prompt: Build a hierarchical tree depth visualizer. Display a tree structure with a root node at the top labeled "Root" connected to 3 child nodes labeled "Branch A", "Branch B", "Branch C". Each branch connects to 2 sub-nodes labeled with numbers (A1, A2 for Branch A, B1, B2 for Branch B, C1, C2 for Branch C). When hovering over any node, highlight the entire path from root to that node in blue and display the depth level number (0 for root, 1 for branches, 2 for sub-nodes) next to the hovered node.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display tree structure with nodes and connecting lines    | major  | The tree visualization shows the hierarchical relationships users need to explore.                               | None         |
| 2   | content     | Display label "Root" on root node                         | minor  | The label helps users identify the top of the hierarchy.                                                         | None         |
| 3   | content     | Display labels "Branch A", "Branch B", "Branch C" on child nodes | minor | Branch labels help users tell the different children apart.                                                      | None         |
| 4   | content     | Display labels A1, A2, B1, B2, C1, C2 on sub-nodes        | minor  | Numbered labels help users identify individual sub-nodes within each branch.                                     | None         |
| 5   | interaction | Highlight path from root to hovered node in blue          | major  | Highlighting the path shows users the full ancestry of any node they point to.                                   | None         |
| 6   | state       | Calculate depth level for hovered node                    | major  | Depth calculation tells users how many levels down from root the node sits.                                      | None         |
| 7   | content     | Display depth level number next to hovered node           | minor  | Showing the number gives users exact hierarchy position information.                                             | C6           |
| 8   | layout      | Position root at top with branches below                  | minor  | Top-down layout makes the tree structure easy to read from root downward.                                        | None         |
| 9   | layout      | Position nodes in hierarchical tree layout                | major  | Proper spacing and alignment makes the tree structure easy to understand.                                        | None         |

## Justification

The hierarchical tree depth visualizer works exactly as expected with path highlighting and depth level display. A root node labeled "Root" appears at the top of the tree structure. Three child nodes labeled "Branch A", "Branch B", and "Branch C" display below the root, connected by lines. Each branch connects to 2 sub-nodes labeled A1, A2, B1, B2, C1, and C2 respectively. Nodes are positioned in a clear hierarchical tree layout with proper vertical and horizontal spacing. When users hover over any node, the entire path from root to that node highlights in blue, and the depth level number appears next to the hovered node showing 0 for root, 1 for branches, and 2 for sub-nodes.
