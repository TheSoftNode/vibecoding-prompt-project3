Category: Web Application

Prompt style: Detailed Specification

Title: Document Layout Builder

Prompt: Build a document layout builder with two panels showing visual linking between components. Display a sections list panel showing draggable section items. Display a document preview panel. Load three pre-populated section items on startup: "Introduction" section, "Content" section, and "Conclusion" section. Draw thin dotted connecting lines from each section in the list to its corresponding rendered block in the preview. When users drag a section item to reorder it within the list, automatically update the document preview to re-render all sections in the new order while animating the connecting lines to follow their new positions. When users double-click any section in the list, open an inline text editor allowing users to rename that section, and when users press Enter or click outside the editor, save the new name updating both the list item label and the corresponding preview block header simultaneously.

Required libraries: react, tailwindcss, lucide-react, react-beautiful-dnd

## Rubric

| #   | ID          | Description                                                                                    | Weight | Rationale                                                                                              | Dependent On |
| --- | ----------- | ---------------------------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display draggable section items in sections list panel                                         | major  | Draggable items enable users to reorder sections.                                                      | None         |
| 2   | visual      | Display document preview panel                                                                  | major  | Preview panel shows the rendered document output.                                                      | None         |
| 3   | content     | Load Introduction section pre-populated on startup                                             | major  | Introduction section provides the first verifiable initial section.                                    | None         |
| 4   | content     | Load Content section pre-populated on startup                                                  | major  | Content section provides the second verifiable initial section.                                        | None         |
| 5   | content     | Load Conclusion section pre-populated on startup                                               | major  | Conclusion section provides the third verifiable initial section.                                      | None         |
| 6   | visual      | Draw thin dotted connecting lines from each section in list to its block in preview            | major  | Dotted lines create visual correspondence showing which list item maps to which preview block.         | C1, C2       |
| 7   | interaction | Update document preview to re-render sections in new order when section dragged                | major  | Preview re-rendering keeps the document output synchronized with the new section order.                | C1           |
| 8   | visual      | Animate connecting lines to follow new positions when section dragged                          | major  | Line animation provides visual feedback showing the connection paths update to new positions.          | C6, C7       |
| 9   | interaction | Open inline text editor when section double-clicked                                            | major  | Inline editor allows users to rename sections directly in the list.                                    | None         |
| 10  | interaction | Save new name when Enter pressed in inline editor                                              | major  | Enter key provides keyboard shortcut for saving the renamed section.                                   | C9           |
| 11  | interaction | Save new name when user clicks outside inline editor                                           | major  | Click-outside provides mouse interaction for saving the renamed section.                               | C9           |
| 12  | state       | Update list item label with new name after save                                                | major  | List label update reflects the section rename in the sections list panel.                              | C10, C11     |
| 13  | state       | Update preview block header with new name after save                                           | major  | Preview header update reflects the section rename in the document preview panel.                       | C10, C11     |

## Justification

The Document Layout Builder will be evaluated based on its ability to coordinate two interconnected panels with drag-and-drop reordering and inline editing with synchronized updates. Success requires displaying a sections list panel showing draggable section items and a document preview panel. Three pre-populated sections must load on startup: Introduction, Content, and Conclusion. Thin dotted connecting lines must be drawn from each section in the list to its corresponding rendered block in the preview. When users drag a section item to reorder it, the implementation must automatically update the document preview to re-render all sections in the new order while animating the connecting lines to follow their new positions. When users double-click any section in the list, the implementation must open an inline text editor, and when users press Enter or click outside the editor, save the new name updating both the list item label and the corresponding preview block header simultaneously. This task tests drag-and-drop interaction with synchronized preview updates and animated line transitions, and inline editing with dual-location name synchronization.
