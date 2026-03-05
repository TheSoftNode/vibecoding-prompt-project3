Rubric Guidelines
Technical Requirements for Rubrics
A high-quality rubric provides a list of atomic, tagged criteria used to grade the model’s output effectively. Use the following standards to ensure consistency across all tasks.

⚙️ Core Requirements
Quantity: Each rubric must contain 8 - 20 (strongly preferred If a rubric exceeds 20 items, prioritize and reduce wherever possible (unless it’s genuinely impossible to do so).
Balance: Include enough checks to cover all critical behaviors without over‑penalizing minor issues.
Verifiability: Every item must be verifiable from either a static screenshot or the provided code.

🏷️ Rubric Tags

| Tag             | Focus Area                                                                                                                                                                                                    | Verification Method         |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------- |
| **visual**      | Tag visual when the rubric concerns an element's existence and/or looks (color, styling, visual emphasis) and can be verified from the screenshot without interpreting text or considering relative position. | Screenshot (Initial Render) |
| **layout**      | Tag layout when the rubric concerns the spatial placement or alignment of elements relative to each other.                                                                                                    | Screenshot or Code          |
| **content**     | Tag content when the rubric concerns the exact text, labels, numbers, or data values displayed to the user, independent of how or where they appear.                                                          | Screenshot or Code          |
| **interaction** | Tag interaction when the rubric concerns a user action (click, type, drag, gesture) and what immediately happens as a result of that action.                                                                  | Code Review                 |
| **state**       | Tag state when the rubric concerns data or application state changing or persisting over time, regardless of how the change is visually presented.                                                            | Code Review                 |

Tags specify which aspect of the application is being evaluated and how it will be verified.
Tag
Focus Area
Verification Method
visual
Tag visual when the rubric concerns an element's existence and/or looks (color, styling, visual emphasis) and can be verified from the screenshot without interpreting text or considering relative position.
Screenshot (Initial Render)
layout
Tag layout when the rubric concerns the spatial placement or alignment of elements relative to each other.
Screenshot or Code
content
Tag content when the rubric concerns the exact text, labels, numbers, or data values displayed to the user, independent of how or where they appear.
Screenshot or Code
interaction
Tag interaction when the rubric concerns a user action (click, type, drag, gesture) and what immediately happens as a result of that action.
Code Review
state
Tag state when the rubric concerns data or application state changing or persisting over time, regardless of how the change is visually presented.
Code Review

📣 Important: Visual Tag Usage
All rubric criteria tagged as visual must be verifiable from a screenshot of the initial load view.
If the application would otherwise render a blank or empty view on initial load, you must explicitly specify pre-loaded sample data in the prompt so that visual elements are present and evaluable.
Examples
Tables or lists: On initial load, render a table pre-populated with at least 5 sample rows using placeholder data.
Cards or grids: On initial load, display a grid of 6 sample product cards, each with a title, price, and image, using mock data.
Charts or visualizations: On initial load, render a bar chart using predefined sample data (e.g., values for Jan–Jun).

⚖️ Weight
Assign weights to distinguish between critical requirements and supplementary features:
major: Critical or core functionality that is essential to the task's success.
minor: "Nice-to-have" functionality or secondary aesthetic details.

🔗 dependent_on
This field contains a list of IDs for criteria that MUST be checked before the current criterion can be evaluated.
Usage: Only use this if a criterion cannot be understood or met without the successful evaluation of other prerequisites.
Logic: For example, you cannot check if "Score updates on click" (state) if the "Score display exists" (content) has failed.

Quality requirements for description:
Clear and unambiguous
Use precise language so the pass/fail condition is obvious. Avoid vague descriptions. Instead specify the exact action and expected outcome.
Forbidden words: correctly, properly, appropriately, clearly, adequately, thoroughly (and similar)
❌ BAD (vague):
Countdown works correctly
✅ GOOD (specific):
Start button begins countdown
Self‑contained
Provide enough context within the item so it can be evaluated on its own without referencing other rubric items or external knowledge.
❌ BAD (vague):
Centered
✅ GOOD (self-contained):
Display center timer on the page
Task-specific
Tie the item to the unique features of your prompt.
❌ BAD (generic, can be used in almost every task):
Includes a button
✅ GOOD (specific):
Reset button returns timer to 25:00
Non‑stacked
Do not bundle multiple expectations into one item. Separate them into independent checks unless the behaviours are inseparable.
❌ BAD (stacked):
Start and pause the timer
✅ GOOD (non-stacked, 2 different descriptions):
Begin countdown when the Start button is clicked

Stop countdown without resetting when the Pause button is clicked
Appropriately flexible
Allow for different valid implementations. Avoid enforcing a particular solution when multiple approaches are acceptable.
❌ BAD (not-flexible):
Use a table element for tasks
✅ GOOD (flexible):
Display tasks in a list or table
Verifiable
Focus on observable behavior. Items should test the rendered output or the code, not the model’s internal reasoning.
❌ BAD (unverifiable):
Keep track of score internally
✅ GOOD (verifiable):
Show current score near the board
Comprehensive
Ensure that every explicit requirement in the prompt is covered by at least one rubric item.
Example requirement: The score should be displayed near the board
❌ BAD (generic, can be used in almost every task):
Omitting a requirement (e.g., no check for the scoreboard)
✅ GOOD (requirements are included):
Display the current score near the board
Non‑redundant
Avoid overlapping or duplicative checks. Each item should evaluate a distinct aspect of the response.
❌ BAD (redundant):
// criteria-1
Show current score

// criteria-2
Display score on screen
✅ GOOD: Only one check is needed
// criteria-1
Display score on screen```
Action word usage
Begin each rubric item with a concrete action verb in the present tense (e.g., “Display,” “Position,” “Animate,” “Count,” “Start”). This signals exactly what the model must do and improves consistency.
❌ BAD (not-actionable):
Countdown displays in MM:SS format
✅ GOOD (actionable):
Display countdown in MM:SS format
Checkable from screenshot + code
The vision‑language model must be able to verify each item from the screenshot or by reading the code.
❌ BAD (not-checkable):
Ensure the user data is correctly saved to the production database

The page should load very quickly
✅ GOOD (checkable):
Display the current score near the board
Quality requirements for rationale:
Rationale must:
Explain WHY the criterion matters (not just restate description)
Be aligned with the description
Contains no factual errors
Be specific to this task
❌ Rationale shouldn’t:
Refer to the agent (e.g, the agent may assume…)
Refer to the specific implementation (e.g, during development, it was not clear that …)
Be generic (e.g, Because this is important. <= end of rationale)
Expose implementation details/hints (e.g … the newly implemented methods should throw an error silently ...)
❌ BAD rationale:
This is important for correctness (too generic)
Agent should clarify this (restates description)
✅ GOOD rationale:
Correctly renders solid balls according to standard pool ball appearance.```
