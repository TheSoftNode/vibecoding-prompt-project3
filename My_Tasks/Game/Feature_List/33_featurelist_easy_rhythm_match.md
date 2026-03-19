Category: Game

Prompt style: Feature_List

Title: Rhythm Matcher

Prompt: Build a rhythm pattern matching game with these features: Display four beat circles arranged horizontally labeled "Beat 1", "Beat 2", "Beat 3", "Beat 4". Display a "Play Rhythm" button below them. When players click "Play Rhythm", play a rhythm pattern by pulsing 3 random beats in sequence - each selected beat pulses larger for 0.5 seconds then returns to normal size, with 0.3 second gaps between pulses. Display a timing accuracy label showing "Waiting..." initially. When players click beats after the rhythm plays, record the time between clicks. When the player has clicked 3 beats, check if the intervals match the original rhythm's timing within 0.2 seconds tolerance. If intervals match, display "Perfect Timing!" in green. If intervals don't match, display "Off Beat!" in red.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display four beat circles horizontally               | major  | The circles provide the rhythm input interface.                                              | None         |
| 2   | content     | Label circles "Beat 1", "Beat 2", "Beat 3", "Beat 4" | major  | Labels identify each beat position.                                                          | C1           |
| 3   | visual      | Display "Play Rhythm" button below circles           | major  | The button lets players trigger the rhythm pattern.                                          | None         |
| 4   | state       | Generate sequence of 3 random beats                  | major  | Randomizing creates different timing challenges.                                             | None         |
| 5   | interaction | Pulse selected beats larger when pattern plays       | major  | Pulsing shows players the rhythm timing to match.                                            | C3           |
| 6   | state       | Pulse each beat for 0.5 seconds with 0.3s gaps       | major  | Specific timing creates the rhythm pattern to memorize.                                      | C5           |
| 7   | content     | Display "Waiting..." timing label initially          | major  | The label tells players no input has been recorded yet.                                      | None         |
| 8   | interaction | Record time between clicks when beats clicked        | major  | Recording intervals captures the player's rhythm timing.                                     | C1           |
| 9   | state       | Detect when player has clicked 3 beats               | major  | Checking count determines when to evaluate the timing.                                       | C8           |
| 10  | state       | Compare intervals to original rhythm within 0.2s tolerance | major  | Comparing determines if the player matched the rhythm timing.                                | C9           |
| 11  | content     | Display "Perfect Timing!" in green when match        | major  | Green message confirms the player matched the rhythm.                                        | C10          |
| 12  | content     | Display "Off Beat!" in red when mismatch             | major  | Red message tells the player their timing was off.                                           | C10          |

## Justification

The rhythm matcher game works exactly as expected for timing-based pattern matching. Four beat circles display horizontally labeled "Beat 1", "Beat 2", "Beat 3", "Beat 4". A "Play Rhythm" button displays below them. A timing accuracy label displays "Waiting..." initially. When players click "Play Rhythm", a rhythm pattern plays by pulsing 3 random beats in sequence - each pulses larger for 0.5 seconds then returns to normal, with 0.3 second gaps between pulses. When players click beats after the rhythm plays, the time between clicks is recorded. When the player has clicked 3 beats, the intervals are compared to the original rhythm's timing. If intervals match within 0.2 seconds tolerance, "Perfect Timing!" displays in green. If intervals don't match, "Off Beat!" displays in red.
