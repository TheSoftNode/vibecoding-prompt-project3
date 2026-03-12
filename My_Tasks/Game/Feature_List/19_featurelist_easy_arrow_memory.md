Category: Game

Prompt style: Feature_List

Title: Arrow Pattern Memory

Prompt: Build an arrow pattern memory game. Display a "Start Round" button that begins a new round. When clicked, show a sequence of 4 random arrow symbols (↑ → ↓ ←) on screen for 3 seconds, then hide the sequence. After hiding, display a prompt saying "Type the pattern using arrow keys". Detect arrow key presses from the user and compare the typed sequence to the original pattern. If correct, display "Success!" in green and increment the score. If wrong, display "Failed!" in red and show the correct sequence. Display a counter showing current score.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display "Start Round" button                              | major  | The button lets users begin a new memory challenge.                                                              | None         |
| 2   | state       | Generate random sequence of 4 arrow symbols               | major  | Random patterns keep each round different and unpredictable.                                                     | None         |
| 3   | content     | Display arrow symbols (↑ → ↓ ←) on screen                 | major  | Showing arrows tells users what pattern to memorize.                                                             | C2           |
| 4   | state       | Show sequence for 3 seconds then hide                     | major  | Timed display tests users' memory by removing the pattern after a short viewing window.                          | None         |
| 5   | content     | Display prompt "Type the pattern using arrow keys"        | minor  | The prompt instructs users what to do after the sequence hides.                                                  | None         |
| 6   | interaction | Detect arrow key presses from user                        | major  | Detecting keypresses captures the sequence the user types.                                                       | None         |
| 7   | state       | Compare typed sequence to original pattern                | major  | Comparing determines if the user remembered the pattern correctly.                                               | C6           |
| 8   | content     | Display "Success!" in green when correct                  | major  | Green success message gives positive feedback for correct answers.                                               | C7           |
| 9   | state       | Increment score when correct                              | major  | Increasing the score rewards users for successful pattern recall.                                                | C7           |
| 10  | content     | Display "Failed!" in red when wrong                       | major  | Red failure message gives feedback that the answer was incorrect.                                                | C7           |
| 11  | content     | Show correct sequence after failure                       | minor  | Revealing the pattern teaches users what they should have typed.                                                 | C7           |
| 12  | content     | Display counter showing current score                     | minor  | The score counter shows users how many rounds they've completed successfully.                                    | C9           |

## Justification

The arrow pattern memory game works exactly as expected with timed sequence display and keyboard input detection. A "Start Round" button displays on screen. When clicked, a random sequence of 4 arrow symbols (↑ → ↓ ←) appears on screen for 3 seconds, then hides automatically. After hiding, a prompt displays saying "Type the pattern using arrow keys". The game detects arrow key presses from the user and compares the typed sequence to the original pattern. If correct, "Success!" displays in green and the score increments by one. If wrong, "Failed!" displays in red along with the correct sequence revealed. A counter displays showing the current score, tracking how many rounds the user has completed successfully.
