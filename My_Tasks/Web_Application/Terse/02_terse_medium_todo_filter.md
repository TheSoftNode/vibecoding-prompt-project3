Category: Web Application

Prompt style: Terse

Title: Todo List with Filtering and Priority

Prompt: Todo list with input and add button. Each todo shows text, priority dropdown (High, Medium, Low), and delete button. Completed todos have strikethrough text. Click todo to toggle completed state. Filter buttons show All, Active, Completed. High priority todos have red left border, Medium yellow, Low green. Counter shows active high-priority count. Each todo displays days since added. Todos older than 7 days with incomplete status show red "Overdue" badge. Progress bar width equals percentage of completed todos.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| ID            | Description                                                                                      | Weight | Rationale                                                                           | Dependent On       |
| ------------- | ------------------------------------------------------------------------------------------------ | ------ | ----------------------------------------------------------------------------------- | ------------------ |
| visual-1      | Render an input field for entering new todo text                                                 | major  | The input field is the primary interface for adding todos.                          | None               |
| visual-2      | Display an add button adjacent to the input field                                                | major  | The add button triggers todo creation from the input value.                         | None               |
| content-1     | Display three filter buttons labeled All, Active, and Completed                                  | major  | Filter buttons enable users to view different subsets of todos.                     | None               |
| interaction-1 | Add a new todo item when the add button is clicked                                               | major  | Adding todos is the core creation functionality of the application.                 | visual-2           |
| content-2     | Display each todo item with its text, priority dropdown, and delete button                       | major  | Todo text, priority, and delete button are the essential elements of each item.     | None               |
| visual-3      | Display priority dropdown with three options: High, Medium, and Low for each todo                | major  | Priority classification enables importance-based task management.                   | content-2          |
| interaction-2 | Remove a todo when its delete button is clicked                                                  | major  | Deletion allows users to remove completed or unwanted tasks.                        | content-2          |
| interaction-3 | Toggle a todo between completed and active states when its text is clicked                       | major  | Click-to-toggle is the specified interaction for changing completion status.        | content-2          |
| visual-4      | Apply strikethrough styling to completed todos                                                   | major  | Strikethrough provides visual distinction between completed and active todos.       | interaction-3      |
| visual-5      | Apply red left border to todos with High priority                                                | major  | Red border provides immediate visual identification of high-priority tasks.         | visual-3           |
| visual-6      | Apply yellow left border to todos with Medium priority                                           | major  | Yellow border distinguishes medium-priority tasks from high and low.                | visual-3           |
| visual-7      | Apply green left border to todos with Low priority                                               | major  | Green border identifies low-priority tasks in the visual hierarchy.                 | visual-3           |
| state-1       | Display only active todos when the Active filter button is clicked                               | major  | Active filter must isolate todos that are not marked as completed.                  | content-1          |
| state-2       | Display only completed todos when the Completed filter button is clicked                         | major  | Completed filter must isolate todos marked as completed.                            | content-1          |
| state-3       | Display all todos when the All filter button is clicked                                          | major  | All filter restores full visibility of the todo list regardless of status.          | content-1          |
| content-3     | Display a counter showing the number of active high-priority todos                               | major  | High-priority active count focuses attention on urgent incomplete tasks.            | None               |
| state-4       | Update the high-priority active counter when todos are added, deleted, toggled, or priority changed | major  | Counter synchronization ensures accuracy across multiple state-changing operations. | content-3          |
| content-4     | Display days since added for each todo                                                           | major  | Days-since-added provides temporal context for task age tracking.                   | None               |
| state-5       | Calculate days since added by comparing todo creation date to current date                       | major  | Days calculation is a time-based derived value requiring date arithmetic.           | content-4          |
| visual-8      | Display red "Overdue" badge on incomplete todos older than 7 days                                | major  | Overdue badge combines age and completion status to identify neglected tasks.       | content-4, interaction-3 |
| state-6       | Show "Overdue" badge only when days since added exceeds 7 and todo is not completed              | major  | Conditional badge display tests compound state logic (age + status).                | visual-8           |
| visual-9      | Display a progress bar                                                                           | major  | Progress bar provides visual representation of overall completion progress.         | None               |
| state-7       | Set progress bar width to percentage of completed todos out of total todos                       | major  | Bar width is derived from completion count divided by total count.                  | visual-9           |
| state-8       | Update progress bar width when todos are added, deleted, or toggled                              | major  | Progress bar synchronization ensures real-time accuracy across state changes.       | state-7            |
