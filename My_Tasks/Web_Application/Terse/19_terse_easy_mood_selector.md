Category: Web_Application

Prompt style: Terse

Title: Emoji Mood Selector

Prompt: Mood selector with 5 emoji buttons: 😊 Happy, 😐 Neutral, 😢 Sad, 😡 Angry, 🤩 Excited. Display buttons horizontally. When user clicks an emoji, show the selected emoji enlarged below the buttons with its mood label. Change background color based on selected mood: green for Happy, gray for Neutral, blue for Sad, red for Angry, yellow for Excited.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display 😊 button with "Happy" label                  | major  | Users need to see the happy mood option.                                                                         | None         |
| 2   | content     | Display 😐 button with "Neutral" label                | major  | Users need to see the neutral mood option.                                                                       | None         |
| 3   | content     | Display 😢 button with "Sad" label                    | major  | Users need to see the sad mood option.                                                                           | None         |
| 4   | content     | Display 😡 button with "Angry" label                  | major  | Users need to see the angry mood option.                                                                         | None         |
| 5   | content     | Display 🤩 button with "Excited" label                | major  | Users need to see the excited mood option.                                                                       | None         |
| 6   | layout      | Position 5 emoji buttons horizontally                 | minor  | Horizontal layout makes all mood options visible in a row.                                                       | None         |
| 7   | interaction | Show selected emoji enlarged when button is clicked   | major  | Clicking an emoji displays it larger to confirm the selection.                                                   | None         |
| 8   | content     | Display mood label below enlarged emoji               | minor  | The label tells users which mood they selected.                                                                  | None         |
| 9   | visual      | Change background to green for Happy selection        | major  | Green background reinforces the happy mood visually.                                                             | None         |
| 10  | visual      | Change background to gray for Neutral selection       | major  | Gray background reinforces the neutral mood visually.                                                            | None         |
| 11  | visual      | Change background to blue for Sad selection           | major  | Blue background reinforces the sad mood visually.                                                                | None         |
| 12  | visual      | Change background to red for Angry selection          | major  | Red background reinforces the angry mood visually.                                                               | None         |
| 13  | visual      | Change background to yellow for Excited selection     | major  | Yellow background reinforces the excited mood visually.                                                          | None         |
| 14  | state       | Track currently selected mood                         | major  | Tracking selection maintains which mood is active.                                                               | None         |
| 15  | layout      | Position enlarged emoji below buttons                 | minor  | Placing selection below keeps the options visible above.                                                         | None         |

## Justification

The emoji mood selector works exactly as expected with visual mood feedback. Five emoji buttons display horizontally across the screen: 😊 Happy, 😐 Neutral, 😢 Sad, 😡 Angry, and 🤩 Excited. When users click an emoji button, the selected emoji appears enlarged below the buttons with its mood label displayed underneath. The background color changes based on the selected mood: green for Happy, gray for Neutral, blue for Sad, red for Angry, and yellow for Excited. The color-coded backgrounds provide immediate visual reinforcement of the selected emotional state.
