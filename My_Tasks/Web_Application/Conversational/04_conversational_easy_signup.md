Category: Web Application

Prompt style: Conversational

Title: User Signup Form

Prompt: Need a simple signup form with username, password, and confirm password fields. On Sign Up click, if password is less than 8 characters show 'Password must be at least 8 characters' in red under the form. If passwords match show 'Account created successfully!' in green under the form and disable the Sign Up button.

Required libraries: react, tailwindcss

## Rubric

| #  | ID            | Description                                                                | Weight | Rationale                                                                                                     | Dependent On  |
| -- | ------------- | -------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------- | ------------- |
| 1  | visual-1      | Render three input fields labeled username, password, and confirm password | major  | Three specific fields (username, password, confirm password) enable user data entry for validation workflow. | None          |
| 2  | visual-2      | Display a Sign Up button | major  | Sign Up button enables user to trigger form submission and validation checks. | None          |
| 3  | interaction-1 | Check if password length is less than 8 characters when Sign Up is clicked       | major  | Password length validation ensures minimum security requirements.                       | visual-2      |
| 4  | content-1     | Display the exact text "Password must be at least 8 characters" when password is less than 8 characters       | major  | Error message communicates specific password length requirement to user.                 | interaction-1 |
| 5  | state-1     | Apply red color to the password length error message       | major  | Red color signals validation error state requiring user attention.                 | content-1 |
| 6  | layout-1      | Position the password length error message below the form                                | major  | Positioning below form associates error message with relevant input context.                  | content-1     |
| 7  | interaction-2 | Compare password and confirm password values when Sign Up is clicked       | major  | Password comparison validates user input consistency.                       | visual-2      |
| 8  | content-2     | Display the exact text "Account created successfully!" when passwords match       | major  | Success message confirms completion of account creation to user.                 | interaction-2 |
| 9  | state-2     | Apply green color to the success message       | major  | Green color signals successful validation state.                 | content-2 |
| 10 | layout-2      | Position the success message below the form                                | major  | Consistent positioning maintains predictable feedback location for user.                  | content-2     |
| 11 | state-3       | Disable the Sign Up button when passwords match and account is created                  | major  | Disabling button prevents duplicate account creation attempts.                                   | content-2     |
