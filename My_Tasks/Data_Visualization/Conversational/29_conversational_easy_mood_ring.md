Category: Data_Visualization

Prompt style: Conversational

Title: Mood Ring Calendar

Prompt: I need a mood tracker showing 5 days as circular rings. Display rings for Monday, Tuesday, Wednesday, Thursday, and Friday arranged horizontally. Each ring shows a mood: Monday is "Happy" in yellow, Tuesday is "Stressed" in red, Wednesday is "Calm" in blue, Thursday is "Excited" in orange, and Friday is "Tired" in gray. Display the day name above each ring and the mood name inside the ring. When I click any ring, that ring pulses larger briefly then returns to normal size and displays the mood in bold text at the top of the screen.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | visual      | Display 5 circular rings                             | major  | The rings provide the visual structure for mood display.                       | None         |
| 2   | layout      | Arrange rings horizontally                           | minor  | Horizontal arrangement creates a weekday timeline layout.                      | C1           |
| 3   | content     | Display day names: Monday, Tuesday, Wednesday, Thursday, Friday | major  | Day names identify which day each ring represents.                             | None         |
| 4   | layout      | Position day names above rings                       | minor  | Top positioning associates each day with its mood ring.                        | C3           |
| 5   | content     | Display mood names: Happy, Stressed, Calm, Excited, Tired | major  | Mood names show the emotional state for each day.                              | None         |
| 6   | layout      | Position mood names inside rings                     | minor  | Inside positioning shows the mood within the visual ring.                      | C5           |
| 7   | visual      | Color Monday ring yellow                             | major  | Yellow color represents the Happy mood for Monday.                             | None         |
| 8   | visual      | Color Tuesday ring red                               | major  | Red color represents the Stressed mood for Tuesday.                            | None         |
| 9   | visual      | Color Wednesday ring blue                            | major  | Blue color represents the Calm mood for Wednesday.                             | None         |
| 10  | visual      | Color Thursday ring orange                           | major  | Orange color represents the Excited mood for Thursday.                         | None         |
| 11  | visual      | Color Friday ring gray                               | major  | Gray color represents the Tired mood for Friday.                               | None         |
| 12  | interaction | Pulse ring larger then return to normal when clicked | major  | Pulsing animation provides feedback that users clicked the ring.               | None         |
| 13  | content     | Display mood in bold text at top when clicked        | major  | Bold text at top shows which mood users selected.                              | None         |
| 14  | layout      | Position clicked mood at top of screen               | minor  | Top placement separates the selection feedback from the rings.                 | C13          |

## Justification

The mood ring calendar works exactly as expected for visualizing daily moods with colored rings. Five circular rings display arranged horizontally with day names "Monday", "Tuesday", "Wednesday", "Thursday", and "Friday" positioned above each ring. Mood names "Happy", "Stressed", "Calm", "Excited", and "Tired" display inside each ring. Monday ring displays in yellow color, Tuesday in red, Wednesday in blue, Thursday in orange, and Friday in gray. When users click any ring, that ring pulses larger briefly then returns to normal size and displays the mood in bold text at the top of the screen.
