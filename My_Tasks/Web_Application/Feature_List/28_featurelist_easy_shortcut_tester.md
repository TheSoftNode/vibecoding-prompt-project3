Category: Web_Application

Prompt style: Feature_List

Title: Keyboard Shortcut Practice Tool

Prompt: Build a keyboard shortcut practice tool. Display a target shortcut at the top showing a combination like "Ctrl + S", "Ctrl + C", or "Ctrl + V". Show instruction text "Press the shortcut to continue". Display a score counter starting at 0. When the user presses the correct key combination, increment the score by 1 and immediately show a new random shortcut from the three options. If the user presses any wrong key, display "Wrong key! Try again" in red text for 2 seconds without changing the target shortcut or score.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display target shortcut at top                       | major  | The target shows users which key combination to press.                                       | None         |
| 2   | state       | Show one of Ctrl+S, Ctrl+C, or Ctrl+V as target     | major  | These three shortcuts provide the practice challenges.                                       | None         |
| 3   | content     | Display instruction "Press the shortcut to continue" | minor  | The instruction guides users on what action to take.                                         | None         |
| 4   | content     | Display score counter                                | major  | The counter shows users how many shortcuts they've completed correctly.                      | None         |
| 5   | state       | Initialize score to 0                                | minor  | Starting at zero gives users a baseline for tracking progress.                               | None         |
| 6   | interaction | Detect when user presses keys                        | major  | Key detection captures user input for comparison with the target shortcut.                   | None         |
| 7   | state       | Check if pressed keys match target shortcut          | major  | Matching validates whether the user pressed the correct combination.                         | C6           |
| 8   | state       | Increment score by 1 when correct                    | major  | Increasing score rewards users for correct shortcut execution.                               | C7           |
| 9   | content     | Update displayed score after increment               | minor  | Showing the new score gives users immediate feedback on their progress.                      | C8           |
| 10  | state       | Select new random shortcut from three options        | major  | Randomizing keeps the practice varied and prevents memorization of sequence.                 | C7           |
| 11  | content     | Display new shortcut immediately after correct press | major  | Showing the next challenge maintains the practice flow without delay.                        | C10          |
| 12  | content     | Display "Wrong key! Try again" when incorrect        | major  | Error message tells users they pressed the wrong keys.                                       | C7           |
| 13  | visual      | Show error message in red text                       | minor  | Red color emphasizes the error visually.                                                     | C12          |
| 14  | state       | Hide error message after 2 seconds                   | minor  | Auto-hiding the message clears the screen for the next attempt.                              | C12          |
| 15  | state       | Keep target shortcut unchanged when wrong key pressed| major  | Maintaining the same target lets users retry the same shortcut challenge.                    | C7           |
| 16  | state       | Keep score unchanged when wrong key pressed          | major  | Not incrementing score for errors ensures only correct presses count.                        | C7           |

## Justification

The keyboard shortcut practice tool works exactly as expected for training key combinations. A target shortcut displays at the top showing one of "Ctrl + S", "Ctrl + C", or "Ctrl + V". Below it, instruction text reads "Press the shortcut to continue" with a score counter starting at 0. When users press the correct key combination, the score increments by 1 and a new random shortcut from the three options immediately displays. If users press any wrong key, "Wrong key! Try again" appears in red text for 2 seconds while the target shortcut and score remain unchanged, allowing users to retry.
