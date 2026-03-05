Scheduling Board
Scheduling board
Difficulty
Hard
Category
Management System
Style
Detailed Specification
Length
Detailed
Prompt
Build a web application that serves as a visual scheduling board. The board needs to support assigning tasks to a fixed number of workers on a variable horizontal timeline. The unscheduled tasks appear in unscheduled panel labeled "Unscheduled Tasks". The user may drag and drop a task onto a worker's horizontal timeline (labeled with worker number) and assign it to that worker. Each worker has its own row. The horizontal drop position determines the start time. Each task is represented by a horizontal block representing the task time interval. The block starts at start time (relative to timeline) and ends at end time = start time + duration of the task. Each task block should contain a task name and time range (example: "First task": [2-6]). If the task name and duration text is longer than the block width, clip the text and add "..." to fit into the block (example: Tas...).
When dropping a task, if it overlaps with lower priority tasks on that worker, the higher priority task replaces them. The displaced lower priority tasks return to the unscheduled panel. If overlapping tasks have equal or higher priority, reject the drop and return the dragged task to unscheduled panel. A drag and drop is also rejected if the remaining timeline space is insufficient (extends beyond timeline end). The user must be able to drag and drop an already scheduled task to another worker or different time slot.
Additionally, each task may require a global GPU resource. If two tasks requiring GPU are overlapping in time, even if distributed to different workers, they should be highlighted red.
Timeline duration is adjustable and should have a scale displayed. If the timeline is extended, add additional time at the end and keep the already scheduled tasks in the board. If the duration is shortened and this causes some tasks to extend beyond timeline end, return them to unscheduled panel.
Initially the timeline spans from time 0 to 12 and we have 2 workers. The initial tasks are "First task" - duration 4, priority 3, requires GPU "Second task" - duration 3, priority 2 "Third task" - duration 5, priority 1 "Fourth task with long name" - duration 2, priority 3, requires GPU "Fifth task" - duration 1, priority 1 "Sixth task" - duration 6, priority 2
The initial attempted assignment is: Worker 1: "Third task": [0-5], "Second task": [5-8], "Fourth task": [5-7], "Fifth task": [0-1] Worker 2: "First task": [2-6], "Sixth task": [7-13]
Initial attempted assignment should first be processed for conflicts and be resolved by the rules of priority swapping. The feasible schedule should then already be rendered on the board on page load.
Required Libraries

Rubric

| ID            | Description                                                                                                                                                    | Weight | Rationale                                                                                                     | Dependent On  |
| ------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------- | ------------- |
| layout-1      | Display an "Unscheduled Tasks" panel and one horizontal timeline row per worker, each worker row labeled distinctly                                            | major  | Core board structure must exist before any scheduling logic can be evaluated.                                 | None          |
| interaction-1 | Enable assigning a task to a worker at a specific time by dragging and dropping a task from the unscheduled panel or from the timeline to a new time or worker | major  | Task assignment must occur through drag and drop interaction.                                                 | None          |
| layout-2      | Render scheduled tasks as horizontal blocks placed on timeline at start time and whose width corresponds to their duration                                     | major  | Visual width must reflect the duration of task.                                                               | None          |
| state-1       | Compute end time as start time plus task duration                                                                                                              | minor  | Task interval start and end times must match the duration and assigned time.                                  | None          |
| content-1     | Display task name and time range inside each scheduled task block in format "Name": [start-end] (example: "First task: [2-6]")                                 | minor  | Time labels enable verification of scheduling correctness.                                                    | state-1       |
| visual-1      | Clip task text and append "..." when and only when the text would overflow because of small block width                                                        | minor  | Text overflow handling is required.                                                                           | None          |
| state-2       | Replace the task when dropping a task that overlaps lower priority tasks on the same worker or reject the drop otherwise                                       | major  | Worker and priority constraint must be enforced.                                                              | None          |
| state-3       | Return displaced lower priority tasks or rejected tasks to the unscheduled panel                                                                               | major  | The displaced or rejected tasks must remain available.                                                        | None          |
| state-4       | Reject a drop when the task interval extends beyond the timeline end                                                                                           | major  | Tasks must fit entirely within timeline bounds.                                                               | None          |
| state-5       | Highlight overlapping tasks that require the GPU across different workers with red                                                                             | major  | Need to detect global resource constraint violation.                                                          | None          |
| interaction-2 | Allow changing the timeline end value                                                                                                                          | major  | Timeline duration must be user adjustable to test the behavior when extending or shortening the timeline end. | None          |
| state-6       | Extend the timeline when the duration increases without altering existing scheduled tasks                                                                      | major  | Timeline expansion must preserve valid assignments.                                                           | interaction-2 |
| state-7       | Return tasks to the unscheduled panel when timeline shortening causes them to exceed the new end                                                               | major  | Tasks must remain within bounds after resizing.                                                               | interaction-2 |
| layout-3      | Display a visible horizontal time scale from 0 to the current timeline end value                                                                               | minor  | Required to visually interpret start/end times and drop positions.                                            | None          |

ID
Description
Weight
Rationale
Dependent On
layout-1
Display an "Unscheduled Tasks" panel and one horizontal timeline row per worker, each worker row labeled distinctly
major
Core board structure must exist before any scheduling logic can be evaluated.
None
interaction-1
Enable assigning a task to a worker at a specific time by dragging and dropping a task from the unscheduled panel or from the timeline to a new time or worker
major
Task assignment must occur through drag and drop interaction.
None
layout-2
Render scheduled tasks as horizontal blocks placed on timeline at start time and whose width corresponds to their duration
major
Visual width must reflect the duration of task.
None
state-1
Compute end time as start time plus task duration
minor
Task interval start and end times must match the duration and assigned time.
None
content-1
Display task name and time range inside each scheduled task block in format "Name": [start-end] (example: "First task: [2-6]")
minor
Time labels enable verification of scheduling correctness.
state-1
visual-1
Clip task text and append "..." when and only when the text would overflow because of small block width
minor
Text overflow handling is required.
None
state-2
Replace the task when dropping a task that overlaps lower priority tasks on the same worker or reject the drop otherwise
major
Worker and priority constraint must be enforced.
None
state-3
Return displaced lower priority tasks or rejected tasks to the unscheduled panel
major
The displaced or rejected tasks must remain available.
None
state-4
Reject a drop when the task interval extends beyond the timeline end
major
Tasks must fit entirely within timeline bounds.
None
state-5
Highlight overlapping tasks that require the GPU across different workers with red
major
Need to detect global resource constraint violation.
None
interaction-2
Allow changing the timeline end value
major
Timeline duration must be user adjustable to test the behavior when extending or shortening the timeline end.
None
state-6
Extend the timeline when the duration increases without altering existing scheduled tasks
major
Timeline expansion must preserve valid assignments.
interaction-2
state-7
Return tasks to the unscheduled panel when timeline shortening causes them to exceed the new end
major
Tasks must remain within bounds after resizing.
interaction-2
layout-3
Display a visible horizontal time scale from 0 to the current timeline end value
minor
Required to visually interpret start/end times and drop positions.
None
