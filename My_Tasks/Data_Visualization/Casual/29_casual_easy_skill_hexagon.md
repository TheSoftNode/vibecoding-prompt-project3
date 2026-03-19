Category: Data_Visualization

Prompt style: Casual

Title: Skill Progress Hexagons

Prompt: Need a skill tracker showing 4 hexagon shapes arranged in a 2x2 grid. Show JavaScript at 85% progress, Python at 60% progress, React at 75% progress, and SQL at 40% progress. Each hexagon displays the skill name inside and fills with green color from bottom to top to match its progress percentage. When I click any hexagon, that hexagon border becomes thicker.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display 4 hexagon shapes                             | major  | The hexagons provide the visual structure for skill progress display.          | None         |
| 2   | layout      | Arrange hexagons in 2x2 grid                         | minor  | Grid arrangement creates an organized layout for the four skills.              | C1           |
| 3   | content     | Display skill names: JavaScript, Python, React, SQL  | major  | Skill names identify what each hexagon represents.                             | None         |
| 4   | layout      | Position skill names inside hexagons                 | minor  | Inside positioning keeps names associated with their progress shapes.          | C3           |
| 5   | state       | Fill hexagon from bottom to top based on percentage  | major  | Fill level visually represents the progress amount.                            | None         |
| 6   | visual      | Fill hexagons with green color                       | minor  | Green color makes the filled portion visible against the hexagon background.   | None         |
| 7   | interaction | Make hexagon border thicker when clicked             | major  | Thicker border provides visual feedback when users click a hexagon.            | None         |

## Justification

The skill progress hexagons work exactly as expected for visualizing skill levels with hexagonal gauges. Four hexagon shapes display arranged in a 2x2 grid. Skill names "JavaScript", "Python", "React", and "SQL" display inside each hexagon. Each hexagon fills from bottom to top with green color to match its progress percentage. When users click any hexagon, that hexagon's border becomes thicker.
