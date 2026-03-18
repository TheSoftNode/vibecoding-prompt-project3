Category: Game

Prompt style: Conversational

Title: Pressure Balancer

Prompt: I need a pressure balancing game with fluid containers. Display two vertical tanks side by side labeled "Tank L" and "Tank R", each showing a pressure gauge starting at "0 PSI". Below each tank, show an "Add Pressure" button. When a player clicks an Add Pressure button, that tank's pressure increases by a random amount between 5 PSI and 15 PSI. The goal is to get both tanks to exactly 50 PSI total pressure combined. When the combined pressure of both tanks equals exactly 50 PSI, display "Perfect Balance Achieved!" message. If combined pressure goes over 50 PSI, display "Overpressure! Try again." message and reset both tanks to 0 PSI.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                | Weight | Rationale                                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display two vertical tanks side by side                    | major  | Showing two tanks gives players the containers they need to balance pressure between.               | None         |
| 2   | content     | Display labels "Tank L" and "Tank R" on tanks              | major  | Showing labels identifies each tank in the balancing system.                                        | C1           |
| 3   | visual      | Display pressure gauge on each tank                        | major  | Showing gauges lets players see the current pressure level in each tank.                            | C1           |
| 4   | content     | Display "0 PSI" as starting pressure on gauges             | major  | Showing starting pressure tells players both tanks begin empty.                                     | C3           |
| 5   | visual      | Display Add Pressure button below each tank                | major  | Showing buttons gives players controls to increase pressure in each tank.                           | C1           |
| 6   | interaction | Increase tank pressure when Add Pressure button clicked    | major  | Clicking button adds pressure to that tank for players to build toward the goal.                    | C5           |
| 7   | state       | Generate random pressure increase between 5 PSI and 15 PSI | major  | Randomizing the increase creates unpredictable challenge for reaching exact target.                 | C6           |
| 8   | content     | Update gauge to show new pressure after increase           | major  | Updating gauge tells players the new pressure level after each addition.                            | C7           |
| 9   | state       | Calculate combined pressure of both tanks                  | major  | Summing both tanks determines if players reached the balance goal.                                  | C7           |
| 10  | state       | Detect when combined pressure equals exactly 50 PSI        | major  | Checking for exact 50 PSI determines if players won the balancing challenge.                        | C9           |
| 11  | content     | Display "Perfect Balance Achieved!" when total is 50 PSI   | major  | Showing success message tells players they achieved the exact pressure goal.                        | C10          |
| 12  | state       | Detect when combined pressure exceeds 50 PSI               | major  | Checking for overpressure determines if players failed by adding too much.                          | C9           |
| 13  | content     | Display "Overpressure! Try again." when over 50 PSI        | major  | Showing failure message tells players they exceeded the limit.                                      | C12          |
| 14  | interaction | Reset both tanks to 0 PSI when overpressure occurs         | major  | Resetting tanks lets players try the balancing challenge again from the start.                      | C12          |

## Justification

The pressure balancer game works as expected for precision resource management. Two vertical tanks display side by side labeled "Tank L" and "Tank R", each showing a pressure gauge starting at "0 PSI". Below each tank, an "Add Pressure" button displays. When a player clicks an Add Pressure button, that tank's pressure increases by a random amount between 5 PSI and 15 PSI and the gauge updates to show the new pressure. The app calculates the combined pressure of both tanks. The goal is to get both tanks to exactly 50 PSI total pressure combined. When the combined pressure equals exactly 50 PSI, "Perfect Balance Achieved!" message displays. If combined pressure goes over 50 PSI, "Overpressure! Try again." message displays and both tanks reset to 0 PSI.
