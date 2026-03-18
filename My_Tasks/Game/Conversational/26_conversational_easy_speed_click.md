Category: Game

Prompt style: Conversational

Title: Speed Clicker

Prompt: I want to build a speed clicking game. Display a large "Click Me!" button in the center of the screen. Display a countdown timer labeled "Time: 10" starting at 10 seconds. When I click the "Click Me!" button, increment a click counter and update the display. The timer counts down automatically from 10 to 0. When the timer reaches 0, disable the button and display a "Final Score: [X] clicks" message showing how many times I clicked.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display large "Click Me!" button                     | major  | Showing button gives players the target they need to click rapidly.                          | None         |
| 2   | layout      | Position button in center of screen                  | minor  | Centering button makes it easy for players to focus and click quickly.                       | C1           |
| 3   | content     | Display countdown timer labeled "Time: 10"           | major  | Showing timer tells players how much time remains for clicking.                              | None         |
| 4   | state       | Start timer at 10 seconds                            | major  | Starting at 10 creates the time limit for the speed clicking challenge.                      | None         |
| 5   | state       | Count down automatically from 10 to 0                | major  | Automatic countdown creates the timed pressure for rapid clicking.                           | C4           |
| 6   | content     | Update displayed timer as countdown progresses       | major  | Updating display shows players the remaining time in real time.                              | C5           |
| 7   | interaction | Detect button clicks from player                     | major  | Detecting clicks captures the rapid clicking actions for counting.                           | C1           |
| 8   | state       | Increment click counter when button clicked          | major  | Incrementing count tracks how many times the player clicked during the challenge.            | C7           |
| 9   | content     | Update displayed click count after each click        | major  | Updating display shows players their clicking progress in real time.                         | C8           |
| 10  | state       | Detect when timer reaches 0                          | major  | Checking for zero determines when the timed challenge ends.                                  | C5           |
| 11  | interaction | Disable button when timer reaches 0                  | major  | Disabling button stops further clicking once time is up.                                     | C10          |
| 12  | content     | Display "Final Score: [X] clicks" message at end    | major  | Showing final score tells players their total clicking performance.                          | C10          |
| 13  | content     | Show actual click count in final score message       | major  | Displaying the number tells players exactly how many clicks they achieved.                   | C8, C12      |

## Justification

The speed clicker game works as expected for timed rapid clicking gameplay. A large "Click Me!" button displays positioned in the center of the screen. A countdown timer labeled "Time: 10" displays starting at 10 seconds and counts down automatically from 10 to 0, updating the displayed time as it progresses. When players click the "Click Me!" button, the game detects the click, increments a click counter, and updates the displayed count after each click. When the timer reaches 0, the game detects completion, disables the button to prevent further clicking, and displays a "Final Score: [X] clicks" message showing the actual click count the player achieved.
