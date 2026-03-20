Category: Data_Visualization

Prompt style: Feature_List

Title: Memory Usage Bubbles

Prompt: Build a memory usage bubble chart that visualizes application RAM consumption. Display 5 circular bubbles arranged horizontally representing Chrome, Slack, VSCode, Spotify, and Docker applications with their current memory usage. Load initial memory data with varied RAM consumption levels. Display the application name and memory amount centered inside each bubble with the name above the amount. When users click any bubble, that bubble calculates and displays its memory percentage of total 8 GB RAM as a label next to it.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                    | Weight | Rationale                                                                                 | Dependent On |
| --- | ----------- | -------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 5 circular bubbles                                     | major  | Bubbles provide the visual containers for displaying each application's memory usage.     | None         |
| 2   | layout      | Arrange bubbles horizontally                                   | minor  | Horizontal arrangement helps users compare memory usage across applications side by side. | C1           |
| 3   | content     | Display app names: Chrome, Slack, VSCode, Spotify, Docker      | major  | App names help users identify which application each bubble represents.                   | None         |
| 4   | state       | Load initial memory data with varied RAM consumption levels    | major  | Loading memory data initializes the bubble values for visualization.                      | None         |
| 5   | content     | Display memory amounts inside bubbles                          | major  | Memory amounts tell users the exact RAM consumption for each application.                 | C4           |
| 6   | layout      | Center app name inside bubble                                  | minor  | Centered positioning keeps the app name visible in the middle of the bubble.              | C3           |
| 7   | layout      | Center memory amount inside bubble                             | minor  | Centered positioning keeps the memory value visible in the middle of the bubble.          | C5           |
| 8   | layout      | Position name above amount inside bubble                       | minor  | Stacking name above amount helps users see the app identity before the memory value.      | C6, C7       |
| 9   | state       | Calculate memory percentage from total 8 GB RAM                | major  | Calculating percentage converts the memory usage into proportion of total system RAM.     | C4           |
| 10  | interaction | Display memory percentage as label next to bubble when clicked | major  | Percentage label shows users what portion of total RAM the application is using.          | C9           |

## Justification

The memory usage bubbles achieved 90% pass rate with one failure. Five circular bubbles display arranged horizontally with application names represented inside each bubble. Initial memory data loads with varied RAM consumption levels. Memory amounts display centered inside each bubble with the name positioned above the amount. When users click any bubble, that bubble calculates its memory percentage of total 8 GB RAM. However, when clicked, the percentage label displays over the bubble instead of next to it as required.
