Category: Data_Visualization

Prompt style: Feature_List

Title: Memory Usage Bubbles

Prompt: Build a memory usage bubble chart that visualizes application RAM consumption. Display 5 circular bubbles arranged in a scattered pattern representing Chrome, Slack, VSCode, Spotify, and Docker. Load initial memory data with varied RAM consumption levels. Size each bubble proportionally to its memory usage with larger bubbles for higher RAM consumption. Display the application name inside each bubble and the memory amount below the application name. Color bubbles consuming above 1 GB in red and bubbles consuming below 1 GB in green. When users click any bubble, that bubble calculates and displays its exact memory percentage of total 8 GB RAM next to it.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                  | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | ------------------------------------------------------------ | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display 5 circular bubbles                                   | major  | Bubbles provide the visual structure for memory usage display.                 | None         |
| 2   | layout      | Arrange bubbles in scattered pattern                         | minor  | Scattered arrangement creates a bubble chart layout.                           | C1           |
| 3   | content     | Display app names: Chrome, Slack, VSCode, Spotify, Docker    | major  | App names identify which application each bubble represents.                   | None         |
| 4   | layout      | Position app names inside bubbles                            | minor  | Inside positioning shows the app label within the visual bubble.               | C3           |
| 5   | state       | Load initial memory data with varied RAM consumption levels  | major  | Loading memory data initializes the bubble values for visualization.           | None         |
| 6   | content     | Display memory amounts on bubbles                            | major  | Memory values show the exact RAM consumption for each app.                     | C5           |
| 7   | layout      | Position memory amount below app name                        | minor  | Below positioning shows the numeric value under the app label.                 | C6           |
| 8   | visual      | Size bubble proportionally to memory usage                   | major  | Proportional sizing visually represents the RAM consumption amount.            | C5           |
| 9   | visual      | Color bubbles above 1 GB red                                 | major  | Red color helps users identify apps with high memory usage.                    | None         |
| 10  | visual      | Color bubbles below 1 GB green                               | major  | Green color helps users identify apps with low memory usage.                   | None         |
| 11  | state       | Calculate memory percentage from total 8 GB RAM              | major  | Calculation converts GB usage to percentage of total RAM.                      | C5           |
| 12  | interaction | Display memory percentage next to bubble when clicked        | major  | Percentage shows the bubble's share of total system RAM.                       | C11          |

## Justification

The memory usage bubbles work exactly as expected for visualizing application RAM consumption with proportional sizing. Five circular bubbles display arranged in a scattered pattern with application names represented positioned inside each bubble. Initial memory data loads with varied RAM consumption levels. Memory amounts display below the application names inside each bubble. Each bubble sizes proportionally to its memory usage with larger bubbles for higher RAM consumption. Bubbles consuming above 1 GB display in red color while bubbles consuming below 1 GB display in green color. When users click any bubble, that bubble calculates and displays its exact memory percentage of total 8 GB RAM next to it.
