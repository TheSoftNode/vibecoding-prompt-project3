Category: Simulation

Prompt style: Feature_List

Title: Voltage Cascade Simulator

Prompt: Build a voltage cascade simulator with these features: Display six circular nodes arranged horizontally in a single row. Label the leftmost node "Power" and the remaining five nodes "V1", "V2", "V3", "V4", "V5" from left to right. All nodes start in gray color. Display a "Power On" button below the nodes. When users click the Power On button, nodes turn green one by one from left to right with a visible sequential cascade effect.

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
| 7   | state       | Turn nodes green one by one from left to right             | major  | Sequential activation simulates voltage propagating through the circuit.                            | C6           |
| 8   | state       | Create visible sequential cascade effect                   | major  | Visible cascade shows the progression of voltage through each node.                                 | C7           |

## Justification

The voltage cascade simulator works exactly as expected for sequential circuit voltage visualization. Six circular nodes display arranged horizontally in a single row. The leftmost node displays labeled "Power" and the remaining five nodes display labeled "V1", "V2", "V3", "V4", "V5" from left to right. All nodes display in gray color initially. A power on button displays below the nodes. When users click the Power On button, nodes turn green one by one from left to right with a visible sequential cascade effect.
