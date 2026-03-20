Category: Data_Visualization

Prompt style: Feature_List

Title: Pipeline Stage Flow Visualizer

Prompt: Build a pipeline stage flow visualizer that shows data processing stages in a deployment pipeline. Display a source stage node labeled "Source" positioned on the left side of the interface, connected by curved lines to 3 processing stage nodes labeled "Build", "Test", "Deploy" arranged vertically to the right of it. When users click any processing stage node, highlight that specific node in purple color and display its execution time number next to it. Only the clicked node should show its execution time. Keep the clicked node highlighted in purple until a different node is clicked.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                     | Weight | Rationale                                                                                 | Dependent On |
| --- | ----------- | --------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display source stage node                                       | major  | The source node shows the starting point of the pipeline flow.                            | None         |
| 2   | visual      | Display 3 processing stage nodes                                | major  | The processing nodes show the stages users need to explore.                               | None         |
| 3   | layout      | Connect processing nodes to source node with curved lines       | major  | Curved lines connecting stages to source establish the pipeline flow visually.            | C1, C2       |
| 4   | content     | Display label "Source" on source node                           | minor  | The label helps users identify the pipeline entry point.                                  | C1           |
| 5   | content     | Display labels "Build", "Test", "Deploy" on processing nodes    | minor  | Stage labels help users tell the different processing nodes apart.                        | C2           |
| 6   | layout      | Position source on left side of interface                       | minor  | Left positioning makes the source the starting point of the flow.                         | C1           |
| 7   | layout      | Arrange processing nodes vertically to the right of source      | minor  | Vertical arrangement makes the pipeline stages easy to read from top to bottom.           | C2           |
| 8   | interaction | Highlight clicked processing node in purple color               | major  | Purple highlighting shows users which processing stage they selected.                     | None         |
| 9   | interaction | Display execution time number next to clicked node              | major  | Showing the time on click is the core behavior that reveals stage performance.            | None         |
| 10  | state       | Show execution time only on clicked node                        | minor  | Showing the time only on the selected node enforces the exclusivity rule.                 | C9           |
| 11  | state       | Keep clicked node highlighted until different node is clicked   | minor  | Maintaining the highlight shows which node is currently selected for time display.        | C8           |

## Justification

The pipeline stage flow visualizer works exactly as expected for visualizing deployment pipeline stages. A source stage node labeled "Source" displays positioned on the left side of the interface. Three processing stage nodes labeled "Build", "Test", and "Deploy" display arranged vertically to the right of the source. Curved lines connect each processing stage node to the source node. When users click any processing stage node, that node highlights in purple color and displays its execution time number next to it. Only the clicked node shows its execution time. The clicked node stays highlighted in purple until a different node is clicked.
