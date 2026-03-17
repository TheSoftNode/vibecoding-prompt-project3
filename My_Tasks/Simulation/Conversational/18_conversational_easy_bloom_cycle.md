Category: Simulation

Prompt style: Conversational

Title: Bioluminescence Bloom Cycle

Prompt: I need an animated bioluminescence bloom simulation. Display three circles stacked vertically representing coral, algae, and plankton organisms with labels "Coral", "Algae", and "Plankton" below each circle. Start with coral glowing. After 4 seconds, switch to plankton glowing. After 3 seconds, switch to algae glowing. After 2 seconds, switch back to coral. Cycle continuously. Include a pause button that stops the cycle when clicked and resumes when clicked again.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                   | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display circle for coral organism                             | major  | The coral circle is the top organism in the bloom sequence showing the first glow state.                         | None         |
| 2   | visual      | Display circle for algae organism                             | major  | The algae circle is the middle organism showing the third glow state.                                            | None         |
| 3   | visual      | Display circle for plankton organism                          | major  | The plankton circle is the bottom organism showing the second glow state.                                        | None         |
| 4   | layout      | Stack three circles vertically                                | minor  | Vertical stacking creates the organism sequence from top to bottom: coral, algae, plankton.                      | None         |
| 5   | content     | Display labels "Coral", "Algae", "Plankton" below circles     | major  | Labels identify which organism each circle represents.                                                           | C1, C2, C3   |
| 6   | layout      | Position labels below each corresponding circle               | minor  | Below positioning associates each label with its organism circle.                                                | C5           |
| 7   | state       | Start with coral glowing                                      | minor  | Starting with coral establishes the initial state of the bloom cycle.                                            | None         |
| 8   | state       | Switch from coral to plankton after 4 seconds                 | major  | The 4-second coral duration sets the first phase timing before transitioning to plankton.                        | None         |
| 9   | state       | Switch from plankton to algae after 3 seconds                 | major  | The 3-second plankton duration gives the second phase time before moving to algae.                               | None         |
| 10  | state       | Switch from algae to coral after 2 seconds                    | major  | The 2-second algae duration provides the brief third phase before returning to start.                            | None         |
| 11  | state       | Cycle continuously through coral-plankton-algae-coral sequence| major  | Continuous cycling maintains the ongoing bloom simulation indefinitely.                                          | None         |
| 12  | visual      | Display pause button                                          | major  | The pause button provides the control for stopping and resuming the cycle.                                       | None         |
| 13  | interaction | Stop cycle when pause button clicked                          | major  | Clicking pause stops the automatic transitions.                                                                  | C12          |
| 14  | interaction | Resume cycle when pause button clicked again                  | major  | Clicking pause again restarts the automatic transitions from current state.                                      | C13          |

## Justification

The Bioluminescence Bloom Cycle works as expected with timed organism glow transitions and pause control. Three circles display vertically representing coral (top), algae (middle), and plankton (bottom) organisms with labels "Coral", "Algae", and "Plankton" positioned below each corresponding circle. The simulation starts with the coral glowing. After 4 seconds, it switches to plankton glowing. After 3 seconds, it switches to algae glowing. After 2 seconds, it switches back to coral. The cycle repeats continuously through the coral-plankton-algae-coral sequence. A pause button displays and when clicked, stops the cycle. Clicking the pause button again resumes the cycle from the current state.
