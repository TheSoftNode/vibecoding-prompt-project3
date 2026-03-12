Category: Simulation

Prompt style: Feature_List

Title: Echo Wave Propagator

Prompt: Build an echo wave propagator. Display a simulation area with a center point labeled "Origin". When the spacebar is pressed, create a circular wave ring that starts from the center and expands outward, growing in radius over 3 seconds before fading out. Allow multiple waves to exist at the same time, with each spacebar press creating an additional wave ring.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display simulation area with center point                 | major  | The simulation area with center point gives users the space and starting location for waves.                     | None         |
| 2   | content     | Display label "Origin" on center point                    | minor  | The label identifies the wave starting location.                                                                 | None         |
| 3   | interaction | Create circular wave ring when spacebar is pressed        | major  | Spacebar creates waves, giving users direct control over when ripples appear.                                    | None         |
| 4   | visual      | Display wave ring starting from center                    | major  | The wave ring appears at the center point where waves originate.                                                 | None         |
| 5   | state       | Expand wave ring radius over 3 seconds                    | major  | The expanding motion creates the ripple effect spreading outward from center.                                    | None         |
| 6   | state       | Fade out wave ring after 3 seconds                        | major  | Fading makes old waves disappear so the screen doesn't get cluttered.                                            | None         |
| 7   | state       | Allow multiple wave rings to exist at the same time       | major  | Multiple waves let users create layered patterns with overlapping ripples.                                       | None         |
| 8   | layout      | Position center point in middle of simulation area        | minor  | Centering the origin point creates symmetric wave expansion in all directions.                                   | None         |

## Justification

The echo wave propagator works exactly as expected with spacebar-triggered expanding waves and simultaneous animation. A simulation area displays on screen with a center point labeled "Origin" positioned in the middle. When users press the spacebar, a circular wave ring appears at the center point and expands outward, growing in radius continuously over 3 seconds before fading out. Each spacebar press creates a new wave ring, and multiple waves can exist at the same time, creating overlapping expanding circles.
