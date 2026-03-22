Category: Data_Visualization

Prompt style: Casual

Title: Trend Arrow Indicator

Prompt: Display five metric cards in a row. Each card shows a number and an arrow. Arrow points up if value increased, down if decreased. Click card to see percentage change below the arrow.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                       | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display five metric cards                                 | major  | Five cards provide multiple data points for trend comparison.                   | None         |
| 2   | layout      | Display cards arranged in a row                           | major  | Row arrangement creates horizontal metric display.                              | C1           |
| 3   | content     | Display number value on each card                         | major  | Number value shows the metric amount.                                           | C1           |
| 4   | visual      | Display arrow on each card                                | major  | Arrow provides visual trend direction indicator.                                | C1           |
| 5   | state       | Point arrow up if value increased                         | major  | Upward arrow indicates positive trend direction.                                | C4           |
| 6   | state       | Point arrow down if value decreased                       | major  | Downward arrow indicates negative trend direction.                              | C4           |
| 7   | interaction | Detect card click                                         | major  | Click detection triggers percentage change display.                             | None         |
| 8   | content     | Calculate percentage change for clicked card              | major  | Percentage calculation provides trend magnitude information.                    | C7           |
| 9   | content     | Display percentage change for clicked card                | major  | Showing percentage tells users the degree of change.                            | C8           |
| 10  | layout      | Position percentage change below arrow                    | major  | Below positioning places percentage near the arrow without blocking the number. | C9           |

## Justification

The trend arrow indicator works as expected for metric trend visualization. Five metric cards display arranged in a row. Each card shows a number value and an arrow. The arrow points up if the value increased and points down if the value decreased. When users click a card, the system calculates the percentage change for that metric and displays it positioned below the arrow showing the degree of trend change.
