Category: Simulation

Prompt style: Feature_List

Title: Echo Decay Visualizer

Prompt: Build an acoustic echo decay simulator with these features: Display a sound source circle labeled "Source" at the left side. Display five echo circles labeled "E1", "E2", "E3", "E4", "E5" spreading horizontally to the right. When users click the "Emit" button, the source pulses once and then each echo lights up in sequence with decreasing brightness, E1 brightest down to E5 dimmest, simulating sound decay over distance. Each echo activates 0.5 seconds after the previous one. After E5 lights up, all echoes fade back to dim. Include a "Clear" button that resets all echoes to dim state.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                | Weight | Rationale                                                                                           | Dependent On |
| --- | ----------- | ---------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display source circle                                      | major  | Showing the source circle establishes the origin point for echo generation.                         | None         |
| 2   | content     | Display label "Source" on source circle                    | major  | Showing the source label identifies the acoustic emission point.                                    | C1           |
| 3   | layout      | Position source circle at left side                        | minor  | Placing source at left creates the starting point for rightward echo spread.                        | C1           |
| 4   | visual      | Display five echo circles                                  | major  | Showing five echo circles gives users the propagating sound reflections.                            | None         |
| 5   | content     | Display labels "E1", "E2", "E3", "E4", "E5" on echoes      | major  | Showing labels identifies each echo in the decay sequence.                                          | C4           |
| 6   | layout      | Spread echo circles horizontally to the right              | minor  | Positioning echoes rightward shows distance progression from source.                                | C4           |
| 7   | visual      | Display Emit button                                        | minor  | Showing the emit button gives users a control to trigger the echo sequence.                         | None         |
| 8   | interaction | Pulse source once when Emit button clicked                 | major  | Clicking emit creates the initial sound burst that generates echoes.                                | C7           |
| 9   | state       | Light up echoes in sequence E1 to E5                       | major  | Activating echoes sequentially simulates sound traveling through space over time.                   | C8           |
| 10  | state       | Decrease brightness from E1 brightest to E5 dimmest        | major  | Reducing brightness across echoes shows acoustic energy decay with distance.                        | C9           |
| 11  | state       | Activate each echo 0.5 seconds after previous              | major  | Timing each echo at 0.5 second intervals controls the propagation speed users observe.              | C9           |
| 12  | state       | Fade all echoes back to dim after E5 lights up             | major  | Returning echoes to dim marks the end of the decay cycle.                                           | C9           |
| 13  | visual      | Display Clear button                                       | minor  | Showing the clear button gives users a control to reset the simulation.                             | None         |
| 14  | interaction | Reset all echoes to dim when Clear clicked                 | major  | Clicking clear returns all echoes to starting state so users can emit again.                        | C13          |

## Justification

The echo decay visualizer works as expected for sequential acoustic energy simulation. A source circle labeled "Source" displays at the left side. Five echo circles labeled "E1", "E2", "E3", "E4", "E5" display spreading horizontally to the right. An emit button displays and when clicked, the source pulses once and then each echo lights up in sequence with decreasing brightness from E1 brightest down to E5 dimmest, simulating sound decay over distance. Each echo activates 0.5 seconds after the previous one. After E5 lights up, all echoes fade back to dim state. A clear button displays and when clicked, resets all echoes to dim state.
