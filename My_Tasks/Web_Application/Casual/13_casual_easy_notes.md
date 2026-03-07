Category: Web Application

Prompt style: Casual

Title: Quick Notes App

Prompt: Notes app with priorities. Type note, pick priority (High, Medium, Low), click add. List shows note with colored dot next to the text - red for High, yellow for Medium, green for Low. Timestamp on each. Click note to edit inline. Delete button on each. On load, show 3 sample notes: one High with red dot, one Medium with yellow dot, one Low with green dot.

Required libraries: react, tailwindcss

## Rubric

| #  | ID            | Description                                              | Weight | Rationale                                                                    | Dependent On |
| -- | ------------- | -------------------------------------------------------- | ------ | ---------------------------------------------------------------------------- | ------------ |
| 1  | visual-1      | Render a text input for typing notes and a priority selector with High, Medium, Low options        | major  | These input elements are the core interface required for users to create notes with priority assignments.                      | None         |
| 2  | visual-2      | Display an add button                                    | major  | The button serves as the trigger for creating new notes in the list.                                           | None         |
| 3  | interaction-1 | Add a new note with selected priority to the list when the add button is clicked | major  | This action creates notes with priority metadata, enabling the full priority-based display system.                              | visual-2     |
| 4  | content-1     | Display each note in a list with its text content and timestamp                              | major  | Showing note text and timestamps provides essential information for users to identify and track their notes.                                    | None         |
| 5  | state-1      | Display red colored dot for High priority notes, yellow colored dot for Medium priority notes, and green colored dot for Low priority notes                    | major  | Color-coded dots provide instant visual priority differentiation without requiring users to read text labels.                                          | content-1    |
| 6  | layout-1     | Position the colored dot next to the note text             | minor  | Placing dots adjacent to note text creates clear visual association between priority and content.            | state-1    |
| 7  | interaction-2 | Enable inline editing when a note is clicked             | major  | Click-to-edit allows quick modifications without navigating away or opening separate edit forms.            | content-1    |
| 8  | visual-3      | Display a delete button for each note                    | major  | Individual delete buttons give users direct control to remove specific notes.                                          | content-1    |
| 9  | interaction-3 | Remove the note from the list when its delete button is clicked        | major  | Deletion removes unwanted notes from the interface, maintaining a clean and relevant note collection.                                   | visual-3     |
| 10 | content-2     | Display 3 sample notes on initial load with one High priority note showing red dot, one Medium priority note showing yellow dot, and one Low priority note showing green dot                        | major  | Pre-populated sample notes demonstrate the full feature set and provide immediate visual examples of the priority system in action.                           | None    |
