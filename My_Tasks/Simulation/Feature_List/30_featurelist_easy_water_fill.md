Category: Simulation

Prompt style: Feature_List

Title: Water Tank Fill

Prompt: Build a water tank fill simulator. Display an empty tank. When clicking Fill, water rises from bottom to top. Display fill level percentage.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                      | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | ------------------------------------------------ | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display empty tank                               | major  | The tank provides the container where water fills.                             | None         |
| 2   | visual      | Display Fill button                              | major  | The button gives users control to trigger the filling simulation.              | None         |
| 3   | interaction | Start water rise when Fill button is clicked     | major  | Clicking Fill initiates the water filling process.                             | None         |
| 4   | state       | Rise water level from bottom to top              | major  | Bottom-to-top rising simulates water filling the tank.                         | C3           |
| 5   | visual      | Display water inside tank                        | major  | Visible water shows the filling progress.                                      | C4           |
| 6   | content     | Display fill level percentage                    | major  | Showing percentage gives users feedback on how full the tank is.               | None         |
| 7   | state       | Calculate fill percentage based on water height  | major  | Calculating percentage tracks how much of the tank is filled.                  | C6           |
| 8   | state       | Increase fill percentage as water rises          | major  | Increasing percentage reflects the filling progress.                           | C7           |

## Justification

The water tank fill simulator works exactly as expected for tank filling visualization. An empty tank displays with a Fill button. When users click the Fill button, water rises from bottom to top filling the tank. Visible water displays inside the tank showing the filling progress. A fill level percentage displays and increases as water rises reflecting how full the tank is.
