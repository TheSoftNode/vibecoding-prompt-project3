Category: Game

Prompt style: Conversational

Title: Color Blend Mixer

Prompt: I want to build a color mixing challenge game. At the top, display a target color box showing the color RGB(180, 90, 200) with its values labeled "Target RGB: [180, 90, 200]". Below that, show three sliders labeled "Red", "Green", and "Blue" ranging from 0 to 255, each displaying its current value. Next to the sliders, display a preview box that updates to show the current mixed color as I move the sliders. Below the preview box, display the current mixed RGB values labeled "Your RGB: [R, G, B]". When my mixed color is close enough to the target color, display "Perfect Match!" message in green. When getting closer but not close enough yet, display "Getting Close!" message in yellow.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                                   | Weight | Rationale                                                                                      | Dependent On |
|----|-------------|---------------------------------------------------------------|--------|------------------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display target color box at the top                           | major  | Showing the target box gives players the color goal they need to recreate.                     | None         |
| 2  | visual      | Show color RGB(180, 90, 200) in target box                    | major  | Displaying the specific target color establishes the mixing goal players aim for.              | C1           |
| 3  | content     | Display label "Target RGB: [180, 90, 200]"                    | major  | Showing target RGB values helps players understand the exact goal numerically.                 | C2           |
| 4  | visual      | Display three sliders below target color                      | major  | Showing sliders gives players the controls to build their color mix.                           | None         |
| 5  | content     | Display labels "Red", "Green", "Blue" on sliders              | major  | Showing labels identifies which color component each slider adjusts.                           | C4           |
| 6  | state       | Set slider range from 0 to 255                                | major  | Setting range to 0-255 matches standard RGB color values for mixing.                           | C4           |
| 7  | content     | Display current value on each slider                          | major  | Showing values tells players the exact RGB number they are setting.                            | C4           |
| 8  | layout      | Position preview box next to sliders                          | minor  | Placing preview next to sliders keeps color result visible while adjusting.                    | None         |
| 9  | interaction | Update preview box to show current mixed color as sliders move| major  | Updating preview in real time shows players their current color mix as they adjust.            | C4           |
| 10 | content     | Display label "Your RGB: [R, G, B]" showing current mix       | major  | Showing current RGB values helps players compare their mix to the target numerically.          | C9           |
| 11 | state       | Check if mixed color is close enough to target                | major  | Determining closeness tells players if they achieved a good enough match.                      | C9           |
| 12 | content     | Display "Perfect Match!" in green when close enough           | major  | Showing success message tells players they matched the target color well enough.               | C11          |
| 13 | state       | Check if getting closer but not close enough yet              | major  | Checking progress state provides feedback when players are approaching but not there yet.      | C9           |
| 14 | content     | Display "Getting Close!" in yellow when closer but not matched| major  | Showing progress message encourages players by showing they are moving toward the target.      | C13          |

## Justification

The color blend mixer game works as expected for RGB color matching challenges. A target color box displays at the top showing the color RGB(180, 90, 200) with its values labeled "Target RGB: [180, 90, 200]". Below that, three sliders display labeled "Red", "Green", and "Blue" ranging from 0 to 255, each displaying its current value. A preview box positioned next to the sliders displays and updates to show the current mixed color as players move the sliders. Below the preview box, the current mixed RGB values display labeled "Your RGB: [R, G, B]". When the mixed color is close enough to the target color, "Perfect Match!" message displays in green. When getting closer but not close enough yet, "Getting Close!" message displays in yellow.
