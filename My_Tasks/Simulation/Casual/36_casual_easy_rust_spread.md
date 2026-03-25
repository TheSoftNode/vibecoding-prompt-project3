Category: Simulation

Prompt style: Casual

Title: Rust Formation

Prompt: Prompt: Click gray metal surface to start rust at center. Orange-brown corrosion spreads from click point. Show rust percentage counter top-right.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                         | Weight | Rationale                                                                           | Dependent On |
| --- | ----------- | ------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display a gray metal surface                                        | major  | The gray metal surface provides the base material that undergoes oxidation.         | None         |
| 2   | interaction | Start the rust when the gray metal surface is clicked               | major  | Clicking initiates rust formation at the chosen location on the metal surface.      | None         |
| 3   | interaction | Display the rust in orange-brown color                              | major  | Orange-brown color represents a realistic appearance of iron oxide corrosion.       | C2           |
| 4   | layout      | Position rust origin at center of metal surface                     | minor  | Center positioning ensures the rust spreads evenly in all directions from the middle of the surface. | C2           |
| 5   | state       | Spread corrosion outward from the click point                       | major  | Outward spreading simulates how real rust expands across the metal surface.         | C2           |
| 6   | content     | Display the rust percentage counter                                 | major  | The percentage counter shows how much of the metal surface has corroded.            | None         |
| 7   | layout      | Position the rust percentage counter at the top-right of the metal surface | minor  | The positioning keeps the counter visible without obscuring the rust spread.        | C6           |
| 8   | state       | Update the percentage as the rust area increases                    | major  | Counter updates track the progression of oxidation across the surface.              | C6           |

## Justification

The rust formation simulator demonstrates metal oxidation spreading behavior. A gray metal surface displays positioned in the center of the screen. When users click anywhere on the surface, rust begins forming at that click position in orange-brown color. The rust spreads outward from the click point, simulating how real corrosion expands across the metal surface. Below the metal surface, a rust percentage counter displays and updates as the corroded area increases, showing what portion of the metal has oxidized.
