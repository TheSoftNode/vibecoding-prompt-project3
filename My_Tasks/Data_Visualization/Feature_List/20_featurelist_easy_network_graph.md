Category: Data_Visualization

Prompt style: Feature_List

Title: Network Connection Graph Analyzer

Prompt: Build a network connection graph analyzer that visualizes server-client relationships in a distributed system. Display a central server node labeled "Server" positioned in the middle of the interface, connected by straight lines to 4 client nodes labeled "Client 1", "Client 2", "Client 3", "Client 4" arranged around it in a radial pattern. When users click any client node, highlight that specific node in green color and display its connection count number next to it. Only the clicked node should show its connection count. Keep the clicked node highlighted in green until a different node is clicked.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                     | Weight | Rationale                                                                                | Dependent On |
| --- | ----------- | --------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display server node                                             | major  | The server node shows the central hub of the network structure.                          | None         |
| 2   | visual      | Display 4 client nodes                                          | major  | The client nodes show the connected devices users need to explore.                       | None         |
| 3   | layout      | Connect client nodes to server node with straight lines         | major  | Straight lines connecting clients to the server establish the network topology visually. | C1, C2       |
| 4   | content     | Display label "Server" on server node                           | minor  | The label helps users identify the central hub of the network.                           | C1           |
| 5   | content     | Display labels "Client 1", "Client 2", "Client 3", "Client 4"   | minor  | Client labels help users tell the different nodes apart.                                 | C2           |
| 6   | layout      | Position server in middle of interface                          | minor  | Central positioning makes the server the focal point of the network.                     | C1           |
| 7   | layout      | Arrange client nodes around server in radial pattern            | minor  | Radial layout makes the network structure easy to read from center outward.              | C2           |
| 8   | interaction | Highlight clicked client node in green color                    | major  | Green highlighting shows users which client node they selected.                          | None         |
| 9   | interaction | Calculate connection count for clicked node                     | major  | Connection calculation happens when users click, determining the node's connectivity.    | None         |
| 10  | interaction | Display connection count number next to clicked node            | major  | Showing the count on click is the core behavior that reveals network information.        | C9           |
| 11  | state       | Keep clicked node highlighted until different node is clicked   | minor  | Maintaining the highlight shows which node is currently selected for connection display. | C8           |

## Justification

The network connection graph analyzer achieved a 77.78% pass rate with two specific failures. A server node labeled "Server" appears in the middle of the network structure. Four client nodes labeled "Client 1", "Client 2", "Client 3", and "Client 4" display around the server. When users click any client node, that node highlights in green and the clicked node stays highlighted until a different node is clicked. However, the model failed to connect the client nodes to the server node with lines as required. Additionally, the model displayed connection count numbers on all nodes simultaneously as static text, instead of showing the connection count only on the clicked node. These two positioning and interaction failures caused the 80% pass rate despite the highlighting and selection persistence working correctly.
