Category: Simulation

Prompt style: Conversational

Title: Bioluminescence Bloom Cycle

Prompt: I need an animated bioluminescence bloom simulation. Display three circles stacked vertically representing coral, algae, and plankton organisms with labels "Coral", "Algae", and "Plankton" below each circle. Start with coral illuminated brighter than the others. After 4 seconds, switch to plankton illuminated brighter. After 3 seconds, switch to algae illuminated brighter. After 2 seconds, switch back to coral illuminated brighter. Cycle continuously. Include a pause button that stops the cycle when clicked and resumes when clicked again.

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
| 7   | state       | Start with coral illuminated brighter than others            | minor  | Starting with coral brighter establishes the initial state of the bloom cycle.                                   | None         |
| 8   | state       | Switch from coral to plankton after 4 seconds                 | major  | The 4-second coral duration sets the first phase timing before transitioning to plankton.                        | None         |
| 9   | state       | Switch from plankton to algae after 3 seconds                 | major  | The 3-second plankton duration gives the second phase time before moving to algae.                               | None         |
| 10  | state       | Switch from algae to coral after 2 seconds                    | major  | The 2-second algae duration provides the brief third phase before returning to start.                            | None         |
| 11  | state       | Cycle continuously through coral-plankton-algae-coral sequence| major  | Continuous cycling maintains the ongoing bloom simulation indefinitely.                                          | None         |
| 12  | visual      | Display pause button                                          | major  | The pause button provides the control for stopping and resuming the cycle.                                       | None         |
| 13  | interaction | Stop cycle when pause button clicked                          | major  | Clicking pause stops the automatic transitions.                                                                  | C12          |
| 14  | interaction | Resume cycle when pause button clicked again                  | major  | Clicking pause again restarts the automatic transitions from current state.                                      | C13          |

## Justification

The bioluminescence bloom simulation works as expected for animated organism illumination cycling. Three circles display stacked vertically representing coral, algae, and plankton organisms with labels "Coral", "Algae", and "Plankton" below each circle. The simulation starts with coral illuminated brighter than the others. After 4 seconds, it switches to plankton illuminated brighter. After 3 seconds, it switches to algae illuminated brighter. After 2 seconds, it switches back to coral illuminated brighter. The cycle repeats continuously. A pause button displays and when clicked, stops the cycle. Clicking the pause button again resumes the cycle.
