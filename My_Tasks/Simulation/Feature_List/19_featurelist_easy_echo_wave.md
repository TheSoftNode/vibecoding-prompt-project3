Category: Simulation

Prompt style: Feature_List

Title: Echo Wave Propagator

Prompt: Build an echo wave propagator. Display a simulation area with a fixed center point. When the spacebar is pressed, create a circular wave ring that starts from the center and expands outward, growing in radius over 3 seconds before fading out completely. Allow multiple waves to exist simultaneously, with each new spacebar press creating an additional expanding wave ring. Display a counter showing the total number of waves created.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display simulation area                                   | major  | The area gives users a space to see the waves expanding.                                                         | None         |
| 2   | visual      | Display fixed center point                                | minor  | The center point shows users where each wave originates from.                                                    | None         |
| 3   | interaction | Create new wave ring when spacebar is pressed             | major  | Spacebar creates waves, giving users direct control over when ripples appear.                                    | None         |
| 4   | visual      | Display circular wave ring element                        | major  | The ring is what users watch to see the wave propagation effect.                                                 | None         |
| 5   | state       | Expand wave ring radius over 3 seconds                    | major  | The expanding motion creates the ripple effect spreading outward from center.                                    | None         |
| 6   | state       | Fade out wave ring after expansion completes              | major  | Fading makes old waves disappear so the screen doesn't get cluttered.                                            | C5           |
| 7   | state       | Allow multiple wave rings to exist simultaneously         | major  | Multiple waves let users create layered patterns with overlapping ripples.                                       | None         |
| 8   | state       | Track total number of waves created                       | minor  | Counting waves gives users feedback on how many times they pressed spacebar.                                     | None         |
| 9   | content     | Display counter showing total waves created               | minor  | The counter displays the running total so users can see their activity.                                          | C8           |
| 10  | layout      | Position center point in middle of simulation area        | minor  | Centering the origin point creates symmetric wave expansion in all directions.                                   | None         |

## Justification

The echo wave propagator works exactly as expected with spacebar-triggered expanding waves and simultaneous animation. A simulation area displays on screen with a fixed center point positioned in the middle. When users press the spacebar, a circular wave ring appears at the center point and expands outward, growing in radius continuously over 3 seconds before fading out completely. Each spacebar press creates a new wave ring, and multiple waves can exist at the same time, creating overlapping expanding circles. A counter displays on screen showing the total number of waves created, incrementing with each spacebar press.
