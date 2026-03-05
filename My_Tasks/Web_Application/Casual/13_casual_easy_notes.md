Category: Web Application

Prompt style: Casual

Title: Quick Notes App

Prompt: Notes app with priorities. Type note, pick priority (High, Medium, Low), click add. List shows note with colored dot - red for High, yellow for Medium, green for Low. Timestamp on each. Click note to edit inline. Top-right corner shows two counters: total notes and how many are High priority. On load, show 3 sample notes: one High with red dot, one Medium with yellow dot, one Low with green dot.

Required libraries: react, tailwindcss

## Rubric

| ID            | Description                                              | Weight | Rationale                                                                    | Dependent On |
| ------------- | -------------------------------------------------------- | ------ | ---------------------------------------------------------------------------- | ------------ |
| visual-1      | Render a text input for typing notes and a priority selector with High, Medium, Low options        | major  | Text input and priority selector (High, Medium, Low) are explicitly required for note creation workflow.                      | None         |
| visual-2      | Display an add button                                    | major  | Add button explicitly triggers note creation as specified in prompt.                                           | None         |
| interaction-1 | Add a new note with selected priority to the list when the add button is clicked | major  | User clicking add button triggers note creation with priority as specified in prompt.                              | visual-2     |
| content-1     | Display each note in a list with its text content and timestamp                              | major  | List display of note text and "Timestamp on each" are explicitly required in prompt.                                    | None         |
| state-1      | Display red colored dot for High priority notes, yellow colored dot for Medium priority notes, and green colored dot for Low priority notes                    | major  | Conditional colored dot rendering (red for High, yellow for Medium, green for Low) explicitly specified in prompt.                                          | content-1    |
| interaction-2 | Enable inline editing when a note is clicked             | major  | Click-to-edit interaction "Click note to edit inline" explicitly specified in prompt.            | content-1    |
| layout-1      | Position two counters in the top-right corner showing total notes count and High priority notes count | major  | Prompt explicitly requires "Top-right corner shows two counters: total notes and how many are High priority."                              | None     |
| state-2       | Update the total notes counter to reflect the current number of notes in the list        | major  | Total notes counter must dynamically update as notes are added or deleted.                                   | layout-1     |
| state-3       | Update the High priority counter to show count of notes where priority is High               | major  | High priority counter filters and counts only High priority notes as explicitly specified in prompt.                              | layout-1     |
| content-2     | Display 3 sample notes on initial load with one High priority note showing red dot, one Medium priority note showing yellow dot, and one Low priority note showing green dot                        | major  | Prompt explicitly requires "On load, show 3 sample notes: one High with red dot, one Medium with yellow dot, one Low with green dot."                           | None    |
| visual-3      | Display a delete button for each note                    | minor  | Delete button provides note removal capability.                                          | content-1    |
| interaction-3 | Remove the note from the list when its delete button is clicked        | minor  | Delete interaction removes notes from the list.                                   | visual-3     |
