Category: Simulation

Prompt style: Casual

Title: Rust Formation

Prompt: Metal oxidation sim. Click gray metal surface to start rust. Orange-brown corrosion spreads from click point. Show rust percentage counter below.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                              | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | -------------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display gray metal surface                               | major  | The gray metal surface provides the base material that undergoes oxidation.    | None         |
| 2   | interaction | Start rust at click position                             | major  | Clicking initiates rust formation at the chosen location on the metal surface. | None         |
| 3   | visual      | Display rust in orange-brown color                       | major  | Orange-brown color represents realistic iron oxide corrosion appearance.       | C2           |
| 4   | state       | Spread corrosion outward from click point                | major  | Outward spreading simulates how real rust expands across the metal surface.    | C2           |
| 5   | content     | Display rust percentage counter                          | major  | The percentage counter shows how much of the metal surface has corroded.       | None         |
| 6   | layout      | Position rust percentage counter below metal surface     | minor  | Below positioning keeps the counter visible without obscuring the rust spread. | C5           |
| 7   | content     | Show percentage value in counter                         | minor  | Displaying the percentage value quantifies the corrosion coverage numerically. | C5           |
| 8   | state       | Update percentage as rust area increases                 | major  | Counter updates track the progression of oxidation across the surface.         | C5           |

## Justification

The rust formation simulator demonstrates metal oxidation spreading behavior. A gray metal surface background displays initially. When users click anywhere on the surface, rust begins forming at that click position in orange-brown color. The rust spreads outward continuously from the origin point, simulating how real corrosion expands across metal. Below the metal surface, a rust percentage counter displays and updates as the corroded area increases, showing what portion of the metal has oxidized.
