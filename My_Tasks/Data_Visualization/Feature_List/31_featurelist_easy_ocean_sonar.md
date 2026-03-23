Category: Data_Visualization

Prompt style: Feature_List

Title: Ocean Depth Sonar

Prompt: Build an ocean depth sonar visualization application that visualizes underwater terrain depths across different ocean zones. Display 5 circular sonar rings arranged in a circular pattern on the screen representing North, South, East, West, Center zones, with realistic sample depths measured in meters. Load initial depth readings showing varied ocean floor levels across the different zones. Color rings with depths of 50 meters or shallower in light blue and rings with depths above 50 meters in dark blue. When users click any sonar ring, that specific ring displays the depth measurement value in the center of the circle and shows a wave icon at the bottom edge of the ring.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                        | Weight | Rationale                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 5 circular sonar rings                                                     | major  | Circular rings are essential for representing the sonar zones visually.             | None         |
| 2   | layout      | Arrange sonar rings in a circular pattern                                          | minor  | Circular arrangement mimics real sonar displays effectively.                        | C1           |
| 3   | content     | Display zone labels North, South, East, West, Center                               | major  | Labels tell users which ocean direction each ring tracks.                           | None         |
| 4   | state       | Load initial depth readings with varied ocean floor levels                         | major  | Varied depths show realistic underwater terrain differences.                        | None         |
| 5   | state       | Load data with at least one zone at 50 meters or shallower and at least one above 50 meters | major  | Specific mix ensures both light blue and dark blue rings are visible.              | None         |
| 6   | content     | Display realistic sample depths in meters                                          | major  | Depth numbers give users actual measurement values.                                 | None         |
| 7   | visual      | Color rings with 50 meters or shallower light blue                                 | major  | Light blue instantly shows which zones have shallow water.                          | C1, C5       |
| 8   | visual      | Color rings above 50 meters dark blue                                              | major  | Dark blue signals deeper ocean zones at a glance.                                   | C1, C5       |
| 9   | interaction | Display depth measurement in center of circle when clicked                         | major  | Clicking reveals the exact depth number for that zone.                              | None         |
| 10  | interaction | Display wave icon at bottom edge of ring when clicked                              | major  | Wave icon confirms which ring was just selected.                                    | None         |
| 11  | layout      | Position depth measurement in center of the clicked ring                           | minor  | Center placement keeps the depth value clearly tied to its ring.                    | C9           |
| 12  | layout      | Position wave icon at bottom edge of the clicked ring                              | minor  | Bottom edge puts the icon where it won't block the depth number.                    | C10          |

## Justification

The ocean depth sonar works exactly as expected for visualizing underwater terrain depths. Five circular sonar rings display arranged in a circular pattern representing North, South, East, West, Center zones with realistic sample depths in meters. Initial depth readings load with varied ocean floor levels with at least one zone at 50 meters or shallower and at least one above 50 meters. Rings with 50 meters or shallower display in light blue color while rings above 50 meters display in dark blue color. When users click any sonar ring, that ring displays the depth measurement in the center of the circle and shows a wave icon at the bottom edge of the ring.
