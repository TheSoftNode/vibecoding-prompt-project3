Category: Web_Application

Prompt style: Conversational

Title: Transaction Gas Fee Estimator

Prompt: I need a gas fee estimator for blockchain transactions. Display three speed options as cards: "Slow (5 min)" at 20 gwei, "Medium (2 min)" at 35 gwei, and "Fast (30 sec)" at 60 gwei. Show a slider below labeled "Transaction complexity" ranging from 1 to 5. When I select a speed or adjust the slider, calculate and display the estimated cost as "Estimated fee: X gwei" where X = speed gwei × complexity value.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display three speed option cards                     | major  | The cards present different transaction speed choices to users.                              | None         |
| 2   | content     | Display "Slow (5 min)" at 20 gwei on first card      | major  | The slow option gives users the cheapest gas fee choice.                                     | None         |
| 3   | content     | Display "Medium (2 min)" at 35 gwei on second card   | major  | The medium option balances cost and speed.                                                   | None         |
| 4   | content     | Display "Fast (30 sec)" at 60 gwei on third card     | major  | The fast option gives users the quickest transaction speed.                                  | None         |
| 5   | visual      | Display slider below speed options                   | major  | The slider lets users indicate their transaction complexity.                                 | None         |
| 6   | content     | Label slider "Transaction complexity"                | minor  | The label explains what the slider controls.                                                 | C5           |
| 7   | state       | Set slider range from 1 to 5                         | major  | The range provides complexity levels for fee calculation.                                    | C5           |
| 8   | interaction | Detect when speed card is selected                   | major  | Selecting a speed triggers fee calculation with that gwei rate.                              | None         |
| 9   | interaction | Detect when slider value changes                     | major  | Adjusting complexity triggers recalculation of the estimated fee.                            | None         |
| 10  | state       | Calculate fee as speed gwei times complexity value   | major  | Multiplying gwei rate by complexity gives the estimated transaction cost.                    | None         |
| 11  | content     | Display "Estimated fee: X gwei" with calculated value| major  | Showing the calculated fee helps users understand their transaction cost.                    | C10          |
| 12  | state       | Update displayed fee when speed or slider changes    | major  | Updating the fee in real-time reflects changes to speed or complexity choices.               | C8, C9, C10  |

## Justification

The gas fee estimator works exactly as expected for calculating transaction costs. Three speed option cards display showing "Slow (5 min)" at 20 gwei, "Medium (2 min)" at 35 gwei, and "Fast (30 sec)" at 60 gwei. Below the cards, a slider displays labeled "Transaction complexity" with a range from 1 to 5. When users select a speed card or adjust the slider, the app calculates the estimated fee by multiplying the speed's gwei value by the complexity value. The result displays as "Estimated fee: X gwei" and updates in real-time whenever the speed selection or slider value changes.
