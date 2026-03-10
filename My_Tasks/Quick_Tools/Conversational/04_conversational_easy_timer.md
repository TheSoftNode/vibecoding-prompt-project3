Category: Quick Tools

Prompt style: Conversational

Title: Gas Fee Estimator

Prompt: I need a gas fee estimator for Ethereum transactions. Show three gas speed options: Slow (20 Gwei), Standard (30 Gwei), and Fast (50 Gwei) as buttons. When I select a speed, display the selected Gwei price. Below that, show an input field to enter gas units (default 21000). As I type the gas units, automatically calculate and display the total fee in ETH. Also show the equivalent USD cost assuming 1 ETH = $2000.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                                         | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display three gas speed option buttons: Slow, Standard, Fast    | major  | The three buttons give users a quick way to pick their preferred transaction speed.                                               | None         |
| 2   | content     | Label Slow button with "20 Gwei"                                 | minor  | Showing 20 Gwei tells users the exact gas price for slow transactions.                                                           | C1           |
| 3   | content     | Label Standard button with "30 Gwei"                             | minor  | Showing 30 Gwei tells users the exact gas price for standard transactions.                                                       | C1           |
| 4   | content     | Label Fast button with "50 Gwei"                                 | minor  | Showing 50 Gwei tells users the exact gas price for fast transactions.                                                           | C1           |
| 5   | interaction | Display selected Gwei price when speed button is clicked        | major  | Clicking a speed button shows which gas price option the user picked.                                                             | C1           |
| 6   | visual      | Display input field to enter gas units                           | major  | The input field lets users type in how many gas units their transaction needs.                                                    | None         |
| 7   | content     | Set default value of 21000 in gas units input field              | minor  | Starting with 21000 is helpful since that's the standard amount for basic ETH transfers.                                          | C6           |
| 8   | state       | Calculate total fee in ETH from selected Gwei and gas units      | major  | The fee calculation converts Gwei and gas units into the final ETH cost users need to pay.                                        | None         |
| 9   | content     | Display calculated total fee in ETH                              | major  | Showing the ETH amount tells users their transaction cost in the native currency.                                                 | C8           |
| 10  | state       | Calculate equivalent USD cost assuming 1 ETH = $2000            | major  | Converting to USD helps users understand the real-world dollar cost of their transaction.                                         | C8           |
| 11  | content     | Display equivalent USD cost                                      | major  | Showing the dollar amount makes it easier for users to grasp the actual cost.                                                     | C10          |
| 12  | layout      | Position gas units input below speed selection buttons           | minor  | Placing the input below the buttons creates a logical top-to-bottom workflow.                                                     | None         |

## Justification

The gas fee estimator works exactly as expected for calculating Ethereum transaction costs. Three buttons display the gas speed options: Slow (20 Gwei), Standard (30 Gwei), and Fast (50 Gwei). When a speed button is clicked, the selected Gwei price displays on screen. Below the buttons, an input field allows entering gas units with a default value of 21000. As users type the gas units, the tool automatically calculates the total fee in ETH based on the selected Gwei price and gas units. It also calculates and displays the equivalent USD cost assuming 1 ETH = $2000, helping users understand the real-world cost of their transaction.
