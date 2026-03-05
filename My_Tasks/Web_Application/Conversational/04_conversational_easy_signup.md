Category: Web Application

Prompt style: Conversational

Title: User Signup Form

Prompt: I need a simple signup form. Just username, password, and confirm password fields. When they click Sign Up, check if the passwords match. If they do, show "Account created successfully!" in green below the form. If they don't match, show "Passwords do not match" in red.

Prompt2: Need a simple signup form with username, password, and confirm password fields. On Sign Up click, if passwords match show 'Account created successfully!' in green under the form; otherwise show 'Passwords do not match' in red.

Required libraries: react, tailwindcss

## Rubric

| ID            | Description                                                                                         | Weight | Rationale                                                                                                   | Dependent On  |
| ------------- | --------------------------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------------------- | ------------- |
| visual-1      | Render three input fields labeled username, password, and confirm password                          | major  | Three specific fields (username, password, confirm password) are explicitly required for validation workflow. | None          |
| visual-2      | Display a Sign Up button                                                                            | major  | Sign Up button explicitly triggers password comparison as specified in prompt.                              | None          |
| interaction-1 | Compare password and confirm password values when Sign Up is clicked                                | major  | User clicking Sign Up button triggers password validation logic as specified in prompt.                     | visual-2      |
| content-1     | Display "Account created successfully!" message when passwords match                                | major  | Exact success message text "Account created successfully!" is explicitly specified in prompt.               | interaction-1 |
| state-1       | Apply green color to success message when passwords match                                           | major  | Green styling signals validation success as explicitly specified in prompt.                                 | content-1     |
| layout-1      | Position the success message below the form                                                         | major  | Prompt explicitly requires message positioned 'below the form' for user feedback visibility.                | content-1     |
| content-2     | Display "Passwords do not match" message when passwords do not match                                | major  | Exact error message text "Passwords do not match" is explicitly specified in prompt.                        | interaction-1 |
| state-2       | Apply red color to error message when passwords do not match                                        | major  | Red styling signals validation failure as explicitly specified in prompt.                                   | content-2     |
| layout-2      | Position the error message below the form                                                           | major  | Prompt explicitly requires message positioned 'below the form' for user feedback visibility.                | content-2     |
