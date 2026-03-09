Category: Quick Tools

Prompt style: Feature List

Title: Crypto Wallet Address Validator

Prompt: Build crypto wallet address validator. Blockchain dropdown at top: Ethereum, Bitcoin, Solana. Input field for wallet address below dropdown. Validate button below input checks if address matches the selected blockchain's format and shows green "Valid" or red "Invalid" result below button.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                      | Weight | Rationale                                                                                                     | Dependent On |
| --- | ----------- | -------------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display blockchain dropdown with Ethereum, Bitcoin, Solana options               | major  | The dropdown provides the three blockchain options that determine which validation rules to apply.            | None         |
| 2   | layout      | Position dropdown at top                                                         | minor  | Top placement establishes the starting point of the validation workflow.                                      | None         |
| 3   | visual      | Display input field for wallet address                                           | major  | The input field allows users to enter the wallet address they want to validate.                               | None         |
| 4   | layout      | Position input field below dropdown                                              | minor  | Placing the input below the dropdown creates a natural top-to-bottom flow from selection to data entry.       | None         |
| 5   | visual      | Display validate button                                                          | major  | The button provides the trigger for initiating the address format check.                                      | None         |
| 6   | interaction | Validate address format when validate button is clicked                          | major  | Clicking the button triggers the validation check that determines if the address is properly formatted.       | None         |
| 7   | state       | Check address format against the selected blockchain's rules                     | major  | Each blockchain has specific address format requirements that must be verified correctly.                     | C6           |
| 8   | content     | Display "Valid" or "Invalid" text based on validation result                     | major  | The result text provides clear feedback about whether the address passed or failed validation.                | C7           |
| 9   | visual      | Display validation result in green for valid or red for invalid                  | major  | Green and red colors provide immediate visual distinction between successful and failed validation.           | C8           |
| 10  | layout      | Position validation result below the validate button                             | minor  | Placing the result below the button shows the outcome in close proximity to the action that triggered it.     | None         |

## Justification

The crypto wallet address validator works exactly as expected. Users select a blockchain from the dropdown (Ethereum, Bitcoin, or Solana), paste or type a wallet address in the input field, and click the validate button. The validator checks if the address matches the selected blockchain's format. Valid addresses show "Valid" in green, invalid addresses show "Invalid" in red below the button.
