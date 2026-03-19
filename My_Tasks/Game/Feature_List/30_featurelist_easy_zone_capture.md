Category: Game

Prompt style: Feature_List

Title: Zone Capturer

Prompt: Build a territory capturing timing game with these features: Display three circular zones labeled "Zone A", "Zone B", "Zone C" arranged horizontally across the screen, each starting with gray color. Display a "Start Capture" button below the zones. When players click "Start Capture", all three zones begin filling with color from bottom to top over 5 seconds - Zone A fills with blue, Zone B with green, Zone C with red. Display a capture status label showing "Capturing..." during the fill animation. When players click a zone while it's filling, that zone stops filling and locks at its current fill percentage. When all three zones are either locked by clicking or fully filled, display "Territory Secured!" message.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display three circular zones horizontally            | major  | The zones provide the capture targets for the timing challenge.                              | None         |
| 2   | content     | Label zones "Zone A", "Zone B", "Zone C"             | major  | Labels identify each distinct capture zone.                                                  | C1           |
| 3   | visual      | Color all zones gray initially                       | major  | Gray shows the uncaptured state before the game starts.                                      | C1           |
| 4   | visual      | Display "Start Capture" button below zones           | major  | The button gives players control to begin the capture sequence.                              | None         |
| 5   | interaction | Begin filling all zones when button clicked          | major  | Starting the fill creates the timing challenge.                                              | C4           |
| 6   | state       | Fill each zone from bottom to top over 5 seconds     | major  | The 5-second fill sets the timing window players must work within.                           | C5           |
| 7   | visual      | Fill Zone A with blue color                          | minor  | Blue color provides visual feedback for Zone A's capture progress.                           | C5           |
| 8   | visual      | Fill Zone B with green color                         | minor  | Green color provides visual feedback for Zone B's capture progress.                          | C5           |
| 9   | visual      | Fill Zone C with red color                           | minor  | Red color provides visual feedback for Zone C's capture progress.                            | C5           |
| 10  | content     | Display "Capturing..." status during fill            | major  | The status tells players the capture sequence is active.                                     | C5           |
| 11  | interaction | Stop zone filling when zone clicked                  | major  | Clicking stops the fill locking that zone's capture percentage.                              | C5           |
| 12  | state       | Lock zone at current fill percentage when clicked    | major  | Locking preserves the timing of the player's click.                                          | C11          |
| 13  | state       | Detect when all zones locked or fully filled         | major  | Checking completion determines when the capture phase ends.                                  | C6, C12      |
| 14  | content     | Display "Territory Secured!" when complete           | major  | The message tells players the capture sequence finished.                                     | C13          |

## Justification

The zone capturer game works exactly as expected for timing-based territory control. Three circular zones display horizontally labeled "Zone A", "Zone B", "Zone C", all starting with gray color. A "Start Capture" button displays below the zones. When players click "Start Capture", all three zones begin filling with color from bottom to top over 5 seconds - Zone A fills with blue, Zone B with green, Zone C with red. A capture status label displays "Capturing..." during the fill. When players click a zone while it's filling, that zone stops filling and locks at its current fill percentage. When all three zones are either locked by clicking or fully filled, "Territory Secured!" message displays.
