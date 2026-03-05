Color Grid Game
Color Grid Game
Difficulty
Medium
Category
Game
Style
Detailed Specification
Length
Detailed
Prompt
Build a pattern memory game on a 3x3 grid of colored panels, each panel a different color. Each round, the game plays back a growing sequence by lighting up panels one at a time with a delay of at least 300 milliseconds between steps, then waits for the player to repeat it by clicking. The sequence starts at one step and adds one more each round. Correct clicks highlight the panel in its color. An incorrect click flashes the panel red and ends the game with a visible game-over message. Score points for each completed round, with each round worth 50% more than the last. Display the score prominently and the current round number as secondary info. Panels should look distinct from each other in their idle state and visually change during playback and interaction. Include a start button to begin the game and a restart button after game over.
Required Libraries
react, framer-motion

Rubric

| ID            | Description                                                                                                                        | Weight | Rationale                                                                                      | Dependent On         |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------- | -------------------- |
| layout-1      | Arrange nine panels in a 3x3 grid formation                                                                                        | major  | A 3x3 grid defines the playing field and everything else builds on top of it.                  | None                 |
| visual-1      | Assign each of the nine panels a visually distinct color in its idle state                                                         | major  | Players track the sequence by color, so each panel must be easily distinguishable at a glance. | layout-1             |
| content-1     | Display a Start button before gameplay begins                                                                                      | major  | Without a Start button, the sequence would begin on page load before the player is ready.      | None                 |
| state-1       | Extend the sequence by one additional panel each round, beginning with a single panel in round one                                 | major  | Adding one step per round creates the difficulty curve and makes the game a memory challenge.  | None                 |
| state-2       | Play back the current sequence by visually activating panels one at a time with a delay of at least 300 milliseconds between steps | major  | Sequential playback at a readable speed is required for the player to follow the pattern.      | state-1              |
| interaction-1 | Accept player clicks on panels to register input after the sequence finishes playing                                               | major  | Player input is required to attempt reproducing the sequence.                                  | state-2              |
| interaction-2 | Highlight a panel when the player clicks it during input                                                                           | major  | Visual feedback confirms that the player's input was registered.                               | interaction-1        |
| interaction-3 | Flash a panel red when the player clicks an incorrect panel in the sequence                                                        | major  | Red provides a clear and universal signal that the input was incorrect.                        | interaction-1        |
| content-2     | Display a game-over message when the player makes an incorrect click                                                               | major  | Players need explicit feedback that the game has ended.                                        | interaction-3        |
| content-3     | Display the player's current score on screen                                                                                       | major  | The score is the primary feedback players use to measure performance.                          | None                 |
| content-4     | Display the current round number on screen                                                                                         | minor  | The round number provides helpful context without competing with the score.                    | None                 |
| visual-2      | Render the score with greater visual prominence than the round number                                                              | minor  | The visual hierarchy should reflect that the score is primary and the round is secondary.      | content-3, content-4 |
| content-5     | Provide a Restart button after the game reaches a game-over state                                                                  | major  | Without a Restart button, players would need to reload the page to play again.                 | content-2            |
| state-3       | Increase the point value of each round by 50% compared to the previous round                                                       | major  | Progressive scoring is explicitly required by the prompt and rewards longer sequences.         | content-3            |

ID
Description
Weight
Rationale
Dependent On
layout-1
Arrange nine panels in a 3x3 grid formation
major
A 3x3 grid defines the playing field and everything else builds on top of it.
None
visual-1
Assign each of the nine panels a visually distinct color in its idle state
major
Players track the sequence by color, so each panel must be easily distinguishable at a glance.
layout-1
content-1
Display a Start button before gameplay begins
major
Without a Start button, the sequence would begin on page load before the player is ready.
None
state-1
Extend the sequence by one additional panel each round, beginning with a single panel in round one
major
Adding one step per round creates the difficulty curve and makes the game a memory challenge.
None
state-2
Play back the current sequence by visually activating panels one at a time with a delay of at least 300 milliseconds between steps
major
Sequential playback at a readable speed is required for the player to follow the pattern.
state-1
interaction-1
Accept player clicks on panels to register input after the sequence finishes playing
major
Player input is required to attempt reproducing the sequence.
state-2
interaction-2
Highlight a panel when the player clicks it during input
major
Visual feedback confirms that the player's input was registered.
interaction-1
interaction-3
Flash a panel red when the player clicks an incorrect panel in the sequence
major
Red provides a clear and universal signal that the input was incorrect.
interaction-1
content-2
Display a game-over message when the player makes an incorrect click
major
Players need explicit feedback that the game has ended.
interaction-3
content-3
Display the player's current score on screen
major
The score is the primary feedback players use to measure performance.
None
content-4
Display the current round number on screen
minor
The round number provides helpful context without competing with the score.
None
visual-2
Render the score with greater visual prominence than the round number
minor
The visual hierarchy should reflect that the score is primary and the round is secondary.
content-3, content-4
content-5
Provide a Restart button after the game reaches a game-over state
major
Without a Restart button, players would need to reload the page to play again.
content-2
state-3
Increase the point value of each round by 50% compared to the previous round
major
Progressive scoring is explicitly required by the prompt and rewards longer sequences.
content-3
