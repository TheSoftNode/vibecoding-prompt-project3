Category: Web Application

Prompt style: Conversational

Title: User Signup Form

Prompt: I need a simple signup form. Just username, password, and confirm password fields. When they click Sign Up, check if the passwords match. If they do, show "Account created successfully!" in green below the form. If they don't match, show "Passwords do not match" in red.

Required libraries: react, tailwindcss

## Rubric

| ID            | Description                                                                 | Weight | Rationale                                                                        | Dependent On |
| ------------- | --------------------------------------------------------------------------- | ------ | -------------------------------------------------------------------------------- | ------------ |
| visual-1      | Render three input fields labeled username, password, and confirm password  | major  | The three fields constitute the minimum required inputs for password validation. | None         |
| visual-2      | Display a Sign Up button                                                    | major  | The button triggers the password matching validation logic.                      | None         |
| state-1       | Compare password and confirm password values when Sign Up is clicked        | major  | Password matching is the core validation requirement.                            | visual-2     |
| content-1     | Display "Account created successfully!" when passwords match                | major  | Success message confirms valid input and simulated account creation.             | state-1      |
| visual-3      | Apply green color styling to the success message                            | major  | Green color provides the specified visual feedback for success state.            | content-1    |
| layout-1      | Position the success message below the form                                 | minor  | Message placement below the form follows conventional UI patterns.               | content-1    |
| content-2     | Display "Passwords do not match" when passwords do not match                | major  | Error message identifies the validation failure to the user.                     | state-1      |
| visual-4      | Apply red color styling to the error message                                | major  | Red color provides the specified visual feedback for error state.                | content-2    |
| layout-2      | Position the error message below the form                                   | minor  | Error message placement below the form follows conventional UI patterns.         | content-2    |
