Category: Management System

Prompt style: Casual

Title: Smart Shopping List

Prompt: Shopping list app. Add items with name, price, and category (Produce, Dairy, Meat). Display items with category colors: Produce in green, Dairy in blue, Meat in red. Show total cost below the list as the sum of all prices.

Required libraries: react, tailwindcss

## Rubric

| #   | ID          | Description                                                                        | Weight | Rationale                                                                            | Dependent On |
| --- | ----------- | ---------------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Render input fields for item name and price                                        | major  | Name and price inputs capture the two details needed for each shopping item.         | None         |
| 2   | content     | Display category selector with Produce, Dairy, and Meat options                    | major  | The category selector provides the three options for organizing items by type.       | None         |
| 3   | visual      | Display an add button                                                              | major  | The add button triggers adding new items to the list.                                | None         |
| 4   | interaction | Add new item with name, price, and category to the list when add button is clicked | major  | Adding items is the main way users build their shopping list.                        | C3           |
| 5   | content     | Display each item showing name, price, and category                                | major  | Showing all three details lets users see what's on their list.                       | C4           |
| 6   | visual      | Display Produce items in green, Dairy items in blue, and Meat items in red         | major  | Category colors make it faster to scan the list by item type.                        | C5           |
| 7   | layout      | Position the total cost below the list                                             | minor  | Placing the total below separates summary information from the items.                | None         |
| 8   | content     | Display total cost of all items                                                    | major  | The total cost shows the sum of all item prices.                                     | None         |
| 9   | state       | Calculate total cost as the sum of all item prices                                 | major  | The total is computed by summing all item prices in the list.                        | C8           |

## Justification

The shopping list works exactly as expected with input fields for item name and price, and a category selector showing Produce, Dairy, and Meat options. When the add button is clicked, the item appears in the list with the correct category color: Produce items in green, Dairy items in blue, and Meat items in red. Below the list, the total cost displays and updates automatically as items are added, calculated as the sum of all item prices.
