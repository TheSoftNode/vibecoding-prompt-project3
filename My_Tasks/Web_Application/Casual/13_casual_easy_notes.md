Category: Web Application

Prompt style: Casual

Title: Quick Notes App

Prompt: Notes app with priorities. Type note, pick priority (High, Medium, Low), click add. List shows note with colored dot next to the text - red for High, yellow for Medium, green for Low. Timestamp on each. Click note to edit inline. Delete button on each. On load, show 3 sample notes: one High with red dot, one Medium with yellow dot, one Low with green dot.

Required libraries: react, tailwindcss

## Rubric

| #  | ID            | Description                                              | Weight | Rationale                                                                    | Dependent On |
| -- | ------------- | -------------------------------------------------------- | ------ | ---------------------------------------------------------------------------- | ------------ |
| 1  | visual-1      | Render a text input for typing notes and a priority selector with High, Medium, Low options        | major  | Text input and priority selector (High, Medium, Low) are explicitly required by prompt for note creation workflow.                      | None         |
| 2  | visual-2      | Display an add button                                    | major  | Add button explicitly required by prompt to trigger note creation.                                           | None         |
| 3  | interaction-1 | Add a new note with selected priority to the list when the add button is clicked | major  | User clicking add button triggers note creation with priority as explicitly specified in prompt.                              | visual-2     |
| 4  | content-1     | Display each note in a list with its text content and timestamp                              | major  | List display of note text and "Timestamp on each" are explicitly required by prompt.                                    | None         |
| 5  | state-1      | Display red colored dot for High priority notes, yellow colored dot for Medium priority notes, and green colored dot for Low priority notes                    | major  | Conditional colored dot rendering (red for High, yellow for Medium, green for Low) explicitly specified in prompt.                                          | content-1    |
| 6  | layout-1     | Position the colored dot next to the note text             | minor  | Prompt explicitly requires colored dot positioned "next to the text" for priority visibility.            | state-1    |
| 7  | interaction-2 | Enable inline editing when a note is clicked             | major  | Click-to-edit interaction "Click note to edit inline" explicitly specified in prompt.            | content-1    |
| 8  | visual-3      | Display a delete button for each note                    | major  | Delete button "Delete button on each" explicitly required by prompt for note removal.                                          | content-1    |
| 9  | interaction-3 | Remove the note from the list when its delete button is clicked        | major  | Delete interaction removes notes from the list as required by prompt.                                   | visual-3     |
| 10 | content-2     | Display 3 sample notes on initial load with one High priority note showing red dot, one Medium priority note showing yellow dot, and one Low priority note showing green dot                        | major  | Prompt explicitly requires "On load, show 3 sample notes: one High with red dot, one Medium with yellow dot, one Low with green dot."                           | None    |
