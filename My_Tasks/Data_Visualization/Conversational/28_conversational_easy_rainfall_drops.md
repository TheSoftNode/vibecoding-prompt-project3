Category: Data_Visualization

Prompt style: Conversational

Title: Rainfall Timeline Drops

Prompt: I want to visualize weekly rainfall as water drops. Display 7 water drop shapes arranged horizontally representing Monday through Saturday with rainfall amounts 2.5 inches, 0.8 inches, 3.2 inches, 1.1 inches, 0.0 inches, 2.9 inches, 1.5 inches. Size each water drop proportionally to its rainfall amount with larger drops for more rain. Display the day name below each drop and the rainfall amount inside the drop. Color drops with rainfall above 2 inches in dark blue and drops below 2 inches in light blue. When I click any drop, highlight it with a yellow border.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                  | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | ------------------------------------------------------------ | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display 7 water drop shapes                                  | major  | The water drops provide the visual structure for rainfall display.             | None         |
| 2   | layout      | Arrange water drops horizontally                             | minor  | Horizontal arrangement creates a timeline layout for the week.                 | C1           |
| 3   | content     | Display day names: Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday | major  | Day names identify which day each water drop represents.                       | None         |
| 4   | layout      | Position day names below water drops                         | minor  | Bottom positioning associates each day with its rainfall drop.                 | C3           |
| 5   | content     | Display rainfall amounts: 2.5, 0.8, 3.2, 1.1, 0.0, 2.9, 1.5  | major  | Rainfall values show the exact precipitation for each day.                     | None         |
| 6   | layout      | Position rainfall amount inside water drop                   | minor  | Inside positioning shows the numeric value within the visual drop.             | C5           |
| 7   | state       | Size water drop proportionally to rainfall amount            | major  | Proportional sizing visually represents the rainfall quantity.                 | None         |
| 8   | visual      | Color drops above 2 inches in dark blue                      | major  | Dark blue indicates heavy rainfall for Monday, Wednesday, and Saturday.        | None         |
| 9   | visual      | Color drops below 2 inches in light blue                     | major  | Light blue indicates lighter rainfall for other days.                          | None         |
| 10  | interaction | Highlight drop with yellow border when clicked               | major  | Yellow border shows which drop users selected.                                 | None         |

## Justification

The rainfall timeline drops work exactly as expected for visualizing weekly precipitation with proportional water drops. Seven water drop shapes display arranged horizontally with day names "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", and "Sunday" positioned below each drop. Rainfall amounts "2.5 inches", "0.8 inches", "3.2 inches", "1.1 inches", "0.0 inches", "2.9 inches", and "1.5 inches" display inside each water drop. Each water drop sizes proportionally to its rainfall amount with larger drops for more rain. Drops with rainfall above 2 inches (Monday, Wednesday, Saturday) display in dark blue color while drops below 2 inches display in light blue color. When users click any drop, it highlights with a yellow border.
