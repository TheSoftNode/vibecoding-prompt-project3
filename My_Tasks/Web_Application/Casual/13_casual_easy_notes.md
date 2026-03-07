Category: Web Application

Prompt style: Casual

Title: Quick Notes App

Prompt: Notes app with priorities. Type note, pick priority (High, Medium, Low), click add. After clicking add, the list shows the note text with a colored dot next to the text - red for High, yellow for Medium, green for Low. Delete button on each note.

Required libraries: react, tailwindcss

## Rubric

| #   | ID            | Description                                                                                                                                 | Weight | Rationale                                                                                                     | Dependent On |
| --- | ------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual-1      | Render a text input for typing notes                                                                                                        | major  | The text input is the primary interface element that allows users to enter note content.                      | None         |
| 2   | visual-2      | Render an add button                                                                                                                        | major  | The button serves as the trigger for creating new notes in the list.                                          | None         |
| 3   | interaction-1 | Add a new note with selected priority to the list when the add button is clicked                                                            | major  | This action creates notes with priority metadata, enabling the full priority-based display system.            | visual-2     |
| 4   | content-1     | Display each note in a list with its text content                                                                                           | major  | Showing note text provides essential information for users to identify their notes.                           | interaction-1|
| 5   | state-1       | Display a red colored dot for High priority notes, a yellow colored dot for Medium priority notes, and a green colored dot for Low priority notes | major  | Color-coded dots provide instant visual priority differentiation without requiring users to read text labels. | content-1    |
| 6   | layout-1      | Position the colored dot next to the note text                                                                                              | minor  | Placing dots adjacent to note text creates clear visual association between priority and content.             | state-1      |
| 7   | visual-3      | Render a delete button for each note                                                                                                        | major  | Individual delete buttons give users direct control to remove specific notes.                                 | content-1    |
| 8   | interaction-2 | Remove the note from the list when its delete button is clicked                                                                             | major  | Deletion removes unwanted notes from the interface, maintaining a clean and relevant note collection.         | visual-3     |
| 9   | content-2     | Display a priority selector with High, Medium, and Low options                                                                              | major  | These three priority options provide the specific selection choices users need to categorize their notes.     | None         |
