Category: Data_Visualization

Prompt style: Casual

Title: Team Collaboration Network Graph

Prompt: Need a collaboration network showing 8 team members as circles connected by lines with varying connection counts. Make circle sizes match their connection counts - more connections mean bigger circles. Group connected people closer together and keep circles from overlapping. When I click someone's circle, highlight their connections in blue and dim everyone else. Show a sidebar with the person's name, connection count, and collaborators. Display overall network density below. Clicking again deselects. Load with sample team data showing realistic collaboration patterns.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                 | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display eight circles representing team members                  | major  | The eight circles provide the foundation for visualizing the team structure.                              | None         |
| 2   | content     | Label each circle with member name                               | minor  | Names help users identify who each circle represents in the network.                                      | None         |
| 3   | visual      | Draw lines connecting team members as specified                  | major  | Connection lines show the collaboration relationships between team members.                               | C1           |
| 4   | state       | Size circles based on connection count (3 largest, 2 medium, 1 smallest) | major  | Size variation helps users quickly identify highly connected vs isolated team members.                    | None         |
| 5   | layout      | Position connected members closer together                       | major  | Proximity clustering reveals collaboration groups and network structure patterns.                         | C1, C3       |
| 6   | layout      | Position circles with no overlaps                                | major  | Non-overlapping circles ensure all team members remain visible and identifiable.                          | C1           |
| 7   | layout      | Route lines to avoid crossing through circles                    | minor  | Avoiding circle crossings improves readability of connection paths.                                       | C3, C6       |
| 8   | interaction | Highlight clicked person's circle                                | major  | Highlighting provides clear visual feedback about which person the user selected.                         | None         |
| 9   | interaction | Highlight direct connections in blue when circle clicked         | major  | Blue highlighting shows which team members collaborate with the selected person.                          | C8           |
| 10  | visual      | Gray out non-connected members when circle clicked               | major  | Graying out unconnected members focuses attention on the selected person's collaboration network.         | C8           |
| 11  | content     | Display sidebar on the right when circle clicked                 | minor  | Right-side positioning keeps the sidebar visible without covering the main network graph.                 | C8           |
| 12  | content     | Show clicked person's name in sidebar                            | minor  | The name confirms which person's details are being displayed.                                             | C11          |
| 13  | content     | Show connection count in sidebar                                 | minor  | The count gives users a quantitative measure of the person's collaboration level.                         | C11          |
| 14  | content     | List all connected names in sidebar                              | major  | The list shows exactly who the selected person collaborates with.                                         | C11          |
| 15  | state       | Calculate network density as actual connections / 28             | major  | Network density provides an overall measure of how interconnected the team is.                            | None         |
| 16  | interaction | Deselect and remove sidebar when clicking same person again      | minor  | Deselection allows users to return to the full network view easily.                                       | C8           |

## Justification

The Team Collaboration Network Graph achieved 56% pass rate (9/16 criteria) with failures in layout algorithms and interaction details. The visualization correctly displays eight circles labeled with team member names (C1, C2 passed) and draws all specified connection lines accurately (C3 passed). Circle sizing worked correctly with three distinct sizes: Alice and Carol (3 connections) rendered as large circles, Bob, Dan, Frank, and Grace (2 connections) as medium, and Eve and Henry (1 connection) as small (C4 passed). However, the model failed C5 by placing members in a random scattered layout instead of positioning connected members closer together - Alice, Bob, Carol, and Dan should form a tight cluster but were spread across opposite corners. The layout algorithm failed C6 with Bob's circle overlapping partially with Eve's circle, making labels hard to read. Line routing failed C7, with multiple connection lines passing directly through unrelated circles instead of curving around them. Click interactions worked partially: clicking a circle highlighted it with a border (C8 passed) and displayed a sidebar on the right (C11 passed) showing the person's name (C12 passed), connection count (C13 passed), and list of connected names (C14 passed). The blue highlighting worked (C9 passed), but the model failed C10 by completely hiding non-connected members instead of graying them out - when clicking Alice, only Alice, Bob, Carol, and Dan remained visible while Eve, Frank, Grace, and Henry disappeared entirely. Network density calculation failed C15 by showing 0.5 (50%) instead of the correct 0.43 (12 actual connections / 28 maximum). The deselect interaction failed C16 - clicking the same person again did nothing instead of removing the selection and hiding the sidebar.
