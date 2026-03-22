Category: Game

Prompt style: Terse

Title: Tile Pattern Matcher

Prompt: Click two tiles to flip. Matching patterns stay flipped. Show match count at top.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                   | Weight | Rationale                                                                 | Dependent On |
| --- | ----------- | --------------------------------------------- | ------ | ------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display grid of tiles                         | major  | Tile grid provides the structure for the matching game.                   | None         |
| 2   | visual      | Display tiles in face-down state              | major  | Face-down state hides patterns before players flip them.                  | C1           |
| 3   | interaction | Flip tile when clicked                        | major  | Clicking flips a tile to reveal its pattern.                              | None         |
| 4   | visual      | Show pattern on flipped tile                  | major  | Pattern display shows what the tile contains.                             | C3           |
| 5   | state       | Detect when two tiles are flipped             | major  | Detecting two flipped tiles determines when to check for a match.         | C3           |
| 6   | state       | Keep tiles flipped if patterns match          | major  | Keeping matched tiles flipped rewards successful pattern matching.        | C5           |
| 7   | state       | Flip tiles back if patterns don't match       | major  | Flipping back non-matching tiles resets the attempt.                      | C5           |
| 8   | content     | Display match count                           | minor  | Showing count gives users feedback on successful matches.                 | None         |
| 9   | layout      | Position match count at top of screen         | minor  | Top positioning keeps count visible without blocking the tiles.           | C8           |
| 10  | state       | Increment match count when patterns match     | major  | Counting each match tracks the player's progress.                         | C6           |

## Justification

The tile pattern matcher game works as expected for memory-based matching gameplay with scoring. A grid of tiles displays in face-down state. When players click a tile, it flips showing its pattern. When two tiles are flipped, the game detects whether their patterns match. If patterns match, the tiles stay flipped. If patterns don't match, the tiles flip back. A match count displays at the top of the screen and increments each time patterns match tracking the player's matching performance.
