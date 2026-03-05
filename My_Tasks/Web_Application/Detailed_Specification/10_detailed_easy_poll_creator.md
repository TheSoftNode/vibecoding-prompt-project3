Category: Web Application

Prompt style: Detailed Specification

Title: Poll Creator and Voting

Prompt: Create a simple poll application that allows users to create a poll with a question and up to four answer options. The poll creation form should include a text input for the poll question and four text inputs for answer options labeled Option A through Option D. Once created, display the poll question prominently with four clickable buttons showing each answer option. When a user clicks an option, display the vote count for each option as both a number and a horizontal bar visualization where bar width represents the percentage of total votes. The bar with the highest vote count should be highlighted in blue, while others remain gray. Show the total number of votes cast below the results. On initial page load, display the poll creation form.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| ID            | Description                                                                                   | Weight | Rationale                                                                        | Dependent On |
| ------------- | --------------------------------------------------------------------------------------------- | ------ | -------------------------------------------------------------------------------- | ------------ |
| visual-1      | Render a text input for the poll question in the creation form                                | major  | Poll question input captures the central inquiry users will vote on.             | None         |
| content-1     | Display four text inputs labeled Option A, Option B, Option C, and Option D in the form      | major  | Four labeled options provide structured answer choices.                          | None         |
| visual-2      | Display a create button in the poll creation form                                             | major  | Create button triggers poll generation from form inputs.                         | None         |
| interaction-1 | Display the poll view with question and answer buttons when create button is clicked          | major  | Poll display is the primary outcome of the creation interaction.                 | visual-2     |
| content-2     | Display the poll question prominently in the poll view                                        | major  | Question display provides context for the voting options.                        | interaction-1 |
| visual-3      | Display four clickable buttons showing the answer options in the poll view                    | major  | Answer buttons are the interactive elements for casting votes.                   | interaction-1 |
| interaction-2 | Register a vote when an answer button is clicked                                              | major  | Vote registration is the core user interaction of the poll.                      | visual-3     |
| content-3     | Display vote count as a number for each option after voting begins                            | major  | Numeric vote counts provide precise result quantification.                       | interaction-2 |
| visual-4      | Display vote results as horizontal bars where width represents percentage of total votes      | major  | Bar visualization enables at-a-glance comparison of option popularity.           | interaction-2 |
| visual-5      | Highlight the bar with the highest vote count in blue color                                   | major  | Blue highlighting draws attention to the leading option.                         | visual-4     |
| visual-6      | Display bars with lower vote counts in gray color                                             | major  | Gray color visually distinguishes non-leading options from the winner.           | visual-4     |
| content-4     | Display total number of votes cast below the results                                          | major  | Total vote count provides context for interpreting individual option percentages.| None         |
| layout-1      | Display the poll creation form on initial page load                                           | major  | Initial form display establishes the starting state for evaluation.              | None         |
