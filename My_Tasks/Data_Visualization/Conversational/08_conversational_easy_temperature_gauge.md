Category: Data Visualization

Prompt style: Conversational

Title: Temperature Gauge Indicator

Prompt: Build a simple gauge that shows the current temperature in London. Display a circular dial with a needle that points to a value between -10°C and 40°C. Color the dial red for temperatures above 25°C, blue for temperatures below 5°C, and gray for everything in between. Add a digital readout beneath the gauge showing the exact temperature number. Include a "Refresh" button that generates a new random temperature and updates both the needle position and digital readout to reflect the new value.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                                         | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display circular dial gauge                                      | major  | The circular dial provides the visual structure for showing temperature ranges.                                                   | None         |
| 2   | visual      | Display needle on the dial                                       | major  | The needle points to the temperature value giving users a quick visual reading.                                                   | C1           |
| 3   | state       | Calculate needle position based on temperature value between -10°C and 40°C | major  | Needle positioning is calculated based on the current temperature value within the range.                                         | None         |
| 4   | visual      | Display circular dial gauge in color based on temperature        | major  | The dial's color provides visual feedback about temperature zones.                                                                | C1           |
| 5   | state       | Determine dial color: red for above 25°C, blue for below 5°C, gray for in between | major  | Color determination is calculated based on temperature thresholds creating conditional visual feedback.                           | None         |
| 6   | content     | Display digital readout showing exact temperature number         | major  | The digital number tells users the precise temperature value in degrees.                                                          | None         |
| 7   | layout      | Position digital readout beneath the gauge                       | minor  | Placing the readout below keeps it visible without covering the dial.                                                             | None         |
| 8   | visual      | Display "Refresh" button                                         | major  | The refresh button gives users control to generate new temperature readings.                                                      | None         |
| 9   | interaction | Generate new random temperature when button is clicked           | major  | Clicking the button creates a random temperature value to simulate updates.                                                       | C8           |
| 10  | state       | Update needle position to reflect new temperature               | major  | Needle recalculates its position to point at the new temperature after refresh button is clicked.                                 | C3           |
| 11  | state       | Update digital readout to reflect new temperature               | major  | Digital number updates to show the new temperature value after refresh button is clicked.                                         | C6           |

## Justification

The temperature gauge indicator displays London's temperature through a circular dial with a needle pointing to values between -10°C and 40°C. The dial changes color based on temperature: red for above 25°C, blue for below 5°C, and gray for temperatures in between. A digital readout beneath the gauge shows the exact temperature number. When users click the "Refresh" button, a new random temperature is generated and both the needle position and digital readout update automatically to reflect the new value, demonstrating how the gauge responds to temperature changes.
