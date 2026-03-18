Category: Game

Prompt style: Conversational

Title: Tile Flip Challenge

Prompt: I want to build a tile flipping game. Display 8 square tiles arranged in two rows of 4. Each tile starts gray. When I click a tile, it flips to blue and stays blue. Display a move counter labeled "Moves: 0" at the top that increments each time I click any tile. When all 8 tiles are flipped to blue, display "Complete!" message in bold text and disable further clicking.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 8 square tiles                               | major  | Showing tiles gives players the objects they need to flip.                                   | None         |
| 2   | layout      | Arrange tiles in two rows of 4                       | minor  | Arranging in rows creates an organized grid layout for the flipping game.                    | C1           |
| 3   | state       | Initialize each tile as gray                         | minor  | Setting initial gray state establishes the unflipped condition players will change.          | None         |
| 4   | visual      | Display each tile in gray color initially            | minor  | Showing gray color makes the initial unflipped state visible to players.                     | C3           |
| 5   | interaction | Flip tile to blue when clicked                       | major  | Clicking tile changes its color showing the flipping action.                                 | C1           |
| 6   | state       | Keep tile blue after flipping                        | major  | Maintaining blue color shows the tile stays flipped and won't revert.                        | C5           |
| 7   | content     | Display move counter labeled "Moves: 0"              | minor  | Showing counter tells players how many flips they've made.                                   | None         |
| 8   | layout      | Position move counter at top                         | minor  | Top positioning keeps counter visible while players flip tiles below.                        | C7           |
| 9   | state       | Increment move counter when tile clicked             | major  | Incrementing count tracks the total number of moves the player makes.                        | C5           |
| 10  | content     | Update displayed move count after each click         | minor  | Updating display shows players their flip count in real time.                                | C9           |
| 11  | state       | Detect when all 8 tiles are blue                     | major  | Checking completion determines when the player has flipped every tile.                       | C6           |
| 12  | content     | Display "Complete!" message when all flipped         | major  | Showing message tells players they successfully flipped all tiles.                           | C11          |
| 13  | visual      | Display "Complete!" in bold text                     | minor  | Bold formatting makes the completion message prominent and celebratory.                      | C12          |
| 14  | interaction | Disable tile clicking after completion               | major  | Disabling clicks prevents further flipping once the challenge is complete.                   | C11          |

## Justification

The tile flip challenge game works as expected for simple clicking gameplay with completion detection. Eight square tiles display arranged in two rows of 4, each starting as gray color. A move counter labeled "Moves: 0" displays positioned at the top. When players click a tile, it flips to blue and stays blue. The game detects each tile click, increments the move counter, and updates the displayed count after each click. When all 8 tiles are flipped to blue, the game detects completion, displays "Complete!" message in bold text, and disables further tile clicking.
