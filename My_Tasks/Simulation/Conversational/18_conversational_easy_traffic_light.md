Category: Simulation

Prompt style: Conversational

Title: Traffic Light Cycle

Prompt: I need an animated traffic light simulation. Display three circles stacked vertically representing red, yellow, and green lights. Start with red illuminated. After 3 seconds, switch to green. After 3 more seconds, switch to yellow. After 2 seconds, switch back to red. Cycle continuously. Show a timer displaying seconds remaining until the next color change.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                              | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | -------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display red circle for red light                         | major  | The red circle is the top light in the traffic signal showing the stop state.                                    | None         |
| 2   | visual      | Display yellow circle for yellow light                   | major  | The yellow circle is the middle light showing the caution/transition state.                                      | None         |
| 3   | visual      | Display green circle for green light                     | major  | The green circle is the bottom light showing the go state.                                                       | None         |
| 4   | layout      | Stack three circles vertically                           | minor  | Vertical stacking creates the standard traffic light layout from top to bottom: red, yellow, green.              | None         |
| 5   | state       | Start with red light illuminated                         | minor  | Starting on red establishes the initial state of the traffic cycle.                                              | None         |
| 6   | visual      | Illuminate active light brighter than inactive lights    | major  | Making the active light brighter shows which signal is currently active in the cycle.                            | None         |
| 7   | state       | Switch from red to green after 3 seconds                 | major  | The 3-second red duration matches typical traffic light timing before allowing traffic to proceed.               | None         |
| 8   | state       | Switch from green to yellow after 3 seconds              | major  | The 3-second green duration gives traffic time to proceed before the warning phase.                              | None         |
| 9   | state       | Switch from yellow to red after 2 seconds                | major  | The 2-second yellow duration provides the brief warning before stopping traffic.                                 | None         |
| 10  | state       | Cycle continuously through red-green-yellow-red sequence | major  | Continuous cycling maintains the ongoing traffic light simulation indefinitely.                                  | None         |
| 11  | state       | Count down seconds remaining until next color change     | major  | Counting down tracks the time so the system knows when to transition to the next light.                          | None         |
| 12  | content     | Display timer showing seconds remaining                  | major  | Showing the countdown tells users when the next color change will occur.                                         | None         |
| 13  | layout      | Position timer below the traffic light circles           | minor  | Placing the timer below separates the timing information from the visual signal display.                         | None         |

## Justification

The application achieved a 92.31% pass rate with one specific failure. Three circles display vertically representing red (top), yellow (middle), and green (bottom) lights. The simulation starts with the red light illuminated brighter than the others. After 3 seconds, it switches to green illuminated. After 3 more seconds, it switches to yellow. After 2 seconds, it switches back to red. The cycle repeats continuously through the red-green-yellow-red sequence. A timer counts down the seconds remaining until the next color change and displays this countdown value. However, the model failed to position the timer below the traffic light circles. Instead, the timer appears to the right of the circles or integrated into the light display, not below as required. This positioning issue caused the failure despite all other functionality working correctly.
