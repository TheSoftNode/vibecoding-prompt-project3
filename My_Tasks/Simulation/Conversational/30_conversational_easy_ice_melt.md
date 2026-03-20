Category: Simulation

Prompt style: Conversational

Title: Ice Cube Melting

Prompt: Need an ice cube melting simulator. Show an ice cube. When I click Melt, the cube shrinks gradually. Show a melt percentage.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                      | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | ------------------------------------------------ | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display ice cube                                 | major  | The ice cube is the object that melts in the simulation.                       | None         |
| 2   | visual      | Display Melt button                              | major  | The button gives users control to trigger the melting simulation.              | None         |
| 3   | interaction | Shrink ice cube when Melt button is clicked      | major  | Shrinking the cube simulates the melting process.                              | None         |
| 4   | state       | Gradually reduce cube size over time             | major  | Gradual reduction creates realistic melting animation.                         | C3           |
| 5   | content     | Display melt percentage                          | major  | Showing percentage gives users feedback on melting progress.                   | None         |
| 6   | state       | Calculate melt percentage based on cube size     | major  | Calculating percentage tracks how much of the cube has melted.                 | C5           |
| 7   | state       | Increase melt percentage as cube shrinks         | major  | Increasing percentage reflects the melting progress.                           | C6           |

## Justification

The ice cube melting simulator works exactly as expected for melting visualization. An ice cube displays with a Melt button. When users click the Melt button, the ice cube shrinks gradually over time simulating the melting process. A melt percentage displays and increases as the cube shrinks reflecting the melting progress.
