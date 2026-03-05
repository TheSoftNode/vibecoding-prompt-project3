Category: Web Application

Prompt style: Feature List

Title: Product Feedback Form

Prompt: Build a product feedback form. Users should provide their name, email, and feedback text. Add a rating dropdown with options 1 to 5 stars. Include a submit button that displays all submitted feedback entries below the form. Each entry should show name, rating, and feedback text. Add a character counter below the feedback text area showing remaining characters out of 200 maximum.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| ID            | Description                                                                  | Weight | Rationale                                                                        | Dependent On |
| ------------- | ---------------------------------------------------------------------------- | ------ | -------------------------------------------------------------------------------- | ------------ |
| visual-1      | Render input fields for name and email                                      | major  | Name and email capture user identity for feedback attribution.                   | None         |
| visual-2      | Render a text area for feedback text                                         | major  | Text area enables multi-line feedback input.                                     | None         |
| visual-3      | Display a rating dropdown with five options: 1, 2, 3, 4, and 5               | major  | Star ratings provide quantifiable satisfaction measurement.                      | None         |
| visual-4      | Display a submit button                                                      | major  | Submit button triggers feedback entry creation.                                  | None         |
| interaction-1 | Create a feedback entry when the submit button is clicked                    | major  | Feedback submission is the core user action of the form.                         | visual-4     |
| content-1     | Display submitted feedback entries below the form                            | major  | Feedback display enables users to see their submitted reviews.                   | None         |
| content-2     | Display name, rating, and feedback text for each feedback entry              | major  | These three fields constitute the essential feedback information.                | content-1    |
| layout-1      | Position feedback entries below the form                                     | minor  | Below-form placement follows conventional submission-display patterns.           | content-1    |
| content-3     | Display a character counter below the feedback text area                     | major  | Character counter provides real-time feedback on input length constraints.       | None         |
| state-1       | Update the character counter to show remaining characters out of 200 maximum | major  | Counter must reflect both current input length and the 200-character limit.      | content-3    |
| state-2       | Prevent feedback text from exceeding 200 characters                          | minor  | Character limit enforcement ensures data consistency.                            | visual-2     |
