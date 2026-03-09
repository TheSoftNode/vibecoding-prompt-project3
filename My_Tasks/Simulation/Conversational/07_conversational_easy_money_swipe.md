Category: Simulation

Prompt style: Conversational

Title: Money Swipe Simulator

Prompt: I want a money swiping simulator. When the app loads, display a $100 dollar bill image in the center on a white background. When I tap the dollar bill, it should swipe to the right off screen and disappear, then immediately a new $100 bill should appear back in the center so I can keep swiping infinitely. Below the dollar bill, show a counter that displays "Sent: $0" initially. Each time a bill completes its swipe off screen, increment the counter by $100 and update the display text in green color.

Required libraries: react, tailwindcss, framer-motion

## Rubric

| #   | ID          | Description                                                                                   | Weight | Rationale                                                                                                                                                      | Dependent On |
| --- | ----------- | --------------------------------------------------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display a white background when the app loads                                                 | minor  | The white background creates a clean canvas for the simulation elements.                                                                                       | None         |
| 2   | visual      | Display a $100 dollar bill image when the app loads                                           | major  | The dollar bill provides the main visual element users interact with to simulate sending money.                                                                | None         |
| 3   | layout      | Position the dollar bill in the center of the screen                                          | minor  | Center positioning makes the bill easily accessible and visually prominent.                                                                                    | None         |
| 4   | interaction | Trigger rightward swipe animation when the dollar bill is tapped                              | major  | Tapping initiates the swipe that simulates the money sending action.                                                                                           | None         |
| 5   | state       | Animate the dollar bill moving smoothly to the right until it disappears off screen           | major  | The smooth animation creates realistic motion as the bill travels off screen.                                                                                  | C4           |
| 6   | visual      | Display a new $100 bill in the center position immediately after the previous bill exits      | major  | Regenerating the bill enables continuous swiping without needing to reset manually.                                                                            | C5           |
| 7   | content     | Display counter text "Sent: $0" below the dollar bill when the app loads                     | major  | The starting counter shows the initial value before any swipes occur.                                                                                          | None         |
| 8   | state       | Calculate and increment the counter value by $100 each time a bill completes its swipe       | major  | The total is computed by adding $100 for each completed swipe.                                                                                                 | C5           |
| 9   | content     | Update the counter display text to reflect the new total after each increment                | major  | Updating the counter shows the cumulative amount sent across all swipes.                                                                                       | C8           |
| 10  | visual      | Display the counter text in green color                                                       | minor  | Green color indicates successful sending actions.                                                                                                              | C7           |
| 11  | layout      | Position the counter text centered horizontally below the dollar bill                         | minor  | Placing the counter below separates the interactive element from the tracking display.                                                                         | None         |

## Justification

The money swipe simulator works exactly as expected with infinite tap-to-swipe interaction. When the app loads, a $100 dollar bill image is displayed in the center of the screen with a counter showing "Sent: $0" below it in green color. When the dollar bill is tapped, it swipes to the right with smooth animation and disappears off screen. Immediately after the bill completes its swipe, a new $100 bill appears back in the center and the counter increments by $100, updating the display to show the new cumulative total. Users can continue tapping and swiping bills infinitely, with the counter tracking the total amount sent.
