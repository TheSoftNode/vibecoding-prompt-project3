Category: Game

Prompt style: Conversational

Title: Tile Flip Challenge

Prompt: I want to build a tile flipping game. Display 8 square tiles arranged in two rows of 4. Each tile starts gray. When I click a tile, it flips to blue and stays blue. Display a move counter labeled "Moves: 0" at the top that increments each time I click any tile. When all 8 tiles are flipped to blue, display "Complete!" message in bold text and disable further clicking.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display 8 square tiles                                    | major  | Showing tiles gives players the objects they need to flip.                                       | None         |
| 2   | layout      | Arrange tiles in two rows of 4                            | minor  | Arranging in rows creates an organized grid layout for the flipping game.                        | C1           |
| 3   | visual      | Display each tile in gray color initially                 | minor  | Showing gray color makes the initial unflipped state visible to players.                         | None         |
| 4   | interaction | Flip tile to blue when clicked                            | major  | Clicking tile changes its color showing the flipping action.                                     | C1           |
| 5   | state       | Keep tile blue after flipping                             | major  | Maintaining blue color shows the tile stays flipped and won't revert.                            | C4           |
| 6   | content     | Display move counter labeled "Moves: 0"                   | minor  | Showing counter tells players how many flips they've made.                                       | None         |
| 7   | layout      | Position move counter at top                              | minor  | Top positioning keeps counter visible while players flip tiles below.                            | C6           |
| 8   | state       | Increment move counter when tile clicked                  | major  | Incrementing count tracks the total number of moves the player makes.                            | C4           |
| C8  |
| 10  | state       | Detect when all 8 tiles are blue                          | major  | Checking completion determines when the player has flipped every tile.                           | C5           |
| 11  | content     | Display "Complete!" message in bold text when all flipped | major  | Showing bold completion message makes it prominent and tells players they successfully finished. | C10          |
| 12  | interaction | Disable tile clicking after completion                    | major  | Disabling clicks prevents further flipping once the challenge is complete.                       | C10          |

## Justification

The tile flip challenge game works exactly as expected for clicking gameplay with move tracking. Eight square tiles display in gray color arranged in two rows of 4. A move counter labeled "Moves: 0" displays positioned at the top. When players click a tile, it flips to blue and stays blue. The move counter increments and the displayed count updates after each click. When all 8 tiles are flipped to blue, "Complete!" message displays in bold text and tile clicking becomes disabled.
