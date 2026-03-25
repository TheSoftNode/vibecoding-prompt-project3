Category: Web Application

Prompt style: Detailed Specification

Title: Poll Creator and Voting

Prompt: Create a poll application with two views: a creation form and a voting interface. The creation form should have a text input for the poll question, four text inputs labeled Option A through Option D for answer choices, and a Create Poll button. When the button is clicked, transition to the voting view showing the poll question at the top and four clickable answer buttons. After a vote is cast, display each option's vote count as a number next to a horizontal bar, where the bar width represents the vote percentage. Highlight the bar with the most votes in blue. On initial page load, display the creation form.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                         | Weight | Rationale                                                                                      | Dependent On |
| --- | ----------- | ------------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display a text input for the poll question                          | major  | The text input captures the central question that users will vote on.                          | None         |
| 2   | visual      | Display four text inputs for the answer options                     | major  | The four inputs provide structured fields for the answer choices.                              | None         |
| 3   | content     | Label answer inputs "Option A", "Option B", "Option C", "Option D"  | minor  | The labels identify each answer input clearly for users filling in the form.                   | C2           |
| 4   | visual      | Display a Create Poll button                                        | major  | The button serves as the trigger to transition from creation to voting interface.              | None         |
| 5   | content     | Label the button "Create Poll"                                      | minor  | The label tells users what action the button performs.                                         | C4           |
| 6   | state       | Display the creation form on initial page load                      | major  | Showing the form initially allows users to create a poll as the starting workflow.             | C1, C2, C4   |
| 7   | interaction | Transition to voting view when the Create Poll button is clicked    | major  | Clicking the button switches from creation mode to voting mode.                                | C4           |
| 8   | content     | Display the poll question at the top of the voting view             | major  | Showing the question provides essential context for what voters are voting on.                 | C7           |
| 9   | layout      | Position the poll question at the top of the voting view            | minor  | Top positioning makes the question the first element voters see.                               | C8           |
| 10  | visual      | Display four clickable answer buttons in the voting view            | major  | The buttons are the interactive elements that enable users to cast votes.                      | C7           |
| 11  | interaction | Register a vote when an answer button is clicked                    | major  | Clicking an answer records the vote for that option.                                           | C10          |
| 12  | content     | Display the vote count as a number next to each option              | major  | The numeric counts show precisely how many votes each option received.                         | C11          |
| 13  | visual      | Display a horizontal bar for each option                            | major  | The horizontal bars provide a visual representation of the vote distribution.                  | C11          |
| 14  | state       | Set the bar width to represent the vote percentage                  | major  | Width proportional to percentage enables visual comparison of option popularity.               | C13          |
| 15  | content     | Highlight the bar with the most votes in blue color                 | major  | Blue highlighting visually distinguishes the leading option for immediate recognition.         | C14          |

## Justification

The poll creator application works as a two-view system for creating and voting on polls. On initial page load, the creation form displays with a text input for the poll question and four text inputs labeled "Option A" through "Option D" for answer choices. A Create Poll button displays that, when clicked, transitions to the voting view. In the voting view, the poll question displays at the top with four clickable answer buttons below showing the options. When an answer button is clicked, a vote is registered and results display showing each option's vote count as a number next to a horizontal bar. The bar width represents the vote percentage of total votes. The bar with the highest vote count highlights in blue color, making the leading option immediately visible.
