Category: Simulation

Prompt style: Conversational

Title: Money Swipe Simulator

Prompt: I want a money swiping simulator. When the app loads, display a $100 dollar bill image in the center on a white background. When I tap the dollar bill, it should swipe to the right off screen and disappear. After the bill disappears, show the text "Sent $100" in green color centered below where the bill was originally positioned.

Required libraries: react, tailwindcss, framer-motion

## Rubric

| #   | ID          | Description                                                                                   | Weight | Rationale                                                                                                                 | Dependent On |
| --- | ----------- | --------------------------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display a white background when the app loads                                                 | minor  | The white background provides a clean canvas for displaying the dollar bill and text elements.                            | None         |
| 2   | visual      | Display a $100 dollar bill image when the app loads                                           | major  | The dollar bill provides the main visual element that users interact with to simulate sending money.                      | None         |
| 3   | layout      | Position the dollar bill in the center of the screen                                          | minor  | Center positioning makes the bill easily accessible and visually prominent for interaction.                               | None         |
| 4   | interaction | Swipe the dollar bill to the right off screen when tapped                                     | major  | Tapping triggers the rightward swipe that moves the bill off the screen, simulating the money sending action.             | None         |
| 5   | state       | Animate the dollar bill moving to the right with smooth motion until it disappears off screen | major  | The smooth swipe animation represents the ongoing time-evolving motion state as the bill travels off screen.              | C4           |
| 6   | content     | Display the text "Sent $100" after the bill disappears                                        | major  | The sent message provides textual confirmation of the completed money send action.                                        | C5           |
| 7   | visual      | Display the "Sent $100" text in green color                                                   | major  | The green color provides positive visual feedback indicating a successful send action.                                    | C6           |
| 8   | layout      | Center the "Sent $100" text below where the bill was originally positioned                    | minor  | Centered below positioning places the confirmation message in a natural reading location aligned with where the bill was. | C6           |

## Justification

The money swipe simulator works exactly as expected with a simple tap-to-swipe interaction. When the app loads, a $100 dollar bill image is displayed in the center of the screen. When the dollar bill is tapped, it swipes to the right with smooth animation and disappears off screen. After the bill swipes away and is removed from view, the text "Sent $100" appears in green color below where the bill was originally positioned, confirming the send action.
