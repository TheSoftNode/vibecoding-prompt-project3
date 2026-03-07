Category: Web Application

Prompt style: Detailed Specification

Title: Poll Creator and Voting

Prompt: Create a poll application with two views: a creation form and a voting interface. The creation form should have a text input for the poll question, four text inputs labeled Option A through Option D for answer choices, and a Create Poll button. When the button is clicked, transition to the voting view showing the poll question at the top and four clickable answer buttons. After a vote is cast, display each option's vote count as a number next to a horizontal bar, where the bar width represents the vote percentage. Highlight the bar with the most votes in blue. On initial page load, display the creation form.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID            | Description                                                                                   | Weight | Rationale                                                                                                                   | Dependent On  |
| --- | ------------- | --------------------------------------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------------------------- | ------------- |
| 1   | visual-1      | Render a text input for the poll question in the creation form                                | major  | This input captures the central inquiry that users will vote on and is essential for creating a meaningful poll.            | None          |
| 2   | content-1     | Display four text inputs labeled Option A, Option B, Option C, and Option D in the form      | major  | These four specifically labeled inputs provide structured answer choices that users can fill in when creating their poll.   | None          |
| 3   | visual-2      | Display a create button in the poll creation form                                             | major  | This button serves as the trigger to transition from the form state to the active poll state.                               | None          |
| 4   | interaction-1 | Display the poll view with question and answer buttons when create button is clicked          | major  | Transitioning to the poll view represents the core workflow of moving from creation to voting interface.                    | visual-2      |
| 5   | content-2     | Display the poll question at the top of the poll view                                         | major  | Showing the question at the top provides essential context for voters to understand what they are voting on.                | interaction-1 |
| 6   | visual-3      | Display four clickable buttons showing the answer options in the poll view                    | major  | These buttons are the primary interactive elements that enable users to cast their votes.                                   | interaction-1 |
| 7   | interaction-2 | Register a vote and display results when an answer button is clicked                          | major  | Vote registration is the fundamental action that drives the entire poll functionality and triggers results display.         | visual-3      |
| 8   | content-3     | Display vote count as a number next to each option after a vote is cast                       | major  | Numeric counts provide precise quantitative feedback showing how many votes each option has received.                       | interaction-2 |
| 9   | visual-4      | Display vote results as horizontal bars where width represents percentage of total votes      | major  | Horizontal bar visualization enables immediate visual comparison of relative option popularity without reading numbers.     | interaction-2 |
| 10  | state-1       | Apply blue color to the bar with the highest vote count                                       | major  | Blue highlighting visually distinguishes the leading option, making poll results immediately interpretable at a glance.     | visual-4      |
