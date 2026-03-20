Category: Simulation

Prompt style: Casual

Title: Bounce Ball Drop

Prompt: Need a ball drop simulator. Click to drop a ball that bounces when it hits the ground. Show bounce count.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                    | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | ---------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display ground line at bottom                  | major  | The ground provides the surface where the ball bounces.                        | None         |
| 2   | visual      | Display ball                                   | major  | The ball is the object users interact with for the simulation.                 | None         |
| 3   | interaction | Drop ball when clicked                         | major  | Clicking drops the ball to initiate the bounce simulation.                     | None         |
| 4   | state       | Move ball downward after drop                  | major  | Downward movement simulates gravity pulling the ball toward the ground.        | C3           |
| 5   | interaction | Bounce ball upward when it hits ground         | major  | Bouncing upward when hitting ground simulates ball physics.                    | C4           |
| 6   | content     | Display bounce count                           | major  | Showing count gives users feedback on how many bounces occurred.               | None         |
| 7   | state       | Increment bounce count each time ball bounces  | major  | Counting each bounce tracks the simulation activity.                           | C6           |

## Justification

The bounce ball drop simulator works exactly as expected for ball physics visualization. A ground line displays at the bottom with a ball above it. When users click, the ball drops downward moving toward the ground. When the ball hits the ground, it bounces upward. A bounce count displays and increments each time the ball bounces.
