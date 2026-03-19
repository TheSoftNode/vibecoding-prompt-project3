Category: Simulation

Prompt style: Feature_List

Title: Voltage Cascade Simulator

Prompt: Build a voltage cascade simulator with these features: Display six circular nodes arranged horizontally in a single row. Label the leftmost node "Power" and the remaining five nodes "V1", "V2", "V3", "V4", "V5" from left to right. All nodes start in gray color. Display a "Power On" button below the nodes. When users click the Power On button, the Power node turns green and stays green, then V1 turns green and stays green, then V2 turns green and stays green, then V3 turns green and stays green, then V4 turns green and stays green, then V5 turns green and stays green, showing voltage flowing through the circuit from power source to endpoints.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                | Weight | Rationale                                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display six circular nodes                                 | major  | The nodes provide the circuit components users observe during voltage flow.                         | None         |
| 2   | layout      | Arrange nodes horizontally in single row                   | minor  | Horizontal arrangement creates an organized linear circuit layout.                                  | C1           |
| 3   | content     | Display label "Power" on leftmost node                     | minor  | The power label identifies the voltage source in the circuit.                                       | C1           |
| 4   | content     | Display labels "V1", "V2", "V3", "V4", "V5" from left to right | minor  | Voltage labels identify each position in the cascade sequence.                                      | C1           |
| 5   | visual      | Display all nodes in gray color initially                  | minor  | Gray color establishes the unpowered starting state.                                                | C1           |
| 6   | visual      | Display Power On button below nodes                        | minor  | The power button gives users control to trigger the voltage cascade.                                | None         |
| 7   | state       | Turn Power node green and keep green when clicked          | major  | Green on power node shows the voltage source activation.                                            | C6           |
| 8   | state       | Turn V1 green and keep green                               | major  | Green on V1 shows voltage reaching first circuit point.                                             | C7           |
| 9   | state       | Turn V2 green and keep green                               | major  | Green on V2 shows voltage reaching second circuit point.                                            | C8           |
| 10  | state       | Turn V3 green and keep green                               | major  | Green on V3 shows voltage reaching third circuit point.                                             | C9           |
| 11  | state       | Turn V4 green and keep green                               | major  | Green on V4 shows voltage reaching fourth circuit point.                                            | C10          |
| 12  | state       | Turn V5 green and keep green                               | major  | Green on V5 shows voltage reaching final endpoint in the circuit.                                   | C11          |

## Justification

The voltage cascade simulator works exactly as expected for sequential circuit voltage visualization. Six circular nodes display arranged horizontally in a single row. The leftmost node displays labeled "Power" and the remaining five nodes display labeled "V1", "V2", "V3", "V4", "V5" from left to right. All nodes display in gray color initially. A power on button displays below the nodes. When users click the Power On button, the Power node turns green and stays green, then V1 turns green and stays green, then V2 turns green and stays green, then V3 turns green and stays green, then V4 turns green and stays green, then V5 turns green and stays green, showing voltage flowing through the circuit from power source to endpoints.
