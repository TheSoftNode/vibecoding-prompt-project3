Category: Game

Prompt style: Conversational

Title: Color Blend Mixer

Prompt: I want to build a color mixing challenge game. At the top, display a target color box showing the color RGB(180, 90, 200) with its values labeled "Target RGB: [180, 90, 200]". Below that, show three sliders labeled "Red", "Green", and "Blue" ranging from 0 to 255, each displaying its current value. Next to the sliders, display a preview box that updates to show the current mixed color as I move the sliders. Below the preview box, display the current mixed RGB values labeled "Your RGB: [R, G, B]". Display an attempt counter labeled "Attempts: 0" at the bottom. Every time I adjust any slider, increment the attempt counter by 1 to track how many adjustments I make.

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
| 11 | content     | Display attempt counter labeled "Attempts: 0" at bottom       | major  | Showing attempt counter lets players track how many adjustments they make.                     | None         |
| 12 | interaction | Detect when any slider is adjusted                            | major  | Detecting slider adjustments triggers the attempt counting mechanism.                          | C4           |
| 13 | state       | Increment attempt counter by 1 when slider adjusted           | major  | Incrementing counter tracks total number of adjustments players make while mixing.             | C12          |
| 14 | content     | Update displayed attempt count after increment                | major  | Updating display shows players their current attempt count in real time.                       | C13          |

## Justification

The color blend mixer game works as expected for RGB color matching with attempt tracking. A target color box displays at the top showing the color RGB(180, 90, 200) with its values labeled "Target RGB: [180, 90, 200]". Below that, three sliders display labeled "Red", "Green", and "Blue" ranging from 0 to 255, each displaying its current value. A preview box positioned next to the sliders displays and updates to show the current mixed color as players move the sliders. Below the preview box, the current mixed RGB values display labeled "Your RGB: [R, G, B]". An attempt counter labeled "Attempts: 0" displays at the bottom. Every time players adjust any slider, the app detects the adjustment, increments the attempt counter by 1, and updates the displayed count.
