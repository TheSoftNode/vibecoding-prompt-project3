Category: Web Application

Prompt style: Terse

Title: Contact Form Submission

Prompt: Build a contact form with three input fields: name, email, and message. Display Submit and Clear buttons below the fields. When the Submit button is clicked, show "Message sent successfully!" in green text below the form. When the Clear button is clicked, reset all three fields to empty.

Required libraries: react, tailwindcss

## Rubric

| ID            | Description                                               | Weight | Rationale                                                                      | Dependent On |
| ------------- | --------------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| visual-1      | Render three input fields for name, email, and message    | major  | These fields constitute the core data collection elements of a contact form.   | None         |
| visual-2      | Display a submit button                                   | major  | The submit button triggers form submission, which is the primary user action.  | None         |
| visual-3      | Display a clear button                                    | major  | The clear button enables users to reset form inputs without page refresh.      | None         |
| content-1     | Label the first field as "name" or "Name"                 | major  | Field labels provide essential context for user input expectations.            | visual-1     |
| content-2     | Label the second field as "email" or "Email"              | major  | Email field identification ensures users enter the correct data type.          | visual-1     |
| content-3     | Label the third field as "message" or "Message"           | major  | Message field label clarifies the purpose of the text area input.              | visual-1     |
| interaction-1 | Display a success message below the form when submit is clicked | major  | Success feedback confirms the form submission action to the user.              | visual-2     |
| interaction-2 | Clear all three input fields when the clear button is clicked | major  | Field reset functionality is explicitly required for user convenience.         | visual-3     |
| state-1       | Initialize all input fields as empty on page load         | minor  | Empty initial state provides a clean starting point for user input.            | None         |
