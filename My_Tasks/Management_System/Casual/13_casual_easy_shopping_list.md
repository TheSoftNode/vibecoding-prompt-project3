Category: Management System

Prompt style: Casual

Title: Smart Shopping List

Prompt: Shopping list app. Add items with quantity and category (Produce, Dairy, Meat). Categories show in different colors: Produce in green, Dairy in blue, Meat in red. Check off items when bought. Calculate and display total item count. Delete button on each item positioned on the right.

Required libraries: react, tailwindcss

## Rubric

| #   | ID          | Description                                                                           | Weight | Rationale                                                                         | Dependent On |
| --- | ----------- | ------------------------------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Render input field for item name                                                      | major  | The input field is the primary way to specify what items need to be purchased.                                  | None         |
| 2   | visual      | Render input field for quantity                                                       | major  | The quantity field allows tracking how many of each item to buy for accurate shopping planning.                 | None         |
| 3   | content     | Display category selector with Produce, Dairy, and Meat options                       | major  | The category selector provides the three options needed to organize items by type.                              | None         |
| 4   | visual      | Display an add button                                                                 | major  | The add button triggers the action of adding new items to the shopping list.                                    | None         |
| 5   | interaction | Add new item with name, quantity, and category to the list when add button is clicked | major  | Adding items with all details captures the complete shopping information for each entry.                        | C4           |
| 6   | visual      | Display Produce items in green, Dairy items in blue, and Meat items in red            | major  | Color coding by category makes it faster to scan and locate items by type while shopping.                       | C5           |
| 7   | interaction | Check off items by clicking a checkbox when bought                                    | major  | Checking off items tracks what's already been purchased to avoid buying duplicates.                             | C5           |
| 8   | state       | Calculate and display total item count                                                | major  | The count is computed automatically to show how many items are on the list without manual tracking.             | C5           |
| 9   | visual      | Display delete button for each item                                                   | major  | The delete button provides a way to remove items that are no longer needed.                                     | C5           |
| 10  | interaction | Remove item from list when delete button is clicked                                   | major  | Deleting items cleans up the list by removing entries that are no longer relevant.                              | C9           |
| 11  | layout      | Position the delete button on the right side of each item                             | minor  | Placing delete on the right keeps it accessible while preventing accidental clicks during normal list viewing.  | C9           |

## Justification

The shopping list works exactly as expected with input fields for item name and quantity, and a category selector showing Produce, Dairy, and Meat options. When the add button is clicked, the item appears in the list with the correct color. Produce items show in green, Dairy items in blue, and Meat items in red. Each item has a checkbox that marks it as checked when clicked. The total item count displays and updates automatically. A delete button positioned on the right of each item removes the item from the list when clicked.
