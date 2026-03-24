Category: Simulation

Prompt style: Casual

Title: Candle Flame Flicker

Prompt: Animated candle flame that flickers naturally. Single orange flame on white candle, random subtle movements, wind slider at bottom changes intensity.

Required libraries: react, tailwindcss, framer-motion

## Rubric

| #   | ID          | Description                                                             | Weight | Rationale                                                                                                             | Dependent On |
| --- | ----------- | ----------------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display white candle body                                               | major  | The candle body provides the base structure from which the flame appears to burn.                                     | None         |
| 2   | visual      | Display orange flame on top of candle                                   | major  | Orange flame creates the primary visual element that users watch for realistic flickering behavior.                   | None         |
| 3   | layout      | Position flame centered on top of candle body                           | minor  | Centering the flame on the candle creates natural candle appearance where fire sits at the wick.                      | None         |
| 4   | state       | Animate flame with random subtle flickering movements                   | major  | Random flickering simulates the natural chaotic motion of real candle flames responding to air currents.              | None         |
| 5   | state       | Continuously animate flame movement throughout simulation                | major  | Continuous animation keeps the flame alive with persistent motion that represents ongoing combustion.                 | C4           |
| 6   | visual      | Display horizontal slider control                                       | major  | The slider provides interactive control for users to adjust wind intensity affecting the flame.                       | None         |
| 7   | content     | Label slider as "Wind" or "Wind Intensity"                              | minor  | The wind label clearly communicates that the slider controls environmental wind strength.                             | None         |
| 8   | layout      | Position slider at bottom of screen                                     | minor  | Bottom placement keeps the control accessible while leaving the candle and flame prominently visible above.           | None         |
| 9   | interaction | Adjust flame flicker intensity when slider value changes                | major  | Changing flicker intensity based on slider input lets users see how wind strength affects flame stability.            | C6           |
| 10  | state       | Increase flame movement amplitude as wind intensity increases           | major  | Greater movement at higher wind values creates realistic response where stronger winds make flames dance more wildly. | C9           |

## Justification

The candle flame flicker simulation creates a realistic animated candle with natural flame behavior. A white candle body displays vertically with an orange flame positioned on top at the center where a wick would be. The flame animates continuously with random subtle flickering movements that simulate natural air currents affecting real candles. At the bottom, a horizontal slider labeled "Wind" or "Wind Intensity" allows users to control environmental conditions. As users drag the slider to increase wind intensity, the flame responds by flickering more dramatically with larger movement amplitude, while lower wind values produce gentler, more stable flame motion.
