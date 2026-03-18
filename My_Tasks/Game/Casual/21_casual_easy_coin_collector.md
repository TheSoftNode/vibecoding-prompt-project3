Category: Game

Prompt style: Casual

Title: Crystal Resonance Tuner

Prompt: Need a crystal tuning rhythm game. Show 5 glowing crystals scattered across a dark cave background, each pulsing at different speeds. Display a resonance meter at the top showing "Tune Count" starting at 0. When a player clicks a crystal while it's at peak brightness, it shatters with light particles and the tune count increases by 1. The crystals pulse continuously with random timing. When the player tunes all 5 crystals by clicking them at peak brightness, display "Perfect resonance!" message.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | ----------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display dark cave background                         | minor  | The cave background creates the atmospheric setting for the crystal game.           | None         |
| 2   | visual      | Display 5 glowing crystals scattered across cave     | major  | The crystals provide the clickable targets that players must tune.                  | None         |
| 3   | state       | Pulse each crystal at different random speeds        | major  | Pulsing at different speeds creates varied timing challenges for each crystal.      | C2           |
| 4   | visual      | Display resonance meter at top showing "Tune Count" | major  | The meter shows players their tuning progress.                                      | None         |
| 5   | content     | Initialize tune count at 0                           | minor  | Starting at zero establishes the baseline before any crystals are tuned.            | C4           |
| 6   | state       | Detect when crystal reaches peak brightness          | major  | Peak detection determines the correct timing window for clicking.                   | C3           |
| 7   | interaction | Shatter crystal when clicked at peak brightness      | major  | Clicking at peak creates light particles and removes the crystal.                   | C6           |
| 8   | interaction | Do nothing when crystal clicked not at peak          | minor  | Wrong timing clicks have no effect, requiring player to wait for peak.              | C6           |
| 9   | state       | Increase tune count by 1 when crystal tuned          | major  | Incrementing count tracks the player's tuning progress.                             | C7           |
| 10  | state       | Check if all 5 crystals are tuned                    | major  | Checking tuning completion determines when the win condition is met.                | C9           |
| 11  | content     | Display "Perfect resonance!" when all crystals tuned | major  | Win message provides feedback that the player succeeded.                            | C10          |

## Justification

The Crystal Resonance Tuner works as expected as a rhythm timing game with a win condition. A dark cave background displays with 5 glowing crystals scattered randomly across it. Each crystal pulses at a different random speed, creating varied timing challenges. A resonance meter displays at the top showing "Tune Count" initialized at 0. Each crystal continuously pulses, and the game detects when each crystal reaches peak brightness. When a player clicks a crystal at its peak brightness, it shatters with light particles and the tune count increases by 1. If a player clicks a crystal when it's not at peak brightness, nothing happens and the player must wait for the peak. The game checks if all 5 crystals are tuned. When the player tunes all 5 crystals by clicking them at peak brightness, the game checks completion and displays "Perfect resonance!" message.
