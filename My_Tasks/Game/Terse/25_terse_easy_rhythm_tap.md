Category: Game

Prompt style: Terse

Title: Rhythm Beat Tapper

Prompt: Falling beats drop from top. Press spacebar when beat reaches bottom line. Perfect timing shows "Perfect!" and adds 10 points. Miss shows "Miss!" Score shows top-right.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display falling beat objects                         | major  | Showing beat objects gives players the targets they need to tap on time.                     | None         |
| 2   | state       | Move beats downward from top continuously            | major  | Moving beats downward creates the timing challenge for the rhythm game.                      | C1           |
| 3   | visual      | Display bottom line as timing target                 | major  | Showing the target line tells players where to time their taps.                              | None         |
| 4   | layout      | Position bottom line at lower section                | minor  | Placing line at bottom creates the target zone for timing judgment.                          | C3           |
| 5   | interaction | Detect spacebar press from player                    | major  | Detecting spacebar lets players attempt to hit the beat on time.                             | None         |
| 6   | state       | Check if beat is at bottom line when spacebar pressed| major  | Checking alignment determines if the timing was perfect or a miss.                           | C5           |
| 7   | content     | Display "Perfect!" when timing is accurate           | major  | Showing perfect message gives feedback that the player timed it correctly.                   | C6           |
| 8   | state       | Add 10 points to score on perfect timing             | major  | Adding points rewards players for accurate rhythm timing.                                    | C6           |
| 9   | content     | Display "Miss!" when timing is inaccurate            | major  | Showing miss message tells players they pressed too early or too late.                       | C6           |
| 10  | content     | Display score counter                                | minor  | Showing score lets players track their rhythm accuracy performance.                          | C8           |
| 11  | layout      | Position score in top-right corner                   | minor  | Top-right positioning keeps score visible without blocking the falling beats.                | C10          |
| 12  | state       | Update displayed score after each perfect hit        | major  | Updating score shows players their cumulative rhythm performance in real time.               | C8           |

## Justification

The rhythm beat tapper game works as expected for timing-based gameplay with scoring. Falling beat objects display and move downward from the top continuously. A bottom line displays positioned at the lower section as the timing target. When players press the spacebar, the game checks if a beat is at the bottom line at that moment. If timing is accurate, "Perfect!" displays and 10 points add to the score. If timing is inaccurate, "Miss!" displays. A score counter displays in the top-right corner and updates after each perfect hit showing the cumulative performance.
