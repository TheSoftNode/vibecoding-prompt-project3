Category: Data_Visualization

Prompt style: Feature_List

Title: Hierarchical Tree Depth Visualizer

Prompt: Build a hierarchical tree depth visualizer. Display a tree structure with a root node labeled "Root" at the top, connected to 3 child nodes labeled "A", "B", "C" below it. When clicking any node, highlight that node in blue and display its depth level number next to it.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display tree structure with nodes and connecting lines    | major  | The tree visualization shows the hierarchical relationships users need to explore.                               | None         |
| 2   | content     | Display label "Root" on root node                         | minor  | The label helps users identify the top of the hierarchy.                                                         | None         |
| 3   | content     | Display labels "A", "B", "C" on child nodes               | minor  | Child labels help users tell the different nodes apart.                                                          | None         |
| 4   | interaction | Highlight clicked node in blue                            | major  | Blue highlighting shows users which node they selected.                                                          | None         |
| 5   | state       | Calculate depth level for clicked node                    | major  | Depth calculation determines how many levels down from root the clicked node sits.                               | None         |
| 6   | interaction | Display depth level number next to clicked node           | major  | Showing the depth on click is the core behavior that reveals hierarchy information.                              | None         |
| 7   | layout      | Position root at top with child nodes below               | minor  | Top-down layout makes the tree structure easy to read from root downward.                                        | None         |
| 8   | visual      | Connect nodes with lines to show parent-child relationships | major | Connection lines make the hierarchical structure clear and easy to follow.                                       | None         |

## Justification

The hierarchical tree depth visualizer works exactly as expected with click-based highlighting and depth level display. A root node labeled "Root" appears at the top of the tree structure. Three child nodes labeled "A", "B", and "C" display below the root, connected by lines showing parent-child relationships. Nodes are positioned in a clear top-down hierarchical layout. When users click any node, that node highlights in blue and the depth level number appears next to the clicked node.
