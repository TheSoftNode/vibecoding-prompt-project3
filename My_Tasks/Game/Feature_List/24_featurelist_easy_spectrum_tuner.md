Category: Game

Prompt style: Feature_List

Title: Spectrum Tuner Game

Prompt: Build a frequency matching game with these features: Display a target frequency bar at the top showing a random frequency between 100 Hz and 500 Hz labeled "Target: [X] Hz". Display three tuning knobs labeled "Low", "Mid", "High" below it. Each knob shows its current frequency value starting at 0 Hz. When players click a knob, its frequency increases by 50 Hz. Clicking past 300 Hz wraps the knob back to 0 Hz. Display a combined frequency meter labeled "Combined: [X] Hz" showing the sum of all three knobs. When the combined frequency matches the target frequency exactly, display "Frequency Locked!" message and disable all knobs.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                | Weight | Rationale                                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display target frequency bar at top                        | major  | Showing the target bar gives players the goal frequency they need to match.                         | None         |
| 2   | state       | Generate random frequency between 100 Hz and 500 Hz        | major  | Randomizing the target creates different puzzle challenges each game.                               | None         |
| 3   | content     | Display label "Target: [X] Hz" showing target frequency    | major  | Showing the target value tells players what total frequency they need to achieve.                   | C2           |
| 4   | visual      | Display three tuning knobs                                 | major  | Showing three knobs gives players the controls to build their frequency sum.                        | None         |
| 5   | content     | Display labels "Low", "Mid", "High" on knobs               | major  | Showing labels identifies each frequency band knob players can adjust.                              | C4           |
| 6   | content     | Display current frequency value on each knob starting at 0 Hz | major | Showing values tells players each knob's current frequency contribution.                         | C4           |
| 7   | interaction | Increase knob frequency by 50 Hz when knob clicked         | major  | Clicking knob increments its frequency so players can build toward the target.                      | C4           |
| 8   | state       | Wrap knob back to 0 Hz when clicked past 300 Hz            | major  | Wrapping frequency creates a cycling challenge where players must find the right combination.       | C7           |
| 9   | content     | Update knob display after frequency change                 | major  | Updating display shows players the new frequency value after each click.                            | C7, C8       |
| 10  | visual      | Display combined frequency meter                           | major  | Showing the combined meter lets players see their progress toward the target.                       | None         |
| 11  | state       | Calculate sum of all three knob frequencies                | major  | Summing frequencies determines the total players have built.                                        | C7, C8       |
| 12  | content     | Display label "Combined: [X] Hz" showing sum               | major  | Showing the combined value tells players their real-time total frequency.                           | C11          |
| 13  | state       | Detect when combined equals target frequency               | major  | Checking equality determines if players solved the frequency matching puzzle.                       | C11          |
| 14  | content     | Display "Frequency Locked!" when frequencies match         | major  | Showing the locked message tells players they won the tuning challenge.                             | C13          |
| 15  | interaction | Disable all knobs when frequencies match                   | major  | Disabling knobs prevents further changes after players achieve the exact match.                     | C13          |

## Justification

The spectrum tuner game works as expected for frequency matching puzzles. A target frequency bar displays at the top showing a random frequency between 100 Hz and 500 Hz labeled "Target: [X] Hz". Three tuning knobs display below labeled "Low", "Mid", "High", each showing its current frequency value starting at 0 Hz. When players click a knob, its frequency increases by 50 Hz and the display updates. Clicking past 300 Hz wraps the knob back to 0 Hz. A combined frequency meter displays labeled "Combined: [X] Hz" showing the sum of all three knobs in real time. When the combined frequency matches the target frequency exactly, "Frequency Locked!" message displays and all knobs become disabled.
