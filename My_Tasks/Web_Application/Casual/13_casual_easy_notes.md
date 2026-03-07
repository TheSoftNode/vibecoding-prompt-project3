Category: Web Application

Prompt style: Casual

Title: Quick Notes App

Prompt: Notes app with priorities. Type note, pick priority (High, Medium, Low), click add. After clicking add, the list shows the note text with a colored dot next to the text - red for High, yellow for Medium, green for Low. Delete button on each note.

Required libraries: react, tailwindcss

## Rubric

| #   | ID          | Description                                                                                                                                 | Weight | Rationale                                                                                                     | Dependent On |
| --- | ----------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Render a text input for typing notes                                                                                                        | major  | These input element is the core interface required for users to create notes.                                 | None         |
| 2   | visual      | Display an add button                                                                                                                       | major  | The button serves as the trigger for creating new notes in the list.                                          | None         |
| 3   | interaction | Add a new note with selected priority to the list when the add button is clicked                                                            | major  | This action creates notes with priority metadata, enabling the full priority-based display system.            | C2           |
| 4   | content     | Display each note in a list with its text content                                                                                           | major  | Showing note text provides essential information for users to identify their notes.                           | None         |
| 5   | state       | Display red colored dot for High priority notes, yellow colored dot for Medium priority notes, and green colored dot for Low priority notes | major  | Color-coded dots provide instant visual priority differentiation without requiring users to read text labels. | C4           |
| 6   | layout      | Position the colored dot next to the note text                                                                                              | minor  | Placing dots adjacent to note text creates clear visual association between priority and content.             | C5           |
| 7   | visual      | Display a delete button for each note                                                                                                       | major  | Individual delete buttons give users direct control to remove specific notes.                                 | C4           |
| 8   | interaction | Remove the note from the list when its delete button is clicked                                                                             | major  | Deletion removes unwanted notes from the interface, maintaining a clean and relevant note collection.         | C7           |
| 9   | content     | Display a priority selector with High, Medium, Low options                                                                                  | major  | Ensures the priority selector provides the required choices so users can categorize items by importance.      | None         |
