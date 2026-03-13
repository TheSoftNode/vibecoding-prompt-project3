Category: Quick_Tools

Prompt style: Casual

Title: Restaurant Bill Tip Splitter

Prompt: Need a tip splitter for splitting restaurant bills. Start with a "Bill Amount" box already set to $100. Below it, show three quick tip buttons (15%, 18%, 20%), plus a "Split Between" field set to 2 people. When I hit a tip button, display the tip amount, total bill, and per-person share underneath.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display input field labeled "Bill Amount"             | major  | The label helps users identify where to enter the bill total.                                                    | None         |
| 2   | visual      | Pre-fill "Bill Amount" with $100                      | major  | Pre-filled data lets users immediately test the calculator without typing.                                       | None         |
| 3   | content     | Display "15%" tip button                              | major  | Preset percentages give users quick access to common tipping amounts.                                            | None         |
| 4   | content     | Display "18%" tip button                              | major  | Preset percentages give users quick access to common tipping amounts.                                            | None         |
| 5   | content     | Display "20%" tip button                              | major  | Preset percentages give users quick access to common tipping amounts.                                            | None         |
| 6   | content     | Display input labeled "Split Between"                 | major  | The label clarifies this input controls how many people share the bill.                                          | None         |
| 7   | visual      | Pre-fill "Split Between" with 2                       | major  | Pre-filled data lets users immediately test splitting without typing.                                            | None         |
| 8   | state       | Calculate tip amount when tip button is clicked       | major  | Tip calculation converts the percentage into a dollar amount users need to add.                                  | C3, C4, C5   |
| 9   | state       | Calculate total bill when tip button is clicked       | major  | Total calculation adds tip to original bill to show the final amount owed.                                       | C8           |
| 10  | state       | Calculate per-person share when tip button is clicked | major  | Per-person calculation divides the total by number of people to show individual share.                           | C9           |
| 11  | interaction | Display tip amount when tip button is clicked         | major  | Showing the tip amount helps users see exactly how much extra they're paying.                                    | C8           |
| 12  | interaction | Display total bill when tip button is clicked         | major  | Showing the total confirms the complete amount including tip.                                                    | C9           |
| 13  | interaction | Display per-person share when tip button is clicked   | major  | Showing individual amounts tells each person exactly what they owe.                                              | C10          |
| 14  | layout      | Position tip buttons below "Bill Amount" input        | minor  | Placing buttons after the bill input creates logical top-to-bottom flow.                                         | None         |
| 15  | layout      | Position results underneath buttons and inputs        | minor  | Showing results at the bottom separates calculated outputs from user controls.                                   | None         |

## Justification

The Restaurant Bill Tip Splitter works exactly as expected with instant calculations. A "Bill Amount" box displays pre-filled with $100. Below it, three quick tip buttons appear (15%, 18%, 20%), plus a "Split Between" field pre-filled with 2 people. When users hit a tip button, the calculator displays the tip amount, total bill, and per-person share underneath the inputs.
