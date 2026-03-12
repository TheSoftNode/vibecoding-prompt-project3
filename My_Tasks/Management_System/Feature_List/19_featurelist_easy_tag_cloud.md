Category: Management_System

Prompt style: Feature_List

Title: Tag Cloud Organizer

Prompt: Build a tag cloud organizer. Display an input field where users can type and add keywords by pressing Enter. Show added tags in a cloud layout with font sizes based on usage count (1x for first occurrence, 1.5x for second, 2x for third and beyond). When clicking any tag, filter the display to show only that tag highlighted in blue while others appear grayed out. Display a counter showing total unique tags and total tag instances.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display input field for typing keywords                   | major  | The input is where users type the tags they want to add to the cloud.                                           | None         |
| 2   | interaction | Add tag when Enter key is pressed                         | major  | Pressing Enter creates a new tag, giving users a quick keyboard-based way to add.                               | None         |
| 3   | visual      | Display added tags in cloud layout                        | major  | The cloud layout shows all tags scattered across the screen.                                                     | None         |
| 4   | state       | Track usage count for each tag                            | major  | Counting how many times a tag appears determines its font size.                                                  | None         |
| 5   | content     | Display tags at 1x font size for first occurrence         | minor  | First-time tags appear in normal size since they're new.                                                         | C4           |
| 6   | content     | Display tags at 1.5x font size for second occurrence      | minor  | Tags used twice get slightly bigger to show they're more common.                                                 | C4           |
| 7   | content     | Display tags at 2x font size for third occurrence and beyond | minor | Frequently used tags appear largest to emphasize their importance.                                             | C4           |
| 8   | interaction | Filter to show only clicked tag                           | major  | Clicking a tag filters the view so users can focus on one keyword.                                               | None         |
| 9   | visual      | Highlight clicked tag in blue                             | minor  | Blue highlighting shows users which tag they selected.                                                           | C8           |
| 10  | visual      | Gray out non-selected tags when filtering                 | minor  | Graying out other tags keeps them visible but de-emphasized during filtering.                                    | C8           |
| 11  | state       | Calculate total unique tags                               | minor  | Counting unique tags tells users how many different keywords exist.                                              | None         |
| 12  | state       | Calculate total tag instances                             | minor  | Counting all instances shows the total number of tags added including duplicates.                                | None         |
| 13  | content     | Display counter showing unique tags and total instances   | minor  | The counter gives users statistics about their tag collection.                                                   | C11, C12     |

## Justification

The tag cloud organizer works exactly as expected with dynamic sizing and click filtering. An input field displays at the top where users can type keywords. When users press Enter, the keyword appears in a cloud layout below the input. Tags display with font sizes based on usage count: 1x for the first occurrence, 1.5x for the second occurrence, and 2x for the third occurrence and beyond. When users click any tag, it highlights in blue while all other tags appear grayed out, creating a filtered view. A counter displays showing the total number of unique tags and total tag instances, updating as users add more keywords.
