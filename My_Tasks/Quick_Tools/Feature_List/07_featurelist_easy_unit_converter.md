Category: Quick Tools

Prompt style: Feature List

Title: Crypto Wallet Address Validator

Prompt: Build crypto wallet address validator. Blockchain dropdown at top: Ethereum, Bitcoin, Solana. Paste input field for wallet address below dropdown. Validate button below input checks format. Result shows green checkmark with "Valid" or red X with "Invalid" below button. Address type label displays below result: "Ethereum (ERC-20)", "Bitcoin (Legacy/SegWit)", "Solana (Base58)".

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                                      | Weight | Rationale                                                                                 | Dependent On |
| --- | ----------- | ------------------------------------------------------------------------------------------------ | ------ | ----------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display blockchain dropdown with options: Ethereum, Bitcoin, Solana                              | major  | The dropdown provides blockchain selection to determine which address format to validate. | None         |
| 2   | layout      | Position blockchain dropdown at top                                                              | minor  | Top placement provides logical flow starting with blockchain selection.                   | None         |
| 3   | visual      | Display input field for wallet address                                                           | major  | The input field allows users to paste or type the wallet address to validate.             | None         |
| 4   | layout      | Position input field below dropdown                                                              | minor  | Below-dropdown placement creates natural top-to-bottom workflow.                          | None         |
| 5   | visual      | Display validate button                                                                          | major  | The validate button triggers the address format checking process.                         | None         |
| 6   | layout      | Position validate button below input                                                             | minor  | Below-input placement follows natural action flow after entering address.                 | None         |
| 7   | interaction | Check wallet address format when validate button is clicked                                      | major  | Clicking validate triggers format verification based on selected blockchain.              | None         |
| 8   | state       | Validate address format based on selected blockchain rules                                       | major  | Validation logic checks if address matches blockchain-specific format requirements.       | C7           |
| 9   | visual      | Display green checkmark with "Valid" below button for valid addresses                            | major  | Green checkmark provides positive visual confirmation of valid address format.            | C8           |
| 10  | visual      | Display red X with "Invalid" below button for invalid addresses                                  | major  | Red X provides clear visual feedback that address format is incorrect.                    | C8           |
| 11  | content     | Display address type label: "Ethereum (ERC-20)", "Bitcoin (Legacy/SegWit)", or "Solana (Base58)" | major  | The label identifies the specific address format type for the selected blockchain.        | None         |
| 12  | layout      | Position address type label below result                                                         | minor  | Below-result placement provides additional context after validation status.               | None         |

## Justification

The crypto wallet address validator works exactly as expected with blockchain selection and format validation. The blockchain dropdown at top displays Ethereum, Bitcoin, and Solana options. Below the dropdown, the input field allows pasting wallet addresses. Below the input, the validate button triggers format checking. When clicked, the validator checks if the address matches the selected blockchain's format rules. For valid addresses, a green checkmark appears with "Valid" below the button. For invalid addresses, a red X appears with "Invalid" below the button. Below the result, the address type label displays the specific format: "Ethereum (ERC-20)" for Ethereum addresses, "Bitcoin (Legacy/SegWit)" for Bitcoin addresses, or "Solana (Base58)" for Solana addresses.
