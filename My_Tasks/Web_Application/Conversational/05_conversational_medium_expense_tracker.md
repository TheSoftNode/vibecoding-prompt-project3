Category: Web Application

Prompt style: Conversational

Title: Expense Tracker with Budgets

Prompt: I want to track my expenses with budget limits. Let me add an expense with description, amount, and category dropdown (Food, Transport, Entertainment, Other). Show all expenses in a list with delete button for each. At the top, display total spent and category breakdown with progress bars. Set budgets: Food $500, Transport $200, Entertainment $150, Other $100. Progress bars turn yellow at 80% and red when exceeding budget. When I delete an expense, update the total, category amounts, and progress bar colors immediately. On initial load, show 5 sample expenses with totals and progress bars in different colors.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                                                   | Weight | Rationale                                                                              | Dependent On  |
| --- | ----------- | ------------------------------------------------------------------------------------------------------------- | ------ | -------------------------------------------------------------------------------------- | ------------- |
| 1   | visual      | Render input fields for description and amount with category dropdown containing Food, Transport, Entertainment, and Other | major  | These inputs capture the three required attributes for each expense.                   | None          |
| 2   | interaction | Add a new expense to the list when the add button is clicked                                                  | major  | Adding expenses is the primary way users create data in the tracker.                  | C1            |
| 3   | content     | Display each expense showing description, amount, and category with a delete button                            | major  | Users need to see all expense details and have a way to remove them.                   | None          |
| 4   | interaction | Remove the expense from the list when its delete button is clicked                                            | major  | Deletion lets users correct mistakes or remove outdated entries.                       | C3            |
| 5   | layout      | Position the total spent and category breakdown at the top of the page                                        | major  | Top placement makes summary metrics immediately visible without scrolling.             | None          |
| 6   | content     | Display category breakdown showing spent amount for each of the four categories with progress bars             | major  | Category breakdowns reveal spending patterns and progress bars show budget usage.      | None          |
| 7   | state       | Calculate and display progress bar fill as category spent divided by budget (Food $500, Transport $200, Entertainment $150, Other $100) | major  | Progress fill is a computed percentage comparing spending against budget limits.       | C6            |
| 8   | visual      | Display progress bars in yellow when spending reaches 80% of budget                                            | major  | Yellow warns that spending is approaching the budget limit.                            | C7            |
| 9   | visual      | Display progress bars in red when spending exceeds 100% of budget                                              | major  | Red signals budget violation requiring attention.                                      | C7            |
| 10  | state       | Recalculate and update total when an expense is deleted                                                        | major  | The total must decrease when expenses are removed to stay accurate.                    | C4            |
| 11  | state       | Recalculate and update category amounts when an expense is deleted                                             | major  | Category totals must decrease when expenses are removed from their categories.         | C4, C6        |
| 12  | state       | Update progress bar fills when category spending changes from deleting an expense                              | major  | Progress fills must recalculate when category amounts change.                          | C7, C11       |
| 13  | state       | Update progress bar colors when category spending crosses 80% or 100% thresholds after deletion                | major  | Colors must transition when deletions cause spending to cross threshold boundaries.    | C8, C9, C12   |
