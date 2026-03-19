Category: Data_Visualization

Prompt style: Casual

Title: Skill Progress Hexagons

Prompt: Need a skill tracker showing 4 hexagon shapes arranged in a 2x2 grid. Show JavaScript at 85% progress, Python at 60% progress, React at 75% progress, and SQL at 40% progress. Each hexagon displays the skill name inside and fills with green color from bottom to top to match its progress percentage. When I click any hexagon, that hexagon border becomes thicker.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                         | Weight | Rationale                                                                       | Dependent On |
| --- | ----------- | --------------------------------------------------- | ------ | ------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 4 hexagon shapes                            | major  | Users need hexagons as the shape containers for visualizing skill progress.     | None         |
| 2   | layout      | Arrange hexagons in 2x2 grid                        | minor  | Grid arrangement makes it easy to view all four skills at once.                 | C1           |
| 3   | content     | Display skill names: JavaScript, Python, React, SQL | major  | Skill names help users identify which technology each hexagon represents.       | None         |
| 4   | layout      | Position skill names inside hexagons                | minor  | Positioning names inside keeps labels clearly associated with their hexagons.   | C3           |
| 5   | content     | Display progress values: 85%, 60%, 75%, 40%         | major  | Progress values tell users the exact proficiency level for each skill.          | None         |
| 6   | state       | Fill hexagon from bottom to top based on percentage | major  | Bottom-to-top filling creates a visual gauge showing how much progress is made. | C5           |
| 7   | visual      | Fill hexagons with green color                      | minor  | Green color makes the progress fill stand out against the hexagon shape.        | None         |
| 8   | interaction | Make hexagon border thicker when clicked            | major  | Thicker border shows users which hexagon they clicked.                          | None         |

## Justification

The skill progress hexagons achieved 87.5% pass rate with one failure. Four hexagon shapes display arranged in a 2x2 grid. Skill names "JavaScript", "Python", "React", and "SQL" display inside each hexagon with progress values 85%, 60%, 75%, and 40%. Each hexagon fills from bottom to top with green color to match its progress percentage. When users click any hexagon, the border does not become visibly thicker; instead, the green filled area shrinks slightly inward revealing more dark border space around it, but the actual border thickness remains the same, making it unclear that the border has thickened as specified.
