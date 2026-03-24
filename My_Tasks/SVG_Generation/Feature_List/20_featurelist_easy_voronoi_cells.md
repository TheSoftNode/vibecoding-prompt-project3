Category: SVG_Generation

Prompt style: Feature_List

Title: Voronoi Cell Generator

Prompt: Build a Voronoi diagram generator that creates organic cell-like patterns. Display an SVG canvas with 6 seed points scattered across it, each represented as a small black circle. Around each seed point, draw a colored polygonal region showing the Voronoi cell, where every point inside the cell is closer to that seed than any other seed. Use different pastel colors for each cell. Below the canvas, include a "Regenerate" button that randomly repositions all seed points and redraws the Voronoi cells.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                                  | Weight | Rationale                                                                                                  | Dependent On |
| --- | ----------- | -------------------------------------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display an SVG canvas                                                                        | major  | The SVG canvas provides the space for rendering Voronoi cells.                                             | None         |
| 2   | visual      | Display 6 seed points on the canvas                                                          | major  | Six seed points create the cell distribution centers.                                                      | None         |
| 3   | visual      | Display seed points as small black circles                                                   | major  | Black circles mark the center of each Voronoi cell.                                                        | C2           |
| 4   | layout      | Scatter seed points across the canvas                                                        | major  | Scattering creates varied cell sizes and shapes.                                                           | C2           |
| 5   | visual      | Draw polygonal regions around each seed point                                                | major  | Polygons define the boundaries of each Voronoi cell.                                                       | C2           |
| 6   | visual      | Color each cell with a different pastel color                                                | major  | Different colors distinguish adjacent Voronoi cells visually.                                              | C5           |
| 7   | visual      | Display a "Regenerate" button                                                                | major  | Regenerate button provides control for creating new patterns.                                              | None         |
| 8   | content     | Display "Regenerate" label on the button                                                     | minor  | Label text clarifies the button's regeneration function.                                                   | C7           |
| 9   | layout      | Position "Regenerate" button below the canvas                                                | minor  | Placing button below separates controls from the visual output.                                            | C7           |
| 10  | interaction | Reposition all seed points randomly when "Regenerate" button is clicked                      | major  | Random repositioning creates new cell distributions.                                                       | C7           |
| 11  | state       | Redraw Voronoi cells after repositioning seed points                                         | major  | Redrawing updates the pattern to match new seed positions.                                                 | C10          |

## Justification

The Voronoi cell generator works as a computational geometry visualizer creating organic patterns. An SVG canvas displays with 6 seed points scattered across it, each shown as a small black circle. Around each seed point, a colored polygonal region appears showing the Voronoi cell. Each cell uses a different pastel color to distinguish it from adjacent cells. Below the canvas, a "Regenerate" button displays positioned below the canvas. When users click the "Regenerate" button, all seed points randomly reposition and the Voronoi cells redraw to match the new distribution.
