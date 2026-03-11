Category: Simulation

Prompt style: Terse

Title: Rainfall Simulator

Prompt: Rain animation. Blue droplets fall from top to bottom continuously at random horizontal positions. Slider labeled "Rain Intensity" controls number of active droplets (10-100). Dragging slider updates droplet count in real-time.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                              | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | -------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display droplet elements                                 | major  | Droplets are the visual particles that represent falling rain in the simulation.                                 | None         |
| 2   | content     | Display droplets in blue color                           | minor  | Blue color makes droplets recognizable as water/rain rather than other particles.                                | None         |
| 3   | state       | Animate droplets falling from top to bottom              | major  | Downward animation creates the rainfall motion that defines the simulation.                                      | None         |
| 4   | state       | Run animation continuously without stopping              | major  | Continuous animation maintains the ongoing rainfall effect.                                                      | None         |
| 5   | state       | Randomize horizontal starting positions for droplets     | major  | Random horizontal positions create natural-looking scattered rainfall instead of vertical columns.               | None         |
| 6   | visual      | Display slider control                                   | major  | The slider provides the interface for adjusting rain intensity.                                                  | None         |
| 7   | content     | Display label "Rain Intensity" on slider                 | minor  | Labeling clarifies that the slider controls how heavy the rainfall is.                                           | None         |
| 8   | content     | Display slider range from 10 to 100                      | minor  | Showing the range tells users the minimum and maximum droplet counts they can set.                               | None         |
| 9   | state       | Control droplet count based on slider value              | major  | Linking droplet count to slider value makes the intensity setting affect the visible rainfall.                   | None         |
| 10  | interaction | Update droplet count in real-time when slider is dragged | major  | Real-time updates let users see the rain intensity change immediately as they adjust the slider.                 | C6           |
| 11  | layout      | Position slider below the rain simulation area           | minor  | Placing the slider below keeps controls separate from the visual simulation space.                               | None         |

## Justification

The application achieved a 90.91% pass rate with one specific failure. Blue droplet elements display and animate continuously, falling from top to bottom. Each droplet starts at a random horizontal position, creating a scattered rainfall pattern. A slider labeled "Rain Intensity" shows a range from 10 to 100. The slider controls the number of active droplets in the simulation. As users drag the slider, the droplet count updates in real-time, making the rain heavier or lighter based on the slider value. However, the model failed to position the slider below the rain simulation area. Instead, the slider appears to the right of the simulation or above it in a control bar, not below as required. This positioning issue caused the failure despite all other functionality working correctly.
