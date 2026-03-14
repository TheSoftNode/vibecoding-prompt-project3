Category: Data_Visualization

Prompt style: Casual

Title: Real-Time Data Streaming Chart

Prompt: Need a live chart that streams random CPU, Memory, and Network data (0-100 range) every second. Show three colored lines: CPU in blue, Memory in green, Network in orange. Keep exactly 30 points visible - when the 31st point arrives, remove the oldest point first before adding the new one. Add a pause/resume button below the chart that stops and restarts the stream. Put a stats panel to the right showing current values and rolling averages for all three metrics.

Required libraries: react, tailwindcss, recharts, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display line chart with three lines                   | major  | The chart provides the foundation for visualizing all three metrics simultaneously.                              | None         |
| 2   | visual      | Display CPU line in blue color                        | minor  | Blue color helps users identify the CPU metric visually.                                                         | None         |
| 3   | visual      | Display Memory line in green color                    | minor  | Green color helps users identify the Memory metric visually.                                                     | None         |
| 4   | visual      | Display Network line in orange color                  | minor  | Orange color helps users identify the Network metric visually.                                                   | None         |
| 5   | state       | Generate random data between 0-100 every second       | major  | Continuous random data generation creates the streaming effect for monitoring.                                   | None         |
| 6   | state       | Maintain exactly 30 data points visible on chart      | major  | The 30-point limit keeps the chart readable and focused on recent activity.                                      | C5           |
| 7   | state       | Remove oldest point before adding 31st point          | major  | Removing before adding ensures the count never exceeds 30, maintaining the sliding window correctly.             | C6           |
| 8   | content     | Display button labeled "Pause Stream" initially       | major  | The specific label tells users they can pause the streaming data.                                                | None         |
| 9   | layout      | Position button below the chart                       | minor  | Placing the button below separates controls from the visualization.                                              | None         |
| 10  | interaction | Stop data generation when button is clicked           | major  | Pausing lets users freeze the display to examine specific values.                                                | C8           |
| 11  | interaction | Change button text to "Resume Stream" when paused     | major  | The exact text "Resume Stream" indicates the paused state and how to continue.                                   | C10          |
| 12  | interaction | Restart data generation when "Resume Stream" is clicked | major  | Resuming allows users to continue monitoring after examining paused data.                                        | C11          |
| 13  | interaction | Change button text back to "Pause Stream" when resumed | major  | Reverting to "Pause Stream" confirms the stream is active again.                                                 | C12          |
| 14  | content     | Display most recent value for each metric in stats panel | major  | Recent values show the latest data point for each metric.                                                        | C5           |
| 15  | layout      | Position stats panel to the right of chart            | minor  | Right-side placement keeps stats visible alongside the streaming chart.                                          | None         |
| 16  | state       | Calculate rolling average from only visible 30 points for each metric | major  | Rolling averages must use only the current 30-point window, not all accumulated data.                            | C6, C7       |

## Justification

The Real-Time Data Streaming Chart achieved 56% pass rate (9/16 criteria) with specific failures across placement, labeling, and state management. The line chart displays correctly with three colored lines (CPU in blue, Memory in green, Network in orange), and random data generates every second between 0-100 as expected. However, the model failed C7 - instead of removing the oldest point before adding the 31st, it added first then removed, briefly showing 31 points which caused a visible flicker in the chart. The button functionality worked but failed C8 - it displayed "Pause" instead of the exact text "Pause Stream", and similarly failed C11 by showing "Resume" instead of "Resume Stream". The button was positioned to the right of the chart instead of below it (C9 failed). The stats box displayed with correct data but failed C15 - it was positioned below the chart instead of to the right of it, and critically failed C16 - the rolling averages calculated from all accumulated data points since page load rather than only from the visible 30-point window, causing the averages to become increasingly stable over time instead of responding to the recent 30-second trend. The pause/resume toggle functionality (C10, C12, C13) worked correctly, stopping and restarting data generation as expected.
