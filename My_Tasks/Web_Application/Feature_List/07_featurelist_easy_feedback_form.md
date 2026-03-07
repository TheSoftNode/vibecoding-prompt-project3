Category: Web Application

Prompt style: Feature List

Title: Product Feedback Form

Prompt: Build a product feedback form. Users should provide their name, email, and feedback text. Add a rating dropdown with options 1 to 5 stars. Include a submit button that displays all submitted feedback entries below the form, and the form fields should reset to empty after submission. Each entry should show name, rating, and feedback text.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID            | Description                                                                  | Weight | Rationale                                                                                                                        | Dependent On |
| --- | ------------- | ---------------------------------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual-1      | Render input fields for name and email                                      | major  | These input fields are essential form elements that allow users to provide their identifying information.                        | None         |
| 2   | visual-2      | Render a text area for feedback text                                         | major  | A text area provides the multi-line input capability needed for longer feedback messages.                                        | None         |
| 3   | content-1     | Display a rating dropdown with five options labeled 1, 2, 3, 4, and 5       | major  | These five numbered options provide the specific rating scale that users can select from to rate the product.                    | None         |
| 4   | visual-3      | Display a submit button                                                      | major  | The submit button serves as the trigger point for users to submit their completed feedback.                                      | None         |
| 5   | interaction-1 | Create a feedback entry when the submit button is clicked                    | major  | Submission creates a new entry in the feedback list, which is the primary action users take to record their feedback.            | visual-3     |
| 6   | state-1       | Reset all form input fields to empty after submission                        | minor  | Automatically resetting inputs after submission returns the form to its initial state, enabling users to easily add more feedback without manual clearing. | interaction-1|
| 7   | content-2     | Display submitted feedback entries below the form                            | major  | Showing submitted entries provides confirmation that feedback was recorded and allows users to review all submissions.           | interaction-1|
| 8   | content-3     | Display name for each feedback entry                                         | major  | The name field identifies who submitted each piece of feedback, providing attribution and context.                               | content-2    |
| 9   | content-4     | Display rating for each feedback entry                                       | major  | The rating value shows the satisfaction score for each feedback, which is essential for evaluating product performance.          | content-2    |
| 10  | content-5     | Display feedback text for each feedback entry                                | major  | The feedback text contains the detailed user comments and is the most important information in each submission.                  | content-2    |
| 11  | layout-1      | Position feedback entries below the form                                     | minor  | Placing entries below the form creates a logical flow where users input above and see results below.                             | content-2    |
