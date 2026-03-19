Category: Data_Visualization

Prompt style: Casual

Title: Skill Progress Hexagons

Prompt: Need a skill tracker showing 4 hexagon shapes arranged in a 2x2 grid. Show JavaScript at 85% progress, Python at 60% progress, React at 75% progress, and SQL at 40% progress. Each hexagon displays the skill name inside and fills with green color from bottom to top to match its progress percentage. Display the percentage number centered at the bottom of each hexagon. When I click any hexagon, that hexagon border becomes thicker to show it's selected and stays thick until another hexagon is clicked.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display 4 hexagon shapes                             | major  | The hexagons provide the visual structure for skill progress display.          | None         |
| 2   | layout      | Arrange hexagons in 2x2 grid                         | minor  | Grid arrangement creates an organized layout for the four skills.              | C1           |
| 3   | content     | Display skill names: JavaScript, Python, React, SQL  | major  | Skill names identify what each hexagon represents.                             | None         |
| 4   | layout      | Position skill names inside hexagons                 | minor  | Inside positioning keeps names associated with their progress shapes.          | C3           |
| 5   | content     | Display progress percentages: 85%, 60%, 75%, 40%     | major  | Percentage values show the exact progress for each skill.                      | None         |
| 6   | layout      | Position percentage centered at bottom of hexagon    | minor  | Bottom center positioning shows the numeric value below the visual gauge.      | C5           |
| 7   | state       | Fill hexagon from bottom to top based on percentage  | major  | Fill level visually represents the progress amount.                            | None         |
| 8   | visual      | Fill hexagons with green color                       | minor  | Green color makes the filled portion visible against the hexagon background.   | None         |
| 9   | interaction | Make hexagon border thicker when clicked             | major  | Thicker border shows which hexagon users selected.                             | None         |
| 10  | state       | Keep hexagon border thick until another clicked      | major  | Maintaining thick border shows which hexagon is currently selected.            | C9           |

## Justification

The skill progress hexagons work exactly as expected for visualizing skill levels with hexagonal gauges. Four hexagon shapes display arranged in a 2x2 grid. Skill names "JavaScript", "Python", "React", and "SQL" display inside each hexagon with progress percentages "85%", "60%", "75%", and "40%" centered at the bottom of each hexagon. Each hexagon fills from bottom to top with green color to match its progress percentage. When users click any hexagon, that hexagon's border becomes thicker showing it's selected and stays thick until another hexagon is clicked.
