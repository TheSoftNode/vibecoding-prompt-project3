Category: Multimedia_Editing

Prompt style: Casual

Title: Shape Connector Canvas

Prompt: Shape connector tool. Draw circles by clicking canvas. Click two circles to draw line connecting them. Delete shapes removes connected lines too.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                 | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display blank canvas for drawing                            | major  | The canvas provides the drawing area where users create shapes and connections.                                  | None         |
| 2   | interaction | Draw circle at click position when user clicks canvas       | major  | Clicking creates circles so users can add shapes to connect.                                                     | None         |
| 3   | state       | Position circle exactly where user clicked                  | major  | Precise positioning ensures circles appear where users intended to place them.                                   | C2           |
| 4   | visual      | Display all drawn circles on canvas                         | major  | Showing all circles lets users see what shapes are available to connect.                                         | None         |
| 5   | interaction | Select two circles by clicking them                         | major  | Clicking two circles marks which shapes the user wants to connect with a line.                                   | None         |
| 6   | interaction | Draw line connecting the two selected circles               | major  | Drawing the line creates the visual connection between the two shapes.                                           | C5           |
| 7   | state       | Position line endpoints at circle centers                   | major  | Lines must connect at circle centers to look properly attached to the shapes.                                    | C6           |
| 8   | visual      | Display all connection lines on canvas                      | major  | Showing all lines lets users see the network of connections they've created.                                     | None         |
| 9   | interaction | Delete circle when user clicks delete on shape              | major  | Deleting circles lets users remove shapes they don't want in their diagram.                                      | None         |
| 10  | state       | Remove all lines connected to deleted circle                | major  | Removing connected lines prevents orphaned lines when their endpoint shape is gone.                              | C9           |
| 11  | state       | Maintain remaining circles visible after deletion           | major  | Other circles must stay visible so users can continue building their diagram.                                    | C9           |
| 12  | state       | Maintain remaining lines visible after deletion             | minor  | Lines between other circles must stay visible and connected after one shape is removed.                          | C10          |

## Justification

The Shape Connector Canvas lets users create diagrams by drawing circles and connecting them with lines. A blank canvas displays where users can click to draw circles. Each click creates a circle positioned exactly where the user clicked. All drawn circles display on the canvas. Users can click two circles to select them, which draws a line connecting the two shapes with endpoints positioned at the circle centers. All connection lines display on the canvas showing the network. When users delete a circle, it removes that shape and all lines connected to it, while maintaining the remaining circles and their connections visible.
