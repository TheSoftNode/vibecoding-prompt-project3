Category: Web_Application

Prompt style: Feature_List

Title: Star Rating Widget

Prompt: Build a star rating widget with these features:
- Display 5 empty star icons in a row
- When hovering over a star, fill that star and all stars to its left with yellow color; clicking a star sets the rating permanently and displays the numeric value (1-5) below the stars

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                              | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | -------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display 5 star icons                                     | major  | Five stars provide the standard rating scale from 1 to 5.                                                        | None         |
| 2   | layout      | Arrange stars in a horizontal row                        | minor  | Horizontal layout creates the familiar star rating interface.                                                    | None         |
| 3   | visual      | Display stars as empty/outlined by default               | major  | Empty stars show the unrated state before any user interaction.                                                  | None         |
| 4   | interaction | Fill hovered star with yellow color on hover             | major  | Yellow fill on hover provides visual feedback showing which star the user is about to select.                    | C1           |
| 5   | interaction | Fill all stars to the left of hovered star on hover      | major  | Filling left stars on hover shows the full rating value being previewed (e.g., hovering star 4 fills stars 1-4). | C1           |
| 6   | state       | Store selected rating value when star is clicked         | major  | Storing the clicked rating persists the user's choice after the click.                                           | None         |
| 7   | visual      | Fill clicked star and all stars to its left permanently  | major  | Permanent fill shows the committed rating after clicking, distinguishing it from hover previews.                 | None         |
| 8   | content     | Display numeric rating value 1-5                         | major  | Showing the number confirms the exact rating value selected.                                                     | None         |
| 9   | layout      | Position numeric value below the star row                | minor  | Placing the number below keeps the rating display separate from the interactive star controls.                   | None         |
| 10  | state       | Clear previous rating when new star is clicked           | major  | Clearing the old rating when selecting a new star allows users to change their rating.                           | None         |
| 11  | visual      | Remove yellow fill from hover when mouse leaves          | minor  | Removing hover fill when the mouse leaves prevents confusion between hover preview and committed rating.         | None         |

## Justification

The application achieved a 90.91% pass rate with one specific failure. Five empty star icons display in a horizontal row. When hovering over a star, that star fills with yellow along with all stars to its left, providing a preview of the rating. When clicking a star, the rating value is stored and that star plus all stars to its left fill permanently with yellow. The numeric rating value (1-5) corresponding to the clicked star displays on screen. Clicking a different star clears the previous rating and sets the new one. When the mouse leaves, hover fill is removed while the clicked rating remains. However, the model failed to position the numeric value below the star row. Instead, the number appears to the right of the stars in the same row or above them in a header, not below as required. This positioning issue caused the failure despite all other functionality working correctly.
