Category: Data_Visualization

Prompt style: Feature_List

Title: Hierarchical Tree Depth Visualizer

Prompt: Build a hierarchical tree depth visualizer. Display a tree structure with a root node labeled "Root" at the top, connected to 3 child nodes labeled "A", "B", "C" below it. When clicking any node, highlight that node in blue and show its depth level number next to it. Only the clicked node should show its depth number. Keep the clicked node highlighted until a different node is clicked.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                   | Weight | Rationale                                                                           | Dependent On |
| --- | ----------- | ------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display root node and 3 child nodes                           | major  | The nodes show the hierarchical structure users need to explore.                    | None         |
| 2   | layout      | Connect child nodes A, B, C to root node with lines           | major  | Connecting children to the root establishes the parent-child hierarchy visually.    | None         |
| 3   | content     | Display label "Root" on root node                             | minor  | The label helps users identify the top of the hierarchy.                            | None         |
| 4   | content     | Display labels "A", "B", "C" on child nodes                   | minor  | Child labels help users tell the different nodes apart.                             | None         |
| 5   | interaction | Highlight clicked node in blue                                | major  | Blue highlighting shows users which node they selected.                             | None         |
| 6   | interaction | Calculate depth level for clicked node                        | major  | Depth calculation happens when users click, determining the node's hierarchy level. | None         |
| 7   | interaction | Display depth level number next to clicked node               | major  | Showing the depth on click is the core behavior that reveals hierarchy information. | None         |
| 8   | layout      | Position root at top with child nodes below                   | minor  | Top-down layout makes the tree structure easy to read from root downward.           | None         |
| 9   | state       | Keep clicked node highlighted until different node is clicked | minor  | Maintaining the highlight shows which node is currently selected for depth display. | None         |

## Justification

The hierarchical tree depth visualizer achieved an 77.78% pass rate with two specific failures. A root node labeled "Root" appears at the top of the tree structure. Three child nodes labeled "A", "B", and "C" display below the root. When users click any node, that node highlights in blue and the clicked node stays highlighted until a different node is clicked. However, the model failed to connect the child nodes to the root node with lines as required. Additionally, the model displayed depth level numbers on all nodes simultaneously as static text, instead of showing the depth number only on the clicked node. These two positioning and interaction failures caused the 80% pass rate despite the highlighting and selection persistence working correctly.
