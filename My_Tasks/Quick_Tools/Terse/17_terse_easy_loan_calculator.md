Category: Quick_Tools

Prompt style: Terse

Title: Loan Amortization Calculator

Prompt: Loan calculator. Input loan amount, annual interest rate, loan term in years. Calculate monthly payment. Display amortization table showing month number, payment amount, principal paid, interest paid, remaining balance for first 12 months.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                            | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ------------------------------------------------------ | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display input field for loan amount                    | major  | Users need to enter their loan amount to calculate payments and amortization.                                    | None         |
| 2   | visual      | Display input field for annual interest rate           | major  | Interest rate is essential for calculating how much of each payment goes to interest versus principal.           | None         |
| 3   | visual      | Display input field for loan term in years             | major  | Loan term determines how many monthly payments will be made over the life of the loan.                           | None         |
| 4   | content     | Display label "Loan Amount" for first input            | minor  | Labeling clarifies that this input is for the principal amount borrowed.                                         | None         |
| 5   | content     | Display label "Annual Interest Rate" for second input  | minor  | Labeling ensures users enter the yearly rate, not monthly rate.                                                  | None         |
| 6   | content     | Display label "Loan Term (Years)" for third input      | minor  | Labeling specifies the time unit is years, preventing confusion with months.                                     | None         |
| 7   | state       | Calculate monthly payment from inputs                  | major  | Monthly payment calculation is the primary output users need to budget for loan repayment.                       | None         |
| 8   | content     | Display calculated monthly payment amount              | major  | Showing the monthly payment tells users what they'll owe each month.                                             | None         |
| 9   | visual      | Display amortization table                             | major  | The table provides detailed breakdown of how each payment affects principal and interest over time.              | None         |
| 10  | content     | Display month number column in table                   | minor  | Month numbers let users track which payment period each row represents.                                          | None         |
| 11  | content     | Display payment amount column in table                 | major  | Payment column shows the fixed amount due each month.                                                            | None         |
| 12  | content     | Display principal paid column in table                 | major  | Principal column shows how much of each payment reduces the loan balance.                                        | None         |
| 13  | content     | Display interest paid column in table                  | major  | Interest column shows how much of each payment goes to the lender as interest cost.                              | None         |
| 14  | content     | Display remaining balance column in table              | major  | Balance column shows how much is still owed after each payment.                                                  | None         |
| 15  | state       | Show only first 12 months in amortization table        | minor  | Limiting to 12 months keeps the table concise while showing the first year's breakdown.                          | None         |
| 16  | layout      | Position amortization table below monthly payment      | minor  | Placing the table below the payment amount creates a logical flow from summary to detailed breakdown.            | None         |

## Justification

The application achieved a 93.75% pass rate with one specific failure. Three input fields display labeled "Loan Amount", "Annual Interest Rate", and "Loan Term (Years)" allowing users to enter loan parameters. The tool calculates the monthly payment amount and displays it prominently. Below, an amortization table shows columns for month number, payment amount, principal paid, interest paid, and remaining balance for the first 12 months of the loan. Each row correctly calculates how the payment splits between principal and interest, and shows the declining balance over time. However, the model failed to position the amortization table below the monthly payment. Instead, the table appears to the right side of the payment amount in a two-column layout, not below as required. This positioning issue caused the failure despite all other functionality working correctly.
