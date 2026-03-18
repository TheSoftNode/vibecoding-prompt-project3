Category: Web_Application

Prompt style: Terse

Title: Multi-Token Balance Tracker

Prompt: Token balance tracker showing three tokens. Display "ETH", "USDT", "USDC" with input boxes next to each. Plus/minus buttons beside inputs adjust values by 1. Bottom shows "Total USD Value" calculating: ETH × 2000 + USDT × 1 + USDC × 1. All tokens start at 0.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display "ETH" token label                            | minor  | The label identifies the Ethereum token.                                                     | None         |
| 2   | visual      | Display input box for ETH                            | major  | The input shows and allows editing of ETH balance.                                           | None         |
| 3   | content     | Display "USDT" token label                           | minor  | The label identifies the Tether token.                                                       | None         |
| 4   | visual      | Display input box for USDT                           | major  | The input shows and allows editing of USDT balance.                                          | None         |
| 5   | content     | Display "USDC" token label                           | minor  | The label identifies the USD Coin token.                                                     | None         |
| 6   | visual      | Display input box for USDC                           | major  | The input shows and allows editing of USDC balance.                                          | None         |
| 7   | visual      | Display plus button beside each input                | major  | Plus buttons provide controls to increase token amounts.                                     | None         |
| 8   | visual      | Display minus button beside each input               | major  | Minus buttons provide controls to decrease token amounts.                                    | None         |
| 9   | state       | Initialize all tokens to 0                           | minor  | Starting at zero gives users a clean slate for tracking balances.                            | None         |
| 10  | interaction | Increase token value by 1 when plus clicked          | major  | Clicking plus increments that token's balance for tracking additions.                        | C7           |
| 11  | interaction | Decrease token value by 1 when minus clicked         | major  | Clicking minus decrements that token's balance for tracking reductions.                      | C8           |
| 12  | content     | Display "Total USD Value" label at bottom            | major  | The label identifies the calculated total value display.                                     | None         |
| 13  | state       | Calculate ETH × 2000 + USDT × 1 + USDC × 1          | major  | The formula converts token amounts to USD value using their rates.                           | None         |
| 14  | content     | Display calculated total USD value                   | major  | Showing the total gives users their portfolio value in dollars.                              | C13          |
| 15  | state       | Update total when any token value changes            | major  | Recalculating keeps the total accurate as balances change.                                   | C10, C11, C13|

## Justification

The multi-token balance tracker works exactly as expected for portfolio value calculation. Three tokens display with labels "ETH", "USDT", and "USDC", each with an input box showing their balance. Plus and minus buttons sit beside each input. When users click plus, the token value increases by 1. When users click minus, the token value decreases by 1. All tokens start at 0. At the bottom, "Total USD Value" displays, calculating the sum of ETH × 2000 + USDT × 1 + USDC × 1. The total updates automatically whenever any token value changes.
