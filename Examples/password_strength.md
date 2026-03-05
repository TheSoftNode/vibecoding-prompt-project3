Password Strength
Password strength checker
Difficulty
Easy
Category
Quick Tools
Style
Feature List
Length
Detailed
Prompt
Build a password strength checker interface with a text input and a strength indicator on top of the text input.
The indicator should be updated on every input change:
if the text length is 0 to 5 characters, set the indicator color to red and display the text "Weak"
if the text length is 6 to 8 characters, set the indicator color to orange and display the text "Medium"
if the text length is greater than 8 characters and contains at least one special character (non letter or digit), set the indicator color to green and display the text "Strong" Implement a "Save" button next to the text input. This button should save and display the current password in a text format below the text input. Only the last 5 saved passwords should be displayed.
On load the text input should be blank and the indicator should be red with a text "Weak".
Required Libraries
react, vanilla javascript
Rubric

| ID            | Description                                                                                                                              | Weight | Rationale                                                                                       | Dependent On |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------- | ------------ |
| visual-1      | Render a single password text input field                                                                                                | major  | The input field is the core UI element required for evaluating password strength.               | None         |
| layout-1      | Display a strength indicator on top of the text input                                                                                    | minor  | Positioning the strength indicator near the input provides immediate visual feedback context.   | None         |
| state-1       | Initialize the input text as empty on page load                                                                                          | major  | A default empty state ensures predictable behavior on first user interaction.                   | visual-1     |
| state-2       | Initialize the indicator to red with the text "Weak" on page load                                                                        | major  | A default indicator state provides a predictable baseline before user input.                    | layout-1     |
| state-3       | Apply a red color and display the text "Weak" when the input length is between 0 and 5 characters                                        | major  | Red color and "Weak" text visually signal insufficient password strength.                       | visual-1     |
| state-4       | Apply an orange color and display the text "Medium" when the input length is between 6 and 8 characters                                  | major  | Orange color and "Medium" text visually signal partial password strength.                       | visual-1     |
| state-5       | Apply a green color and display the text "Strong" when the input length exceeds 8 characters and contains at least one special character | major  | Green color and "Strong" text visually signal that the password satisfies strength constraints. | visual-1     |
| interaction-1 | Update the indicator color and text on every user input event                                                                            | major  | Real-time feedback allows the user to evaluate password strength while typing.                  | visual-1     |
| layout-2      | Render a Save button next to the password input field                                                                                    | major  | The Save button enables the password history feature.                                           | None         |
| interaction-2 | Save the current password value and display it below the input when the "Save" button is clicked                                         | major  | Persisting and displaying passwords helps users manage and review saved values.                 | layout-2     |
| state-6       | Limit the displayed saved password list to the five most recent entries                                                                  | major  | Limiting history size prevents uncontrolled growth and maintains a clean interface.             | None         |
| content-2     | Display saved passwords in reverse order, with the most recent at the top                                                                | minor  | Showing recent passwords first improves accessibility to the latest entries.                    | None         |

ID
Description
Weight
Rationale
Dependent On
visual-1
Render a single password text input field
major
The input field is the core UI element required for evaluating password strength.
None
layout-1
Display a strength indicator on top of the text input
minor
Positioning the strength indicator near the input provides immediate visual feedback context.
None
state-1
Initialize the input text as empty on page load
major
A default empty state ensures predictable behavior on first user interaction.
visual-1
state-2
Initialize the indicator to red with the text "Weak" on page load
major
A default indicator state provides a predictable baseline before user input.
layout-1
state-3
Apply a red color and display the text "Weak" when the input length is between 0 and 5 characters
major
Red color and "Weak" text visually signal insufficient password strength.
visual-1
state-4
Apply an orange color and display the text "Medium" when the input length is between 6 and 8 characters
major
Orange color and "Medium" text visually signal partial password strength.
visual-1
state-5
Apply a green color and display the text "Strong" when the input length exceeds 8 characters and contains at least one special character
major
Green color and "Strong" text visually signal that the password satisfies strength constraints.
visual-1
interaction-1
Update the indicator color and text on every user input event
major
Real-time feedback allows the user to evaluate password strength while typing.
visual-1
layout-2
Render a Save button next to the password input field
major
The Save button enables the password history feature.
None
interaction-2
Save the current password value and display it below the input when the "Save" button is clicked
major
Persisting and displaying passwords helps users manage and review saved values.
layout-2
state-6
Limit the displayed saved password list to the five most recent entries
major
Limiting history size prevents uncontrolled growth and maintains a clean interface.
None
content-2
Display saved passwords in reverse order, with the most recent at the top
minor
Showing recent passwords first improves accessibility to the latest entries.
None
