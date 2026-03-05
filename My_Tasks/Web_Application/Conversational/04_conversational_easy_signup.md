Category: Web Application

Prompt style: Conversational

Title: User Signup Form

Prompt: Need a signup form with username, password, and confirm password fields. When the user clicks the Sign Up button, if password is less than 8 characters show 'Password must be at least 8 characters' under the form. If passwords do not match show 'Passwords do not match' under the form. If passwords match show 'Account created successfully!' in green under the form and disable the Sign Up button after successful account creation.

Required libraries: react, tailwindcss

## Rubric

| #  | ID            | Description                                                                | Weight | Rationale                                                                                                     | Dependent On  |
| -- | ------------- | -------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------- | ------------- |
| 1  | visual-1      | Render three input fields labeled username, password, and confirm password | major  | Three specific fields (username, password, confirm password) are explicitly required by prompt for validation workflow. | None          |
| 2  | visual-2      | Display a Sign Up button | major  | Sign Up button is explicitly required by prompt "When the user clicks the Sign Up button" to trigger validation. | None          |
| 3  | interaction-1 | Check if password length is less than 8 characters when Sign Up button is clicked       | major  | Password length validation "if password is less than 8 characters" explicitly required by prompt.                       | visual-2      |
| 4  | content-1     | Display the exact text "Password must be at least 8 characters" when password is less than 8 characters       | major  | Exact error message text "Password must be at least 8 characters" explicitly required by prompt.                 | interaction-1 |
| 5  | layout-1      | Position the password length error message below the form                                | minor  | Consistent placement below form creates predictable location for all validation feedback.                  | content-1     |
| 6  | interaction-2 | Check if passwords do not match when Sign Up button is clicked       | major  | Password mismatch validation "if passwords do not match" explicitly required by prompt.                       | visual-2      |
| 7  | content-2     | Display the exact text "Passwords do not match" when passwords do not match       | major  | Exact error message text "Passwords do not match" explicitly required by prompt.                 | interaction-2 |
| 8  | layout-2      | Position the password mismatch error message below the form                                | minor  | Consistent placement below form creates predictable location for all validation feedback.                  | content-2     |
| 9  | content-3     | Display the exact text "Account created successfully!" when passwords match       | major  | Exact success message text "Account created successfully!" explicitly required by prompt.                 | interaction-2 |
| 10 | state-1     | Apply green color to the success message       | minor  | Green color differentiates success state from error feedback for user clarity.                 | content-3 |
| 11 | layout-3      | Position the success message below the form                                | minor  | Consistent placement below form creates predictable location for all validation feedback.                  | content-3     |
| 12 | state-2       | Disable the Sign Up button when passwords match and account is created                  | major  | Disabling button prevents duplicate submissions after successful account creation.                                   | interaction-2     |
