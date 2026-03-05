Category: Web Application

Prompt style: Conversational

Title: User Signup Form

Prompt: Need a simple signup form with username, password, and confirm password fields. On Sign Up click, if password is less than 8 characters show an error message in red under the form. If passwords match show 'Account created successfully!' in green under the form and disable the Sign Up button.

Required libraries: react, tailwindcss

## Rubric

| #  | ID            | Description                                                                | Weight | Rationale                                                                                                     | Dependent On  |
| -- | ------------- | -------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------- | ------------- |
| 1  | visual-1      | Render three input fields labeled username, password, and confirm password | major  | Three specific fields (username, password, confirm password) are explicitly required by prompt for validation workflow. | None          |
| 2  | visual-2      | Display a Sign Up button | major  | Sign Up button is implicitly required by prompt "On Sign Up click" to trigger validation checks. | None          |
| 3  | interaction-1 | Check if password length is less than 8 characters when Sign Up is clicked       | major  | Password length check "if password is less than 8 characters" explicitly required by prompt.                       | visual-2      |
| 4  | content-1     | Display an error message when password is less than 8 characters       | major  | Error message display "show an error message" explicitly required by prompt.                 | interaction-1 |
| 5  | state-1     | Apply red color to the password length error message       | minor  | Red color differentiates error state from success feedback for user clarity.                 | content-1 |
| 6  | layout-1      | Position the password length error message below the form                                | minor  | Consistent placement below form creates predictable location for all validation feedback.                  | content-1     |
| 7  | interaction-2 | Compare password and confirm password values when Sign Up is clicked       | major  | Password comparison "if passwords match" explicitly required by prompt.                       | visual-2      |
| 8  | content-2     | Display the exact text "Account created successfully!" when passwords match       | major  | Exact success message text "Account created successfully!" explicitly required by prompt.                 | interaction-2 |
| 9  | state-2     | Apply green color to the success message       | minor  | Green color differentiates success state from error feedback for user clarity.                 | content-2 |
| 10 | layout-2      | Position the success message below the form                                | minor  | Consistent placement below form creates predictable location for all validation feedback.                  | content-2     |
| 11 | state-3       | Disable the Sign Up button when passwords match and account is created                  | major  | Disabling button prevents duplicate submissions after successful account creation.                                   | interaction-2     |
