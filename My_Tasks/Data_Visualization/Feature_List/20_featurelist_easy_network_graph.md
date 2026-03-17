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
| 9   | interaction | Display connection count number next to clicked node            | major  | Showing the count on click is the core behavior that reveals network information.        | None         |
| 10  | state       | Show connection count only on clicked node                      | minor  | Showing the count only on the selected node enforces the exclusivity rule.               | C9           |
| 11  | state       | Keep clicked node highlighted until different node is clicked   | minor  | Maintaining the highlight shows which node is currently selected for connection display. | C8           |

## Justification

The network connection graph analyzer works exactly as expected for visualizing server-client relationships. A server node labeled "Server" displays positioned in the middle of the interface. Four client nodes labeled "Client 1", "Client 2", "Client 3", and "Client 4" display arranged around the server in a radial pattern. Straight lines connect each client node to the server node. When users click any client node, that node highlights in green color and displays its connection count number next to it. Only the clicked node shows its connection count. The clicked node stays highlighted in green until a different node is clicked.
