Category: Multimedia_Editing

Prompt style: Casual

Title: Paint Splatter Chain

Prompt: Need a paint splatter editor. Click a color dot to splatter paint outward to all touching dots of the same color. Show a splatter count and undo button.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                 | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display canvas with color dots                              | major  | The canvas with dots provides the surface where users apply splatter effects.                                    | None         |
| 2   | visual      | Display dots in multiple colors                             | major  | Multiple colors enable chain reactions to spread only through matching color groups.                             | C1           |
| 3   | layout      | Position dots touching each other                           | major  | Touching dots create the adjacency needed for splatter chains to spread between neighbors.                       | C1           |
| 4   | interaction | Splatter clicked dot when user clicks it                    | major  | Clicking a dot initiates the splatter effect on that starting point.                                             | None         |
| 5   | state       | Spread splatter to all touching same-color dots             | major  | Spreading to touching same-color dots creates the chain reaction effect.                                         | C4           |
| 6   | state       | Change splatted dots to show paint effect                   | major  | Visual change shows which dots have been affected by the splatter.                                               | C5           |
| 7   | content     | Display splatter count                                      | major  | Showing count gives users feedback on how many splatter actions they've performed.                               | None         |
| 8   | state       | Increment splatter count with each click                    | major  | Counting each splatter action tracks the user's editing activity.                                                | C7           |
| 9   | visual      | Display undo button                                         | major  | Showing undo button gives users control to reverse splatter mistakes.                                            | None         |
| 10  | layout      | Position undo button in accessible location                 | minor  | Placing undo button accessibly lets users quickly reach the control when needed.                                 | C9           |
| 11  | interaction | Reverse last splatter action when undo clicked              | major  | Clicking undo removes the most recent splatter so users can fix errors.                                          | C9           |
| 12  | state       | Restore dots to pre-splatter state when undone              | major  | Restoring dot appearance returns them to how they looked before the last splatter.                               | C11          |
| 13  | state       | Decrement splatter count when undo clicked                  | major  | Decreasing count reflects that one splatter action has been reversed.                                            | C11          |

## Justification

The Paint Splatter Chain editor lets users create chain reaction splatter effects by clicking color dots. A canvas displays with multiple colored dots positioned touching each other. When users click a dot, it splatters paint outward to all touching dots of the same color, changing their appearance to show the paint effect. A splatter count displays and increments with each click to track editing activity. An undo button displays in an accessible location. When users click undo, it reverses the last splatter action by restoring dots to their pre-splatter state and decrementing the splatter count.
