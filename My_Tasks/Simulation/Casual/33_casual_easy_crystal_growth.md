Category: Simulation

Prompt style: Casual

Title: Crystal Growth Pattern

Prompt: Need a crystal growth simulator that shows how crystals form from a seed. Show a single blue seed crystal in the center of the screen with a "Grow" button and a "Clear" button positioned below it. When I click the Grow button, the crystal starts expanding outward from the seed in a branching pattern, with new crystalline structures forming in shades of blue and cyan radiating in multiple directions. When I click the Clear button, remove all grown crystal branches and return to just the original seed crystal.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                     | Weight | Rationale                                                                                                          | Dependent On |
| --- | ----------- | --------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display blue seed crystal                                       | major  | The seed crystal provides the origin point from which the entire growth pattern emerges.                           | None         |
| 2   | layout      | Position seed crystal at center of screen                       | minor  | Centering the seed creates equal space for growth to radiate in all directions.                                    | C1           |
| 3   | visual      | Display Grow button                                             | major  | The grow button gives users control to initiate the crystallization process.                                       | None         |
| 4   | layout      | Position Grow button below seed crystal                         | minor  | Placing the grow button below keeps it accessible while keeping focus on the crystal growth area.                  | C3           |
| 5   | visual      | Display Clear button                                            | major  | The clear button allows users to reset the simulation for repeated observations.                                   | None         |
| 6   | layout      | Position Clear button below seed crystal                        | minor  | Positioning the clear button below groups it with the grow button for logical control placement.                   | C5           |
| 7   | interaction | Expand crystal outward from seed when Grow clicked              | major  | Clicking grow triggers the crystallization animation that demonstrates the formation process.                      | C3           |
| 8   | state       | Create branching pattern radiating in multiple directions       | major  | Branching in multiple directions simulates the natural geometric growth of real crystal structures.                | C7           |
| 9   | visual      | Display new crystal structures in blue and cyan shades          | major  | Using blue and cyan colors creates visual distinction between different crystal formations and growth stages.      | C8           |
| 10  | state       | Grow crystal gradually over time                                | major  | Gradual growth allows users to observe the progressive nature of crystallization rather than instant appearance.   | C7           |
| 11  | interaction | Remove all grown branches and return to seed when Clear clicked | major  | Clearing the growth resets the visual state so users can start fresh simulations from the original seed.           | C5           |

## Justification

The crystal growth simulator provides an engaging visualization of crystallization processes. A blue seed crystal displays at the center of the screen with a Grow button and Clear button positioned below it. When users click the Grow button, the crystal begins expanding outward from the seed crystal in a branching pattern. New crystalline structures form gradually in shades of blue and cyan, radiating outward in multiple directions to simulate natural crystal geometry. The growth animation progresses over time, allowing observation of the formation process. When users click the Clear button, all grown crystal branches are removed and the display returns to just the original seed crystal, ready for another growth cycle.
