Category: Quick_Tools

Prompt style: Feature_List

Title: Reading Time Estimator

Prompt: Build a reading time estimator. Display a textarea labeled "Paste Your Text" where users can enter content. Below the textarea, show three reading speed buttons: "Slow (150 WPM)", "Average (200 WPM)", and "Fast (250 WPM)". When users click any speed button, count the total words in the textarea, calculate the reading time in minutes based on the selected words-per-minute rate, and display the result as "Reading Time: X minutes" below the buttons.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display textarea labeled "Paste Your Text"            | major  | The label tells users where to input the content they want to measure.                                           | None         |
| 2   | content     | Display "Slow (150 WPM)" button                       | major  | Labeled speed options help users choose a reading pace that matches their ability.                               | None         |
| 3   | content     | Display "Average (200 WPM)" button                    | major  | Labeled speed options help users choose a reading pace that matches their ability.                               | None         |
| 4   | content     | Display "Fast (250 WPM)" button                       | major  | Labeled speed options help users choose a reading pace that matches their ability.                               | None         |
| 5   | state       | Count total words in textarea when button is clicked  | major  | Word counting converts the text into a measurable unit for time calculation.                                     | None         |
| 6   | state       | Calculate reading time using 150 WPM when "Slow" is clicked | major  | The calculation divides word count by 150 to estimate minutes needed at slow pace.                               | C5           |
| 7   | state       | Calculate reading time using 200 WPM when "Average" is clicked | major  | The calculation divides word count by 200 to estimate minutes needed at average pace.                            | C5           |
| 8   | state       | Calculate reading time using 250 WPM when "Fast" is clicked | major  | The calculation divides word count by 250 to estimate minutes needed at fast pace.                               | C5           |
| 9   | interaction | Display "Reading Time: X minutes" when "Slow" is clicked | major  | Showing the time estimate helps users plan how long reading will take at slow pace.                              | C6           |
| 10  | interaction | Display "Reading Time: X minutes" when "Average" is clicked | major  | Showing the time estimate helps users plan how long reading will take at average pace.                           | C7           |
| 11  | interaction | Display "Reading Time: X minutes" when "Fast" is clicked | major  | Showing the time estimate helps users plan how long reading will take at fast pace.                              | C8           |
| 12  | layout      | Position speed buttons below textarea                 | minor  | Placing buttons after the text input creates logical top-to-bottom workflow.                                     | None         |
| 13  | layout      | Position result display below speed buttons           | minor  | Showing results at the bottom separates the calculated output from user controls.                                | None         |

## Justification

The Reading Time Estimator works exactly as expected with accurate word-based calculations. A textarea labeled "Paste Your Text" displays where users can enter content. Below the textarea, three reading speed buttons appear: "Slow (150 WPM)", "Average (200 WPM)", and "Fast (250 WPM)". When users click any speed button, the tool counts the total words in the textarea, calculates the reading time in minutes based on the selected words-per-minute rate, and displays the result as "Reading Time: X minutes" below the buttons.
