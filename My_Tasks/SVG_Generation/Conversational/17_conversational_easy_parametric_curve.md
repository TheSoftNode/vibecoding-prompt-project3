Category: SVG_Generation

Prompt style: Conversational

Title: Parametric Curve Drawer

Prompt: I need a parametric curve generator. Show two input fields labeled "Amplitude" and "Frequency" with default values 50 and 3. When I change either value, redraw a smooth wave curve in the SVG canvas using the formula x = t, y = amplitude × sin(frequency × t) for t from 0 to 2π. Display the curve in red. Below the canvas, show the current equation in the format "y = A × sin(F × t)" with actual values substituted.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                  | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ------------------------------------------------------------ | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display input field for amplitude parameter                  | major  | The amplitude input lets users control the wave height in the parametric equation.                               | None         |
| 2   | visual      | Display input field for frequency parameter                  | major  | The frequency input lets users control how many wave cycles appear in the curve.                                 | None         |
| 3   | content     | Display label "Amplitude" on first input                     | minor  | Labeling clarifies which parameter controls the wave height.                                                     | None         |
| 4   | content     | Display label "Frequency" on second input                    | minor  | Labeling clarifies which parameter controls the number of wave cycles.                                           | None         |
| 5   | state       | Set amplitude default value to 50                            | minor  | Default 50 provides a reasonable starting wave height that's visible without being too extreme.                  | None         |
| 6   | state       | Set frequency default value to 3                             | minor  | Default 3 shows multiple wave cycles without making the curve too compressed.                                    | None         |
| 7   | visual      | Display SVG canvas area                                      | major  | The SVG canvas is where the parametric curve will be drawn.                                                      | None         |
| 8   | visual      | Display smooth wave curve in SVG                             | major  | The curve visualizes the parametric equation as a continuous smooth path.                                        | None         |
| 9   | content     | Display curve in red color                                   | minor  | Red color makes the curve stand out clearly against the background.                                              | None         |
| 10  | state       | Calculate curve using y = amplitude × sin(frequency × t)     | major  | This parametric formula generates the wave shape based on user parameters.                                       | None         |
| 11  | state       | Calculate curve for t from 0 to 2π                           | major  | Using t from 0 to 2π ensures the curve covers a complete cycle range.                                            | None         |
| 12  | interaction | Redraw curve when amplitude value changes                    | major  | Real-time redraw when amplitude changes lets users see how that parameter affects the wave height.               | C1           |
| 13  | interaction | Redraw curve when frequency value changes                    | major  | Real-time redraw when frequency changes lets users see how that parameter affects the wave cycles.               | C2           |
| 14  | content     | Display equation "y = A × sin(F × t)" with substituted values | major | Showing the equation with actual values helps users understand the mathematical relationship they're visualizing. | None         |
| 15  | layout      | Position equation display below the SVG canvas               | minor  | Placing the equation below the canvas creates a clear separation between visualization and formula reference.    | None         |

## Justification

The application achieved a 93.33% pass rate with one specific failure. Two input fields labeled "Amplitude" and "Frequency" display with default values 50 and 3 respectively. An SVG canvas area shows a smooth red wave curve calculated using the parametric equation y = amplitude × sin(frequency × t) for t ranging from 0 to 2π. When users change the amplitude input, the curve redraws immediately to reflect the new wave height. When users change the frequency input, the curve redraws to show more or fewer wave cycles. The current equation displays in the format "y = A × sin(F × t)" with actual amplitude and frequency values substituted. However, the model failed to position the equation display below the SVG canvas. Instead, the equation appears to the right of the canvas in a side panel or above it in a header, not below as required. This positioning issue caused the failure despite all other functionality working correctly.
