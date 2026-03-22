Category: Game

Prompt style: Conversational

Title: Color Mixer Challenge

Prompt: I need a color mixing game. Click two color orbs to mix them into a new color. Show mix count.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                      | Weight | Rationale                                                                  | Dependent On |
| --- | ----------- | ------------------------------------------------ | ------ | -------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display color orbs                               | major  | Showing color orbs gives players the elements they need to mix.            | None         |
| 2   | visual      | Display orbs in initial colors                   | major  | Initial colors provide the starting palette for mixing.                    | C1           |
| 3   | interaction | Select first orb when clicked                    | major  | Clicking selects the first orb for mixing.                                 | None         |
| 4   | visual      | Show selection indicator on first orb            | major  | Selection indicator shows which orb is selected.                           | C3           |
| 5   | interaction | Select second orb when clicked                   | major  | Clicking another orb selects the second orb to complete the mix.           | C3           |
| 6   | state       | Mix colors of two selected orbs                  | major  | Mixing colors creates the color combination mechanic.                      | C5           |
| 7   | visual      | Display new color orb after mixing               | major  | New orb shows the result of the color mixing.                              | C6           |
| 8   | content     | Display mix count                                | minor  | Showing count gives users feedback on how many mixes they created.         | None         |
| 9   | layout      | Position mix count at top of screen              | minor  | Top positioning keeps count visible without blocking the orbs.             | C8           |
| 10  | state       | Increment mix count when colors mixed            | major  | Counting each mix tracks the player's mixing activity.                     | C6           |

## Justification

The color mixer challenge game works as expected for color mixing gameplay with scoring. Color orbs display in initial colors. When players click an orb, it gets selected showing a selection indicator. When players click a second orb, the game mixes the colors of the two selected orbs. A new color orb appears displaying the mixed result. A mix count displays at the top of the screen and increments each time colors are mixed tracking the player's mixing performance.
