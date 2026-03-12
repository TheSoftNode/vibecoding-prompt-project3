Category: Web_Application

Prompt style: Feature_List

Title: Keyboard Shortcut Trainer

Prompt: Build a keyboard shortcut trainer. Display a random action name from a predefined list of 10 common actions (like "Save File", "Undo", "Copy", "Paste", "Cut", "Select All", "New Tab", "Close Tab", "Refresh", "Find"). Below the action name, show a text prompt saying "Press the correct keyboard shortcut". Detect the key combination pressed by the user and compare it to the correct shortcut. If correct, display a green checkmark with the message "Correct!". If wrong, display a red X with the message "Wrong! The correct shortcut is" followed by the actual shortcut in bold. Show a "Next" button to load another random action.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | state       | Select random action from predefined list of 10           | major  | Randomly picking an action keeps the trainer unpredictable and challenging.                                      | None         |
| 2   | content     | Display random action name                                | major  | Showing the action tells users which shortcut they need to press.                                                | C1           |
| 3   | content     | Display prompt "Press the correct keyboard shortcut"      | minor  | The prompt instructs users what to do next.                                                                      | None         |
| 4   | interaction | Detect key combination pressed by user                    | major  | Detecting keypresses captures what combination the user typed.                                                   | None         |
| 5   | state       | Compare pressed keys to correct shortcut                  | major  | Comparing determines if the user got the answer right or wrong.                                                  | C4           |
| 6   | visual      | Display green checkmark when correct                      | major  | The green checkmark gives visual confirmation of success.                                                        | C5           |
| 7   | content     | Display message "Correct!" when right                     | minor  | The message reinforces the positive feedback for correct answers.                                                | C5           |
| 8   | visual      | Display red X when wrong                                  | major  | The red X gives visual feedback that the answer was incorrect.                                                   | C5           |
| 9   | content     | Display message "Wrong! The correct shortcut is" when incorrect | minor | The message introduces the correct answer after a mistake.                                                  | C5           |
| 10  | content     | Display actual shortcut in bold after wrong answer        | major  | Showing the correct shortcut teaches users what they should have pressed.                                        | C5           |
| 11  | visual      | Display "Next" button                                     | major  | The button lets users move on to another random action.                                                          | None         |
| 12  | interaction | Load new random action when "Next" is clicked             | major  | Clicking Next refreshes the challenge with a different action.                                                   | None         |

## Justification

The keyboard shortcut trainer works exactly as expected with random action challenges and keystroke detection. A random action name displays from a predefined list of 10 common actions like "Save File", "Undo", "Copy", "Paste", "Cut", "Select All", "New Tab", "Close Tab", "Refresh", and "Find". Below the action name, a prompt displays saying "Press the correct keyboard shortcut". When users press a key combination, the tool detects the keypress and compares it to the correct shortcut. If correct, a green checkmark appears with the message "Correct!". If wrong, a red X appears with the message "Wrong! The correct shortcut is" followed by the actual shortcut displayed in bold. A "Next" button displays that loads another random action when clicked.
