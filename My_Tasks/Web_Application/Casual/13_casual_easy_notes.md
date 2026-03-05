Category: Web Application

Prompt style: Casual

Title: Quick Notes App

Prompt: Notes app, keep it simple. Type note, click add, shows up in list. Each note gets a timestamp. Click note to edit inline. Delete button on each. That's it.

Required libraries: react, tailwindcss

## Rubric

| ID            | Description                                              | Weight | Rationale                                                                    | Dependent On |
| ------------- | -------------------------------------------------------- | ------ | ---------------------------------------------------------------------------- | ------------ |
| visual-1      | Render a text input or text area for typing notes        | major  | Input field is the primary interface for note creation.                      | None         |
| visual-2      | Display an add button                                    | major  | Add button triggers note creation.                                           | None         |
| interaction-1 | Add a new note to the list when the add button is clicked | major  | Note addition is the core creation interaction.                              | visual-2     |
| content-1     | Display each note in a list                              | major  | List display organizes notes for viewing.                                    | None         |
| content-2     | Display a timestamp for each note                        | major  | Timestamps provide temporal context for each note.                           | content-1    |
| interaction-2 | Enable inline editing when a note is clicked             | major  | Click-to-edit provides direct manipulation for note modification.            | content-1    |
| visual-3      | Display a delete button for each note                    | major  | Delete button enables note removal.                                          | content-1    |
| interaction-3 | Remove the note when its delete button is clicked        | major  | Deletion allows users to remove unwanted notes.                              | visual-3     |
