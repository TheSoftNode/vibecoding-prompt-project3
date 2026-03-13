Category: Data_Visualization

Prompt style: Casual

Title: Real-Time Data Streaming Chart

Prompt: Build a live streaming line chart that updates with new random data points every second. Display three separate colored lines representing CPU (blue), Memory (green), and Network (orange) metrics with values between 0-100. Show the last 30 data points only, automatically removing the oldest point when a new one arrives. Include a pause/resume button that stops and restarts the data stream. Add a stats panel showing the current value and calculated average for each of the three metrics, updating in real-time as new data arrives.

Required libraries: react, tailwindcss, recharts, lucide-react, framer-motion

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display line chart canvas                             | major  | The chart provides the foundation for visualizing all the streaming data.                                        | None         |
| 2   | content     | Display "CPU" metric label                            | major  | Labels help users identify which line represents which system metric.                                            | None         |
| 3   | content     | Display "Memory" metric label                         | major  | Labels help users identify which line represents which system metric.                                            | None         |
| 4   | content     | Display "Network" metric label                        | major  | Labels help users identify which line represents which system metric.                                            | None         |
| 5   | visual      | Display CPU line in blue color                        | minor  | Color coding lets users quickly distinguish between different metrics.                                           | None         |
| 6   | visual      | Display Memory line in green color                    | minor  | Color coding lets users quickly distinguish between different metrics.                                           | None         |
| 7   | visual      | Display Network line in orange color                  | minor  | Color coding lets users quickly distinguish between different metrics.                                           | None         |
| 8   | state       | Generate random data points between 0-100 every second | major  | Continuous random data generation creates the streaming effect for monitoring.                                   | None         |
| 9   | state       | Maintain last 30 data points for each metric         | major  | The sliding window keeps the chart focused on recent data without overloading the display.                       | C8           |
| 10  | state       | Remove oldest point when new point arrives            | major  | Automatic removal ensures the chart always shows exactly the last 30 points.                                     | C9           |
| 11  | content     | Display pause/resume button                           | major  | The button gives users control over the data stream.                                                             | None         |
| 12  | interaction | Stop data stream when pause button is clicked         | major  | Pausing lets users freeze the display to examine specific values.                                                | C11          |
| 13  | interaction | Restart data stream when resume button is clicked     | major  | Resuming allows users to continue monitoring after examining paused data.                                        | C11, C12     |
| 14  | content     | Display stats panel with metric labels                | major  | The stats panel provides a dedicated area for numerical details.                                                 | None         |
| 15  | state       | Calculate current value for each metric               | major  | Current values show the latest data point for each metric.                                                       | C8           |
| 16  | state       | Calculate average value for each metric               | major  | Averages give users a sense of typical performance across the visible time window.                               | C9           |
| 17  | content     | Display current value for CPU in stats panel          | major  | Showing the exact current value helps users see precise numbers alongside the visual chart.                      | C15          |
| 18  | content     | Display current value for Memory in stats panel       | major  | Showing the exact current value helps users see precise numbers alongside the visual chart.                      | C15          |
| 19  | content     | Display current value for Network in stats panel      | major  | Showing the exact current value helps users see precise numbers alongside the visual chart.                      | C15          |
| 20  | content     | Display average value for CPU in stats panel          | major  | Showing the average helps users understand overall trends beyond momentary spikes.                               | C16          |
| 21  | content     | Display average value for Memory in stats panel       | major  | Showing the average helps users understand overall trends beyond momentary spikes.                               | C16          |
| 22  | content     | Display average value for Network in stats panel      | major  | Showing the average helps users understand overall trends beyond momentary spikes.                               | C16          |
| 23  | layout      | Position stats panel adjacent to chart                | minor  | Placing stats near the chart makes it easy to correlate numbers with visual trends.                              | None         |

## Justification

The Real-Time Data Streaming Chart achieved 52% pass rate with multiple complex failures across state management and interaction features. The line chart canvas displays correctly with three colored lines (CPU in blue, Memory in green, Network in orange) and proper metric labels. The stats panel appears adjacent to the chart with labels for all three metrics. However, the model failed to implement the critical sliding window behavior. The data points generated every second, but instead of maintaining exactly the last 30 points and removing the oldest when new ones arrive, the chart kept accumulating all data points indefinitely, causing the visualization to become increasingly compressed and unreadable over time. This dependency chain failure (C8→C9→C10) broke the core streaming concept. Additionally, the pause/resume functionality partially worked - clicking pause stopped the data stream as expected, but clicking resume failed to restart it properly, leaving the chart frozen. The stats panel displayed current values correctly for all three metrics, but the average calculations were incorrect, showing the mean of all accumulated data points rather than just the last 30 visible points. These interdependent failures across state management (sliding window + averages) and interaction (pause/resume) caused the overall 52% pass rate, demonstrating the complexity of coordinating real-time updates with proper data window management.
