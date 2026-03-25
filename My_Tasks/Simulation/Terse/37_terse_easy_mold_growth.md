Category: Simulation

Prompt style: Terse

Title: Mold Colony Growth

Prompt: Click bread to plant spore. Green-gray mold spreads across tan surface. Show colony count.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                  | Weight | Rationale                                                         | Dependent On |
| --- | ----------- | -------------------------------------------- | ------ | ----------------------------------------------------------------- | ------------ |
| 1   | visual      | Display tan bread surface background         | major  | Tan surface represents bread substrate where mold grows.          | None         |
| 2   | interaction | Plant mold spore at clicked position         | major  | Click plants spore to initiate fungal growth at chosen location.  | None         |
| 3   | visual      | Display mold in green-gray color             | major  | Green-gray color represents typical bread mold appearance.        | C2           |
| 4   | state       | Spread mold outward from spore origin        | major  | Outward spreading simulates fungal colony expansion.              | C2           |
| 5   | state       | Animate mold growth continuously             | major  | Continuous growth represents ongoing fungal propagation.          | C4           |
| 6   | content     | Display colony count                         | major  | Colony count shows number of separate mold growths planted.       | None         |
| 7   | state       | Increment colony count when new spore planted| major  | Counting each planted spore tracks total colonies started.        | C6           |
| 8   | state       | Allow multiple colonies to grow simultaneously| major  | Multiple simultaneous colonies show independent fungal growth.    | None         |

## Justification

The mold colony growth simulator demonstrates fungal propagation on bread. A tan bread surface displays as the background. When users click anywhere on the bread, a mold spore plants at that position. Green-gray mold spreads outward continuously from each spore origin point, simulating colony expansion. Users can click multiple times to create several independent colonies growing simultaneously. A colony count displays and increments each time a new spore is planted.
