Category: Web Application

Prompt style: Detailed Specification

Title: Document Layout Builder

Prompt: Build a document layout builder with three connected panels showing visual linking between components. Display a header image panel positioned at top-left, a sections list panel positioned at bottom-left directly below the header panel, and a document preview panel positioned at top-right. Load initial sample header image and three pre-populated section items on startup: "Introduction" section, "Content" section, and "Conclusion" section. Draw thin dotted connecting lines from each section in the bottom-left list to its corresponding rendered block in the top-right document preview. When users click a section in the list, highlight both the list item and its preview block, and change the connecting line from dotted to solid. The document preview rendering depends on section priority order: Introduction must render at the top of the preview, Content in the middle after Introduction is positioned, and Conclusion at the bottom after Content is positioned.

Required libraries: react, tailwindcss, lucide-react, react-beautiful-dnd

## Rubric

| #   | ID          | Description                                                                              | Weight | Rationale                                                                                     | Dependent On |
| --- | ----------- | ---------------------------------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------- | ------------ |
| 1   | layout      | Display header image panel positioned at top-left                                        | major  | Top-left positioning creates the primary visual anchor for the document header.               | None         |
| 2   | layout      | Display sections list panel positioned at bottom-left directly below header panel        | major  | Bottom-left positioning creates vertical panel alignment with header above.                   | C1           |
| 3   | layout      | Display document preview panel positioned at top-right                                   | major  | Top-right positioning separates the input sections from the output preview.                   | None         |
| 4   | state       | Load initial sample header image on startup                                              | major  | Loading header image provides immediate initial state for the header panel.                   | None         |
| 5   | content     | Display Introduction section pre-populated in sections list on initial load              | major  | Introduction section provides the first verifiable initial section.                           | None         |
| 6   | content     | Display Content section pre-populated in sections list on initial load                   | major  | Content section provides the second verifiable initial section.                               | None         |
| 7   | content     | Display Conclusion section pre-populated in sections list on initial load                | major  | Conclusion section provides the third verifiable initial section.                             | None         |
| 8   | visual      | Display thin dotted connecting lines from each section in list to its block in preview   | major  | Dotted lines create visual correspondence showing which list item maps to which preview block.| C2, C3       |
| 9   | interaction | Highlight clicked section in list when clicked                                           | major  | List highlight shows users which section they selected.                                       | None         |
| 10  | interaction | Highlight clicked section's preview block when clicked                                   | major  | Preview block highlight shows users the corresponding preview section.                        | None         |
| 11  | interaction | Change connecting line from dotted to solid when section clicked                         | major  | Solid line change provides visual feedback for the active connection.                         | C8           |
| 12  | state       | Render Introduction section at top of document preview                                   | major  | Top positioning enforces Introduction as the document starting point.                         | C5           |
| 13  | state       | Render Content section in middle of document preview after Introduction is positioned    | major  | Middle positioning enforces document structure and depends on Introduction first.             | C12          |
| 14  | state       | Render Conclusion section at bottom of document preview after Content is positioned      | major  | Bottom positioning completes the document hierarchy and depends on Content first.             | C13          |

## Justification

The Document Layout Builder with Visual Links will be evaluated based on its ability to coordinate three interconnected panels with visual linking and render dependencies. Success requires displaying the header image panel at top-left with a loaded sample header image, the sections list panel at bottom-left positioned directly below the header panel showing three pre-populated sections (Introduction, Content, Conclusion), and the document preview panel at top-right. Thin dotted connecting lines must be drawn from each section in the bottom-left list to its corresponding rendered block in the top-right document preview. When users click a section in the list, the implementation must highlight both the list item and its preview block while simultaneously changing the connecting line from dotted to solid style. The document preview must enforce section priority order by rendering Introduction at the top, Content in the middle after Introduction is positioned (state-3 depends on state-2), and Conclusion at the bottom after Content is positioned (state-4 depends on state-3). This task tests multi-panel layout positioning with specific spatial relationships (bottom-left directly below top-left), initial data loading (header image on startup), visual linking through connecting lines with dynamic style changes on interaction, and sequential section rendering dependencies where each section depends on the previous one being positioned first.
