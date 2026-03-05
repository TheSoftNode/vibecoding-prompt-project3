Category: Web Application

Prompt style: Conversational

Title: User Signup Form

Prompt: I need a simple signup form. Just username, password, and confirm password fields. When they click Sign Up, check if the passwords match. If they do, show "Account created successfully!" in green below the form. If they don't match, show "Passwords do not match" in red.

Prompt2: Need a simple signup form with username, password, and confirm password fields. On Sign Up click, if passwords match show 'Account created successfully!' in green under the form; otherwise show 'Passwords do not match' in red.

Required libraries: react, tailwindcss

## Rubric

| ID            | Description                                                                | Weight | Rationale                                                                  | Dependent On  |
| ------------- | -------------------------------------------------------------------------- | ------ | -------------------------------------------------------------------------- | ------------- |
| visual-1      | Render three input fields labeled username, password, and confirm password | major  | Input fields are the presentation elements for data entry.                 | None          |
| visual-2      | Display a Sign Up button                                                   | major  | Button is the visual element that triggers user interaction.               | None          |
| interaction-1 | Compare password and confirm password values when Sign Up is clicked       | major  | User clicking Sign Up button triggers password validation logic.           | visual-2      |
| state-1       | Store result of password comparison (match or no match)                    | major  | Internal validation result determines which message to display.            | interaction-1 |
| content-1     | Display "Account created successfully!" message when passwords match       | major  | Success message shows what data is presented after validation succeeds.    | state-1       |
| visual-3      | Apply green color styling to the success message                           | major  | Green color defines how the success message is visually presented.         | content-1     |
| layout-1      | Position the success message under the form                                | minor  | Message placement defines spatial relationship to form elements.           | content-1     |
| content-2     | Display "Passwords do not match" message when passwords do not match       | major  | Error message shows what data is presented after validation fails.         | state-1       |
| visual-4      | Apply red color styling to the error message                               | major  | Red color defines how the error message is visually presented.             | content-2     |
| layout-2      | Position the error message under the form                                  | minor  | Message placement defines spatial relationship to form elements.           | content-2     |
