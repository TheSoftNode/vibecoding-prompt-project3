Category: Web Application

Prompt style: Feature List

Title: Product Feedback Form

Prompt: Build a product feedback form. Users should provide their name, email, and feedback text. Add a rating dropdown with options 1 to 5 stars. Include a submit button that displays all submitted feedback entries below the form. The form fields should automatically clear after each successful submission to prepare for the next entry. Each entry should show name, rating, and feedback text.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                  | Weight | Rationale                                                                                                                        | Dependent On |
| --- | ----------- | ---------------------------------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Render input fields for name and email                                      | major  | These input fields are essential form elements that allow users to provide their identifying information.                        | None         |
| 2   | visual      | Render a text area for feedback text                                         | major  | A text area provides the multi-line input capability needed for longer feedback messages.                                        | None         |
| 3   | content     | Label the rating dropdown with five options: 1, 2, 3, 4, and 5              | major  | These five numbered options provide the specific rating scale that users can select from to rate the product.                    | None         |
| 4   | visual      | Render a submit button                                                       | major  | The submit button serves as the trigger point for users to submit their completed feedback.                                      | None         |
| 5   | interaction | Add a new feedback entry to the list when the submit button is clicked       | major  | Clicking submit creates a new entry in the feedback list, which is the primary user action for recording feedback.               | C4           |
| 6   | state       | Reset all form input fields to empty after submission                        | minor  | Automatically resetting inputs after submission returns the form to its initial state, enabling users to easily add more feedback without manual clearing. | C5           |
| 7   | content     | Label submitted feedback entries with name                                   | major  | The name field identifies who submitted each piece of feedback, providing attribution and context.                               | C5           |
| 8   | content     | Label submitted feedback entries with rating                                 | major  | The rating value shows the satisfaction score for each feedback, which is essential for evaluating product performance.          | C5           |
| 9   | content     | Label submitted feedback entries with feedback text                          | major  | The feedback text contains the detailed user comments and is the most important information in each submission.                  | C5           |
| 10  | layout      | Position feedback entries below the form                                     | minor  | Placing entries below the form creates a logical flow where users input above and see results below.                             | C5           |
