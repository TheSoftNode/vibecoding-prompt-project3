Category: Data_Visualization

Prompt style: Terse

Title: Crypto Portfolio Pie Chart

Prompt: Portfolio pie chart showing wallet holdings. Three slices: ETH 50% (blue), BTC 30% (orange), USDT 20% (green). Display percentage inside each slice. Show legend below with token names and their percentages. Total portfolio value "$10,000" displays at center of pie.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display pie chart                                    | major  | The pie chart visualizes portfolio distribution across tokens.                               | None         |
| 2   | visual      | Display ETH slice at 50%                             | major  | The ETH slice shows the largest portion of the portfolio.                                    | None         |
| 3   | visual      | Display BTC slice at 30%                             | major  | The BTC slice shows the second largest portion.                                              | None         |
| 4   | visual      | Display USDT slice at 20%                            | major  | The USDT slice shows the smallest portion.                                                   | None         |
| 5   | state       | Size slices proportionally to percentages            | major  | Proportional sizing accurately represents the portfolio distribution.                        | None         |
| 6   | visual      | Color ETH slice blue                                 | minor  | Blue color identifies the ETH portion visually.                                              | None         |
| 7   | visual      | Color BTC slice orange                               | minor  | Orange color identifies the BTC portion visually.                                            | None         |
| 8   | visual      | Color USDT slice green                               | minor  | Green color identifies the USDT portion visually.                                            | None         |
| 9   | content     | Display "50%" inside ETH slice                       | major  | The percentage shows ETH's exact portfolio allocation.                                       | None         |
| 10  | content     | Display "30%" inside BTC slice                       | major  | The percentage shows BTC's exact portfolio allocation.                                       | None         |
| 11  | content     | Display "20%" inside USDT slice                      | major  | The percentage shows USDT's exact portfolio allocation.                                      | None         |
| 12  | visual      | Display legend below pie chart                       | major  | The legend clarifies which color represents which token.                                     | None         |
| 13  | content     | Show "ETH 50%" in legend                             | minor  | The legend entry identifies ETH and its percentage.                                          | None         |
| 14  | content     | Show "BTC 30%" in legend                             | minor  | The legend entry identifies BTC and its percentage.                                          | None         |
| 15  | content     | Show "USDT 20%" in legend                            | minor  | The legend entry identifies USDT and its percentage.                                         | None         |
| 16  | content     | Display "$10,000" at center of pie                   | major  | The total value shows the portfolio's worth in dollars.                                      | None         |
| 17  | layout      | Position total value at center of pie                | minor  | Center positioning makes the total immediately visible.                                      | C16          |

## Justification

The crypto portfolio pie chart works exactly as expected for visualizing wallet holdings. A pie chart displays with three slices sized proportionally: ETH at 50% colored blue, BTC at 30% colored orange, and USDT at 20% colored green. The percentages "50%", "30%", and "20%" display inside their respective slices. At the center of the pie, "$10,000" displays showing the total portfolio value. Below the pie, a legend displays with entries "ETH 50%", "BTC 30%", and "USDT 20%" matching the slice colors.
