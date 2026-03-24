Category: Simulation

Prompt style: Feature_List

Title: Domino Chain Reaction

Prompt: Build a domino chain reaction simulator. Display a row of 10 vertical gray dominoes equally spaced in a horizontal line. Include a "Push" button positioned above the leftmost domino. When clicked, animate dominoes falling sequentially from left to right with a short delay between each fall, creating a chain reaction effect where each domino tips over before the next one falls.

Required libraries: react, tailwindcss, framer-motion

## Rubric

| #   | ID          | Description                                                                           | Weight | Rationale                                                                                                                        | Dependent On |
| --- | ----------- | ------------------------------------------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 10 domino elements                                                            | major  | Ten dominoes provide enough pieces to demonstrate a satisfying chain reaction without overwhelming the screen.                   | None         |
| 2   | content     | Display dominoes in gray color                                                        | minor  | Gray gives dominoes a neutral stone-like appearance that resembles real domino pieces.                                           | None         |
| 3   | visual      | Display dominoes in vertical upright orientation initially                            | major  | Vertical orientation represents standing dominoes ready to fall, establishing the initial state before chain reaction begins.    | None         |
| 4   | layout      | Arrange all 10 dominoes in single horizontal row                                      | major  | Horizontal row alignment creates the classic domino chain setup where each piece can knock down the next.                        | None         |
| 5   | layout      | Space dominoes equally with consistent gaps between consecutive pieces                | minor  | Equal spacing creates visual rhythm and ensures each domino has room to fall without colliding incorrectly with neighbors.       | None         |
| 6   | visual      | Display button labeled "Push"                                                         | major  | The push button provides clear interaction point for users to initiate the chain reaction.                                       | None         |
| 7   | layout      | Position push button above leftmost domino                                            | minor  | Positioning above the first domino shows visually which piece gets pushed to start the cascade.                                  | None         |
| 8   | interaction | Trigger domino animation sequence when push button is clicked                         | major  | Click interaction starts the simulation, letting users control when the chain reaction begins.                                   | C6           |
| 9   | state       | Animate leftmost domino falling first when sequence starts                            | major  | The first domino must fall to initiate the chain, representing the initial push that starts the cascade.                         | C8           |
| 10  | state       | Animate remaining dominoes falling sequentially from left to right                    | major  | Sequential left-to-right falling creates the chain reaction effect where each domino triggers the next.                          | C9           |
| 11  | state       | Add short delay between consecutive domino falls during sequence                      | major  | Delay between falls makes the chain reaction visible and satisfying instead of all pieces falling simultaneously.                | C10          |
| 12  | state       | Rotate each domino from vertical to horizontal orientation during fall animation      | major  | Rotation from upright to tipped represents the physical falling motion where dominoes pivot around their base edge.              | None         |

## Justification

The domino chain reaction simulator demonstrates sequential cascade physics with interactive trigger control. Ten gray rectangular dominoes appear in vertical upright orientation, arranged in a single horizontal row with equal spacing between consecutive pieces. Above the leftmost domino sits a button labeled "Push" that initiates the sequence. When users click the push button, the leftmost domino animates first, rotating from vertical to horizontal to show it falling over. Then remaining dominoes fall sequentially from left to right in order, with each piece rotating to horizontal orientation one after another. A short delay separates consecutive falls, creating a visible chain reaction where users can watch the cascade travel through the row instead of all dominoes falling at once.
