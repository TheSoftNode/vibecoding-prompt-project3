Category: Management System

Prompt style: Casual

Title: Smart Shopping List

Prompt: Shopping list app. Add items with quantity and category (Produce, Dairy, Meat). Categories show in different colors: Produce in green, Dairy in blue, Meat in red. Check off items when bought. Calculate and display total item count. Delete button on each item positioned on the right.

Required libraries: react, tailwindcss

## Rubric

| #   | ID          | Description                                                                           | Weight | Rationale                                                                         | Dependent On |
| --- | ----------- | ------------------------------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Render input field for item name                                                      | major  | Entering the item name is how you specify what to buy.                            | None         |
| 2   | visual      | Render input field for quantity                                                       | major  | The quantity field lets you specify how many of each item to get.                 | None         |
| 3   | content     | Display category selector with Produce, Dairy, and Meat options                       | major  | The three category options organize items by type.                                | None         |
| 4   | visual      | Display an add button                                                                 | major  | The add button is how you add items to the list.                                  | None         |
| 5   | interaction | Add new item with name, quantity, and category to the list when add button is clicked | major  | Clicking add creates a new item with all the details filled in.                   | C4           |
| 6   | visual      | Display Produce items in green, Dairy items in blue, and Meat items in red            | major  | Color coding makes it easier to scan the list by category type.                   | C5           |
| 7   | interaction | Check off items by clicking a checkbox when bought                                    | major  | Clicking the checkbox marks items as bought to track shopping progress.           | C5           |
| 8   | state       | Calculate and display total item count                                                | major  | The count updates automatically to show how many items are on the list.           | C5           |
| 9   | visual      | Display delete button for each item                                                   | major  | The delete button lets you remove items you don't need.                           | C5           |
| 10  | interaction | Remove item from list when delete button is clicked                                   | major  | Clicking delete removes that item from the list.                                  | C9           |
| 11  | layout      | Position the delete button on the right side of each item                             | minor  | Putting delete on the right keeps it accessible but out of the way.               | C9           |

## Justification

The shopping list works exactly as expected with input fields for item name and quantity, and a category selector showing Produce, Dairy, and Meat options. When the add button is clicked, the item appears in the list with the correct color. Produce items show in green, Dairy items in blue, and Meat items in red. Each item has a checkbox that marks it as checked when clicked. The total item count displays and updates automatically. A delete button positioned on the right of each item removes the item from the list when clicked.
