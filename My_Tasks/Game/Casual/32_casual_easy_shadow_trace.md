Category: Game

Prompt style: Casual

Title: Shadow Path Tracer

Prompt: Hover to draw a fading trail. Click target dots to remove them and increase hit count at top. Trail fades after 2 seconds.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                      | Weight | Rationale                                                                  | Dependent On |
| --- | ----------- | ------------------------------------------------ | ------ | -------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display target dot objects                       | major  | Target dots give players something to aim for.                             | None         |
| 2   | visual      | Draw fading trail on hover                       | major  | Trail shows where the cursor has been.                                     | None         |
| 3   | state       | Make trail fade after 2 seconds                  | major  | Fading after 2 seconds creates time pressure.                              | C2           |
| 4   | interaction | Hit target when clicked                          | major  | Clicking target scores a point.                                            | None         |
| 5   | state       | Remove target when hit                           | major  | Removing hit targets keeps the game progressing.                           | C4           |
| 6   | content     | Display hit count                                | minor  | Count shows how many targets were hit.                                     | None         |
| 7   | layout      | Position hit count at top                        | minor  | Top positioning keeps score visible.                                       | C6           |
| 8   | state       | Increment hit count when target clicked          | major  | Counting hits tracks player performance.                                   | C4           |

## Justification

The shadow path tracer game works as a trail-following targeting game with scoring. Target dot objects display on screen. When players hover, a fading trail draws showing where the cursor has been. The trail disappears after time creating time pressure. When players click a target, it gets hit and removes from the screen. A hit count displays at the top and increments each time a target is clicked tracking player performance.
