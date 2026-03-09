Category: Simulation

Prompt style: Conversational

Title: Money Swipe Simulator

Prompt: I want a money swiping simulator. When the app loads, display a $100 dollar bill image in the center on a white background. When I tap the dollar bill, it should swipe to the right off screen and disappear, then immediately a new $100 bill should appear back in the center so I can keep swiping infinitely. Below the dollar bill, show a counter that displays "Sent: $0" initially. Each time a bill completes its swipe off screen, increment the counter by $100 and update the display text in green color.

Required libraries: react, tailwindcss, framer-motion

## Rubric

| #   | ID          | Description                                                                                   | Weight | Rationale                                                                                                                                                                                       | Dependent On |
| --- | ----------- | --------------------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display a white background when the app loads                                                 | minor  | The white background provides a clean canvas that ensures the dollar bill and counter elements are clearly visible without visual clutter or distracting patterns.                              | None         |
| 2   | visual      | Display a $100 dollar bill image when the app loads                                           | major  | The dollar bill image serves as the primary interactive element that users tap to trigger swipe actions, making it essential for the core simulation experience.                                | None         |
| 3   | layout      | Position the dollar bill in the center of the screen                                          | minor  | Centering the bill horizontally and vertically creates balanced visual composition and ensures the interactive element is easily reachable regardless of screen size.                           | None         |
| 4   | interaction | Trigger rightward swipe animation when the dollar bill is tapped                              | major  | The tap interaction initiates the swipe sequence that simulates sending money, forming the foundation of the user's engagement with the simulator.                                              | None         |
| 5   | state       | Animate the dollar bill moving smoothly to the right until it disappears off screen           | major  | The continuous rightward motion represents time-evolving animation state where the bill's position updates frame-by-frame creating the swipe effect.                                            | C4           |
| 6   | visual      | Display a new $100 bill in the center position immediately after the previous bill exits      | major  | Regenerating the bill restores the main interactive visual element ensuring the simulation remains playable for infinite rounds without manual resets.                                          | C5           |
| 7   | content     | Display counter text "Sent: $0" below the dollar bill when the app loads                     | major  | The initial counter text establishes the baseline value that will increment with each swipe, providing users with a starting reference point for tracking their sending activity.               | None         |
| 8   | state       | Calculate and increment the counter value by $100 each time a bill completes its swipe       | major  | Computing the running total represents derived state that accumulates based on completed swipe events, maintaining an accurate count of all sending actions.                                    | C5           |
| 9   | content     | Update the counter display text to reflect the new total after each increment                | major  | Refreshing the displayed text ensures users see real-time feedback showing the cumulative amount sent, reinforcing the impact of each swipe action.                                             | C8           |
| 10  | interaction | Display the counter text in green color                                                       | minor  | The green color provides positive visual feedback that signals successful money sending actions, creating an encouraging interaction response that motivates continued engagement.              | C7           |
| 11  | layout      | Position the counter text centered horizontally below the dollar bill                         | minor  | Placing the counter directly beneath the bill creates logical visual hierarchy where the action element sits above the result tracker, making the cause-and-effect relationship immediately clear. | None         |

## Justification

The money swipe simulator works exactly as expected with infinite tap-to-swipe interaction. When the app loads, a $100 dollar bill image is displayed in the center of the screen with a counter showing "Sent: $0" below it in green color. When the dollar bill is tapped, it swipes to the right with smooth animation and disappears off screen. Immediately after the bill completes its swipe, a new $100 bill appears back in the center and the counter increments by $100, updating the display to show the new cumulative total. Users can continue tapping and swiping bills infinitely, with the counter tracking the total amount sent.
