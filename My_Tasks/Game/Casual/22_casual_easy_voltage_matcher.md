Category: Game

Prompt style: Casual

Title: Voltage Matcher Challenge

Prompt: Need a voltage matching puzzle game. Display a target voltage meter at the top showing a random voltage between 5V and 15V labeled "Target: [X]V". Below it, show three circuit breaker switches labeled "3V", "5V", "7V" that players can toggle on or off. Display a current voltage meter labeled "Current: 0V" that sums up all active switch voltages. Players must turn on the right combination of switches to match the target voltage exactly. When the current voltage equals the target voltage, display "Circuit Complete!" message and highlight the meters in green.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                | Weight | Rationale                                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display target voltage meter at top                        | major  | Showing the target meter gives players the goal voltage they need to match.                         | None         |
| 2   | state       | Generate random voltage between 5V and 15V                 | major  | Randomizing the target creates different puzzle challenges each game.                               | None         |
| 3   | content     | Display label "Target: [X]V" showing target voltage        | major  | Showing the target value tells players what voltage sum they need to achieve.                       | C2           |
| 4   | visual      | Display three circuit breaker switches                     | major  | Showing three switches gives players the controls to build their voltage sum.                       | None         |
| 5   | content     | Display labels "3V", "5V", "7V" on switches                | major  | Showing voltage values tells players what each switch contributes to the sum.                       | C4           |
| 6   | interaction | Toggle switch on when clicked                              | major  | Clicking a switch turns it on so its voltage adds to the current total.                             | C4           |
| 7   | interaction | Toggle switch off when clicked again                       | major  | Clicking an active switch turns it off so its voltage subtracts from the total.                     | C6           |
| 8   | visual      | Display current voltage meter                              | major  | Showing the current meter lets players see their progress toward the target.                        | None         |
| 9   | state       | Calculate sum of all active switch voltages                | major  | Summing active voltages determines the current total players have built.                            | C6, C7       |
| 10  | content     | Display label "Current: [X]V" showing current sum          | major  | Showing the current value tells players their real-time voltage total.                              | C9           |
| 11  | state       | Detect when current equals target voltage                  | major  | Checking equality determines if players solved the voltage matching puzzle.                         | C9           |
| 12  | content     | Display "Circuit Complete!" message when voltages match    | major  | Showing the completion message tells players they won the matching challenge.                       | C11          |
| 13  | visual      | Highlight meters in green when voltages match              | major  | Highlighting meters green provides visual feedback that the circuit is successfully completed.      | C11          |

## Justification

The voltage matcher game works as expected for circuit puzzle solving. A target voltage meter displays at the top showing a random voltage between 5V and 15V with label "Target: [X]V". Below it, three circuit breaker switches display labeled "3V", "5V", "7V" that players can toggle on or off by clicking. A current voltage meter displays labeled "Current: 0V" that calculates and shows the sum of all active switch voltages in real time. Players turn on the right combination of switches to match the target voltage exactly. When the current voltage equals the target voltage, "Circuit Complete!" message displays and the meters highlight in green.
