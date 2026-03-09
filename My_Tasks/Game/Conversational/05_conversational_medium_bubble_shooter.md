Category: Game

Prompt style: Conversational

Title: Chain Reaction Bubble Shooter

Prompt: I want a bubble shooter game. Display 5 rows of colored bubbles at top: red, blue, green. Cannon at bottom center rotates to follow mouse cursor. Click to shoot bubble toward cursor with smooth flight animation. When shot bubble collides with existing bubble, attach it and check for 3+ same-colored touching bubbles: those pop with burst animation. Track combo: popping within 3 seconds of last pop increases multiplier shown at top (×2, ×3, ×4) with pulsing animation that intensifies at higher multiplier levels. When multiplier reaches ×4, all remaining same-colored bubbles automatically pop.

Required libraries: react, tailwindcss, framer-motion

## Rubric

| #   | ID          | Description                                                                                | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ------------------------------------------------------------------------------------------ | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display colored bubbles in 5 rows at top                                                   | major  | The bubble grid provides the initial game board structure.                                   | None         |
| 2   | content     | Display bubbles in 3 colors: red, blue, green                                              | major  | The three color options enable match detection logic.                                        | None         |
| 3   | visual      | Display cannon at bottom center                                                            | major  | The cannon provides the visible shooting mechanism.                                          | None         |
| 4   | state       | Rotate cannon continuously to follow mouse cursor position                                 | major  | Continuous rotation tracking creates dynamic aiming state that updates frame-by-frame.       | None         |
| 5   | interaction | Shoot bubble toward cursor when clicked                                                    | major  | Click interaction triggers the projectile launch action.                                     | None         |
| 6   | state       | Animate bubble flying with smooth motion along trajectory                                  | major  | Flight animation represents time-evolving motion state as bubble travels toward target.      | C5           |
| 7   | state       | Attach shot bubble to grid and check for 3+ same-colored touching bubbles                  | major  | Collision attachment and match detection determine which bubble groups should pop.           | C6           |
| 8   | state       | Pop matched bubbles with burst animation                                                   | major  | Burst animation represents the pop action with time-evolving visual effect.                  | C7           |
| 9   | state       | Track time elapsed since last bubble pop                                                   | major  | Time tracking maintains timing state needed for combo window calculation.                    | C8           |
| 10  | state       | Increase multiplier (×2, ×3, ×4) when popping within 3 seconds of previous pop             | major  | Combo timing calculates derived multiplier state based on rapid sequential actions.          | C9           |
| 11  | content     | Display current multiplier value at top                                                    | major  | Multiplier text shows the active combo level.                                                | C10          |
| 12  | layout      | Position multiplier display at top of screen                                               | minor  | Top positioning makes combo status visible during gameplay.                                  | None         |
| 13  | state       | Apply pulsing scale animation to multiplier that intensifies at higher levels              | major  | Animation intensity proportional to multiplier creates visual feedback escalating with combo.| C11          |
| 14  | state       | Pop all remaining same-colored bubbles across board when multiplier reaches ×4             | major  | Multiplier threshold triggers automatic cascade clearing all matching bubbles simultaneously.| C10          |

## Justification

The bubble shooter works with layered complexity through cross-feature dependencies and cascading reactions. Colored bubbles (red, blue, green) display in 5 rows at top. Cannon at bottom center rotates continuously to follow mouse cursor position. Clicking shoots bubble with smooth flight animation toward cursor. Shot bubble attaches when colliding with existing bubble, triggering match detection for 3+ same-colored touching bubbles. Matched bubbles pop with burst animation. Combo system tracks time elapsed since last pop: popping within 3 seconds of previous pop increases chain multiplier (×2, ×3, ×4) displayed at top with pulsing animation that intensifies proportionally at higher multiplier levels. When multiplier reaches ×4, all remaining bubbles of the same color automatically pop across the entire board. Multiple systems interact: collision triggers match detection and pop, pop timing drives multiplier escalation, multiplier level drives animation intensity, ×4 threshold triggers board-wide cascade.
