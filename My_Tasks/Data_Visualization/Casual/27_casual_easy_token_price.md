Category: Data_Visualization

Prompt style: Casual

Title: Crypto Token Price Sparkline

Prompt: Need a mini price chart for crypto tokens. Show 3 sparklines (tiny line charts) vertically stacked: ETH with prices [2000, 2100, 2050, 2200, 2150], BTC with prices [40000, 41000, 40500, 42000, 41500], SOL with prices [100, 105, 103, 110, 108]. Display token name on the left of each sparkline. Show latest price on the right. Color sparkline green if last price is higher than first price, red if lower.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display "ETH" token label                            | minor  | The label identifies the Ethereum token.                                                     | None         |
| 2   | content     | Display "BTC" token label                            | minor  | The label identifies the Bitcoin token.                                                      | None         |
| 3   | content     | Display "SOL" token label                            | minor  | The label identifies the Solana token.                                                       | None         |
| 4   | visual      | Display sparkline for ETH prices                     | major  | The sparkline visualizes ETH price trend over time.                                          | None         |
| 5   | visual      | Display sparkline for BTC prices                     | major  | The sparkline visualizes BTC price trend over time.                                          | None         |
| 6   | visual      | Display sparkline for SOL prices                     | major  | The sparkline visualizes SOL price trend over time.                                          | None         |
| 7   | state       | Plot ETH sparkline with values [2000, 2100, 2050, 2200, 2150] | major | Plotting specific values shows the actual ETH price movement.                         | None         |
| 8   | state       | Plot BTC sparkline with values [40000, 41000, 40500, 42000, 41500] | major | Plotting specific values shows the actual BTC price movement.                    | None         |
| 9   | state       | Plot SOL sparkline with values [100, 105, 103, 110, 108] | major | Plotting specific values shows the actual SOL price movement.                             | None         |
| 10  | layout      | Position token label left of sparkline               | minor  | Left positioning clearly associates the label with its chart.                                | None         |
| 11  | content     | Display latest price right of each sparkline         | major  | Showing the current price gives users the most recent value.                                 | None         |
| 12  | state       | Compare last price to first price for each token     | major  | Comparing prices determines if the token is gaining or losing value.                         | None         |
| 13  | visual      | Color sparkline green if last price higher than first| major  | Green indicates upward price movement over the period.                                       | C12          |
| 14  | visual      | Color sparkline red if last price lower than first   | major  | Red indicates downward price movement over the period.                                       | C12          |
| 15  | layout      | Stack three sparklines vertically                    | minor  | Vertical stacking organizes tokens in a scannable list.                                      | None         |

## Justification

The crypto token price sparkline works exactly as expected for quick price trend visualization. Three sparklines display stacked vertically. The first shows ETH with its label on the left, a sparkline plotting prices [2000, 2100, 2050, 2200, 2150], and the latest price 2150 on the right colored green since the last price is higher than the first. The second shows BTC with its label on the left, a sparkline plotting prices [40000, 41000, 40500, 42000, 41500], and the latest price 41500 on the right colored green. The third shows SOL with its label on the left, a sparkline plotting prices [100, 105, 103, 110, 108], and the latest price 108 on the right colored green.
