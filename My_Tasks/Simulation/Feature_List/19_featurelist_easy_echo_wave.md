Category: Simulation

Prompt style: Feature_List

Title: Echo Wave Propagator

Prompt: Build an echo wave propagator. Display a simulation area with a center point labeled "Origin". Below the simulation, show a button labeled "Create Wave". When the button is clicked, create a circular wave ring that starts from the center and expands outward, growing in radius over 3 seconds before fading out. Allow multiple waves to exist at the same time, with each button click creating an additional wave ring.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display simulation area with center point                 | major  | The simulation area with center point gives users the space and starting location for waves.                     | None         |
| 2   | content     | Display label "Origin" on center point                    | minor  | The label identifies the wave starting location.                                                                 | None         |
| 3   | content     | Display button labeled "Create Wave"                      | major  | The button text tells users how to trigger wave creation.                                                        | None         |
| 4   | interaction | Create circular wave ring when button is clicked          | major  | Clicking the button creates waves, giving users direct control over when ripples appear.                         | C3           |
| 5   | state       | Start wave ring from center point                         | minor  | Starting from center creates waves that expand outward symmetrically.                                            | None         |
| 6   | state       | Expand wave ring radius over 3 seconds                    | major  | The expanding motion creates the ripple effect spreading outward from center.                                    | None         |
| 7   | state       | Fade out wave ring after 3 seconds                        | major  | Fading makes old waves disappear so the screen doesn't get cluttered.                                            | None         |
| 8   | state       | Allow multiple wave rings to exist at the same time       | major  | Multiple waves let users create layered patterns with overlapping ripples.                                       | None         |
| 9   | layout      | Position button below simulation area                     | minor  | Placing button below keeps controls separate from the wave display.                                              | None         |
| 10  | layout      | Position center point in middle of simulation area        | minor  | Centering the origin point creates symmetric wave expansion in all directions.                                   | None         |

## Justification

The echo wave propagator achieved a 90% pass rate with one specific failure. A simulation area displays on screen with a center point labeled "Origin" positioned in the middle. Below the simulation, a button labeled "Create Wave" displays on screen. When users click the button, a circular wave ring appears and expands outward, growing in radius continuously over 3 seconds before fading out. Each button click creates a new wave ring, and multiple waves can exist at the same time, creating overlapping expanding circles. However, the model failed to start the wave ring from the center point. Instead, the wave appears to originate from a different location on the canvas, not from the labeled "Origin" center point as required. This positioning issue caused the failure despite all other wave animation and simultaneous wave functionality working correctly.
