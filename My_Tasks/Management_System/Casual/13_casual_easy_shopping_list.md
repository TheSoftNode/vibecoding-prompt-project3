Category: Management System

Prompt style: Casual

Title: Smart Shopping List

Prompt: Shopping list app. Add items with quantity and category (Produce, Dairy, Meat). Categories show in different colors: Produce in green, Dairy in blue, Meat in red. Check off items when bought. Delete button on each item positioned on the right.

Required libraries: react, tailwindcss

## Rubric

| #   | ID          | Description                                                                           | Weight | Rationale                                                                         | Dependent On |
| --- | ----------- | ------------------------------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Render input field for item name                                                      | major  | The input field provides a place to type what to shop for.                        | None         |
| 2   | visual      | Render input field for quantity                                                       | major  | The quantity field allows specifying how many of each item to buy.                | None         |
| 3   | content     | Display category selector with Produce, Dairy, and Meat options                       | major  | The selector provides the category choices for organizing items.                  | None         |
| 4   | visual      | Display an add button                                                                 | major  | The add button triggers adding items to the list.                                 | None         |
| 5   | interaction | Add new item with name, quantity, and category to the list when add button is clicked | major  | This creates items with all the info needed for the shopping list.                | C4           |
| 6   | content     | Display each item showing name, quantity, and category                                | major  | Displaying all item details shows what's on the list.                             | None         |
| 7   | state       | Display Produce items in green, Dairy items in blue, and Meat items in red            | major  | Different colors for each category make it faster to find items by type.          | C6           |
| 8   | visual      | Display checkbox for each item                                                        | major  | Checkboxes allow marking off items when bought.                                   | C6           |
| 9   | interaction | Toggle item checked status when checkbox is clicked                                   | major  | Checking off items tracks what's already been bought.                             | C8           |
| 10  | visual      | Display delete button for each item                                                   | major  | Delete buttons allow removing items from the list.                                | C6           |
| 11  | interaction | Remove item from list when delete button is clicked                                   | major  | Deletion clears items that aren't needed anymore.                                 | C10          |
| 12  | layout      | Position the delete button on the right side of each item                             | minor  | Putting the delete button on the right keeps it out of the way but easy to click. | C10          |

## Justification

The shopping list works exactly as expected with input fields for item name and quantity, and a category selector showing Produce, Dairy, and Meat options. When the add button is clicked, the item appears in the list displaying its name, quantity, and category with the correct color. Produce items show in green, Dairy items in blue, and Meat items in red. Each item has a checkbox that marks it as checked when clicked, and a delete button positioned on the right that removes the item from the list.
