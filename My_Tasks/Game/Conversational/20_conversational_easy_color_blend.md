Category: Game

Prompt style: Conversational

Title: Color Blend Mixer

Prompt: I want to build a color mixing challenge game. At the top, display a target color box showing a randomly generated color. Below that, show three sliders labeled "Red", "Green", and "Blue" ranging from 0 to 255. Next to the sliders, display a preview box that updates to show the current mixed color as I move the sliders. When my mixed color matches the target color within a 10-point tolerance for each RGB value, display "Color Matched!" in bold text below the preview box and add 1 point to a score counter shown at the top. After a match, generate a new random target color automatically.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display a target color box at the top                    | major  | The target shows users the color they need to recreate.                            | None         |
| 2  | state       | Show randomly generated color in target box              | major  | Random colors create unpredictable challenges for each round.                      | None         |
| 3  | visual      | Display three sliders below target color                 | major  | The sliders provide the controls for mixing the color.                             | None         |
| 4  | content     | Label sliders "Red", "Green", and "Blue"                 | major  | The labels tell users which color component each slider controls.                  | C3           |
| 5  | state       | Set slider range from 0 to 255                           | major  | The 0-255 range matches standard RGB color values.                                 | None         |
| 6  | visual      | Display a preview box next to sliders                    | major  | The preview shows users their current mixed color result.                          | None         |
| 7  | interaction | Update preview box color as sliders move                 | major  | Real-time updates let users see their color mix as they adjust sliders.            | None         |
| 8  | state       | Match colors within 10-point tolerance for each RGB value | major  | The tolerance makes matching achievable without requiring perfect precision.       | None         |
| 9  | content     | Display "Color Matched!" when colors match               | major  | The success message tells users they achieved the target color.                    | None         |
| 10 | visual      | Display message in bold text below preview box           | minor  | Bold text makes the success message prominent.                                     | C9           |
| 11 | visual      | Display score counter at the top                         | major  | The score shows users their total successful matches.                              | None         |
| 12 | interaction | Add 1 point to score when color matches                  | major  | Scoring rewards users for successful color mixing.                                 | None         |
| 13 | state       | Generate new random target color after match             | major  | Auto-generating keeps the game progressing with new challenges.                    | None         |

## Justification

The Color Blend Mixer works as expected with real-time color mixing and matching validation. A target color box displays at the top showing a randomly generated color. A score counter appears at the top tracking successful matches. Below the target, three sliders labeled "Red", "Green", and "Blue" appear ranging from 0 to 255. Next to the sliders, a preview box displays that updates to show the current mixed color as users move the sliders. When the mixed color matches the target color within a 10-point tolerance for each RGB value, "Color Matched!" displays in bold text below the preview box and 1 point adds to the score counter. After a match, a new random target color generates automatically.
