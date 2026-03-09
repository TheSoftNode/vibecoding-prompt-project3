Category: SVG Generation

Prompt style: Conversational

Title: Simple Flowchart Builder

Prompt: I need to create SVG flowcharts with connected boxes. I want an "Add Box" button that creates a box with editable label text. Each box should have a small "Connect" button that lets me click another box to draw an SVG arrow line from the first box to the second box. The arrow should point from the right edge of the source box to the left edge of the target box. I should be able to edit the label text on any box. When I click a box, highlight it with a colored border. At the bottom, show the total box count as the sum of all boxes in the flowchart.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                                           | Weight | Rationale                                                                                                                                                         | Dependent On |
| --- | ----------- | ----------------------------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display "Add Box" button                                                                             | major  | The add box button provides the interface for creating flowchart boxes dynamically.                                                                              | None         |
| 2   | interaction | Create new box with editable label text field when Add Box button is clicked                         | major  | Creating boxes on demand lets users build flowcharts by adding as many boxes as needed.                                                                          | C1           |
| 3   | visual      | Render each box as SVG with the entered label text                                                   | major  | The box SVG displays the flowchart step with user-entered text as vector graphics.                                                                               | C2           |
| 4   | visual      | Display "Connect" button on each box                                                                 | major  | The connect button on each box enables creating connections between boxes to show flow.                                                                          | None         |
| 5   | interaction | Enter connection mode when Connect button on a box is clicked                                        | major  | Connection mode allows users to select a target box to establish directed flow relationships.                                                                    | C4           |
| 6   | interaction | Draw SVG arrow line from source box to target box when target box is clicked in connection mode      | major  | The arrow line visually represents the directional flow from one step to another in the flowchart.                                                               | C5           |
| 7   | layout      | Route arrow from right edge of source box to left edge of target box                                 | major  | Edge-to-edge arrow routing positions the connection line at logical anchor points showing directional flow.                                                      | C6           |
| 8   | interaction | Allow editing label text field on any box                                                            | major  | Editable fields let users update box labels after creation for maintaining accurate flowcharts.                                                                  | None         |
| 9   | interaction | Highlight box with colored border when it is clicked                                                 | major  | Border highlighting provides visual feedback showing which box is currently selected.                                                                            | None         |
| 10  | content     | Display total box count at the bottom                                                                | major  | The box count label provides summary information about the flowchart size.                                                                                       | None         |
| 11  | state       | Calculate total box count as the sum of all boxes in the flowchart                                   | major  | Counting all boxes aggregates the flowchart size dynamically as boxes are added to the chart.                                                                    | C10          |

## Justification

The flowchart builder works exactly as expected with dynamic SVG box creation and connections. An "Add Box" button is displayed for creating flowchart boxes. Clicking it creates a new box with an editable label text field that renders as an SVG box with the entered label text. Each box displays a small "Connect" button on it. When the Connect button on a box is clicked, connection mode is entered allowing the user to click another target box. When a target box is clicked in connection mode, an SVG arrow line is drawn from the source box to the target box, with the arrow pointing from the right edge of the source box to the left edge of the target box. The label text field on any box can be edited after creation. Clicking on a box highlights it with a colored border. At the bottom, the total box count is displayed, calculated as the sum of all boxes in the flowchart.
