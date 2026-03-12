Category: Simulation

Prompt style: Feature_List

Title: Echo Wave Propagator

Prompt: Build an echo wave propagator. Display a simulation area with a center point labeled "Origin". When the spacebar is pressed, create a circular wave ring that starts from the center and expands outward, growing in radius over 3 seconds before fading out. Allow multiple waves to exist at the same time, with each spacebar press creating an additional wave ring.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display simulation area                                   | major  | The simulation area gives users space to see the wave animations.                                                | None         |
| 2   | visual      | Display center point                                      | minor  | The center point shows users where waves originate from.                                                         | None         |
| 3   | content     | Display label "Origin" on center point                    | minor  | The label identifies the wave starting location.                                                                 | None         |
| 4   | interaction | Create new wave ring when spacebar is pressed             | major  | Spacebar creates waves, giving users direct control over when ripples appear.                                    | None         |
| 5   | state       | Expand wave ring radius over 3 seconds                    | major  | The expanding motion creates the ripple effect spreading outward from center.                                    | None         |
| 6   | state       | Fade out wave ring after expansion completes              | major  | Fading makes old waves disappear so the screen doesn't get cluttered.                                            | C5           |
| 7   | state       | Allow multiple wave rings to exist at the same time       | major  | Multiple waves let users create layered patterns with overlapping ripples.                                       | None         |
| 8   | layout      | Position center point in middle of simulation area        | minor  | Centering the origin point creates symmetric wave expansion in all directions.                                   | None         |

## Justification

The echo wave propagator works exactly as expected with spacebar-triggered expanding waves and simultaneous animation. A simulation area displays on screen with a center point labeled "Origin" positioned in the middle. When users press the spacebar, a circular wave ring appears at the center point and expands outward, growing in radius continuously over 3 seconds before fading out. Each spacebar press creates a new wave ring, and multiple waves can exist at the same time, creating overlapping expanding circles.
