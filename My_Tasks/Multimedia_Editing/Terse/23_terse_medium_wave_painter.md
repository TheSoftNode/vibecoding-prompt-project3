Category: Multimedia_Editing

Prompt style: Terse

Title: Wave Pattern Painter

Prompt: Drag to draw waves. Every 3 waves cycles color blue-red-green. Count shows top-right. Undo removes wave and decrements count.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                 | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display blank canvas for drawing                            | major  | The canvas provides the drawing area where users create wave patterns.                                           | None         |
| 2   | interaction | Draw wave curve when user drags on canvas                   | major  | Dragging creates wave curves so users can paint their pattern.                                                   | None         |
| 3   | state       | Track total number of waves drawn                           | major  | Counting waves determines when to cycle brush colors based on the every-3 rule.                                  | C2           |
| 4   | content     | Display wave count in top-right corner                      | major  | Showing the count lets users see how many waves they've drawn.                                                   | C3           |
| 5   | layout      | Position wave count in top-right corner of canvas           | minor  | Top-right positioning keeps the counter visible without blocking the drawing area.                               | C4           |
| 6   | state       | Calculate current color from wave count modulo 3            | major  | Computing color from count divided by 3 determines which color in the blue-red-green cycle to use.               | C3           |
| 7   | visual      | Draw first 3 waves in blue color                            | major  | Blue color for waves 1-3 establishes the first phase of the color cycle.                                         | C6           |
| 8   | visual      | Draw next 3 waves in red color                              | major  | Red color for waves 4-6 establishes the second phase of the color cycle.                                         | C6           |
| 9   | visual      | Draw next 3 waves in green color                            | major  | Green color for waves 7-9 establishes the third phase before cycling back to blue.                               | C6           |
| 10  | state       | Cycle back to blue after every 3 colors complete            | major  | Cycling back creates the repeating blue-red-green pattern indefinitely.                                          | C6           |
| 11  | visual      | Display undo button                                         | major  | The undo button lets users remove their most recent wave.                                                        | None         |
| 12  | interaction | Remove last drawn wave when undo clicked                    | major  | Clicking undo deletes the most recent wave from the canvas.                                                      | C11          |
| 13  | state       | Decrement wave count when undo clicked                      | major  | Reducing the count keeps the counter accurate after removing a wave.                                             | C12          |
| 14  | state       | Update displayed count after decrement                      | major  | Updating the display reflects the new wave count after undo.                                                     | C13          |
| 15  | state       | Recalculate color based on new count after undo             | major  | Recalculating color ensures the next wave uses the correct color for the current count.                          | C13          |

## Justification

The Wave Pattern Painter creates evolving color patterns based on wave count with undo support. A blank canvas displays where users can drag to draw wave curves. The app tracks the total number of waves drawn and displays this count in the top-right corner of the canvas. Every 3 waves, the brush color cycles through blue, red, and green. The first 3 waves draw in blue, the next 3 in red, the next 3 in green, then the pattern cycles back to blue. The color is calculated from the wave count modulo 3. An undo button removes the last drawn wave, decrements the wave count, updates the displayed count, and recalculates the brush color based on the new count so the next wave uses the correct color.
