Category: SVG_Generation

Prompt style: Feature_List

Title: Voronoi Cell Generator

Prompt: Build a Voronoi diagram generator that creates organic cell-like patterns. Display an SVG canvas with 6 seed points scattered across it, each represented as a small black circle. Around each seed point, draw a colored polygonal region showing the Voronoi cell, where every point inside the cell is closer to that seed than any other seed. Use different pastel colors for each cell. Below the canvas, include a "Regenerate" button that randomly repositions all seed points and redraws the Voronoi cells.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                                  | Weight | Rationale                                                                                                  | Dependent On |
| --- | ----------- | -------------------------------------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display an SVG canvas                                                                        | major  | The SVG canvas provides the space for rendering Voronoi cells.                                             | None         |
| 2   | visual      | Display 6 seed points on the canvas                                                          | major  | Six seed points create the cell distribution centers.                                                      | C1           |
| 3   | visual      | Display seed points as small black circles                                                   | major  | Black circles mark the center of each Voronoi cell.                                                        | C2           |
| 4   | layout      | Scatter seed points across the canvas                                                        | major  | Scattering creates varied cell sizes and shapes.                                                           | C2           |
| 5   | visual      | Draw polygonal regions around each seed point                                                | major  | Polygons define the boundaries of each Voronoi cell.                                                       | C2           |
| 6   | visual      | Color each cell with a different pastel color                                                | major  | Different colors distinguish adjacent Voronoi cells visually.                                              | C5           |
| 7   | state       | Calculate Voronoi cell boundaries based on seed point positions                              | major  | Boundary calculation determines which regions belong to each seed.                                         | C2           |
| 8   | visual      | Display a "Regenerate" button below the canvas                                               | major  | Regenerate button provides control for creating new patterns.                                              | None         |
| 9   | interaction | Randomly reposition all seed points when "Regenerate" button is clicked                      | major  | Random repositioning creates new cell distributions.                                                       | C8           |
| 10  | interaction | Redraw Voronoi cells after repositioning seed points                                         | major  | Redrawing updates the pattern to match new seed positions.                                                 | C9           |
| 11  | layout      | Position "Regenerate" button below the canvas                                                | minor  | Placing button below separates controls from the visual output.                                            | C1, C8       |

## Justification

The Voronoi cell generator works as a computational geometry visualizer creating organic patterns. An SVG canvas displays with 6 seed points scattered across it, each shown as a small black circle. Around each seed point, a colored polygonal region appears showing the Voronoi cell where every point inside the cell is closer to that seed than any other seed. Each cell uses a different pastel color to distinguish it from adjacent cells. The application calculates Voronoi cell boundaries based on seed point positions. Below the canvas, a "Regenerate" button displays. When users click the "Regenerate" button, all seed points randomly reposition and the Voronoi cells redraw to match the new distribution.
