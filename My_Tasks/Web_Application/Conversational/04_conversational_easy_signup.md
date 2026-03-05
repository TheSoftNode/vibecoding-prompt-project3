Category: Web Application

Prompt style: Conversational

Title: User Signup Form

Prompt: Need a simple signup form with username, password, and confirm password fields. On Sign Up click, if any field is empty show 'All fields are required' in red under the form. If password is less than 8 characters show 'Password must be at least 8 characters' in red under the form. If passwords match show 'Account created successfully!' in green under the form and disable the Sign Up button; otherwise show 'Passwords do not match' in red.

Required libraries: react, tailwindcss

## Rubric

| #  | ID            | Description                                                                | Weight | Rationale                                                                                                     | Dependent On  |
| -- | ------------- | -------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------- | ------------- |
| 1  | visual-1      | Render three input fields labeled username, password, and confirm password | major  | Three specific fields (username, password, confirm password) are explicitly required by prompt for validation workflow. | None          |
| 2  | visual-2      | Display a Sign Up button                                                   | major  | Sign Up button explicitly required by prompt to trigger validation checks.                                | None          |
| 3  | interaction-1 | Check if any field is empty when Sign Up is clicked       | major  | Empty field validation "if any field is empty" explicitly required by prompt.                       | visual-2      |
| 4  | content-1     | Display the exact text "All fields are required" when any field is empty       | major  | Exact error message text "All fields are required" explicitly required by prompt.                 | interaction-1 |
| 5  | state-1     | Apply red color to the empty fields error message       | major  | Red color for empty fields error message explicitly required by prompt "show 'All fields are required' in red".                 | content-1 |
| 6  | layout-1      | Position the empty fields error message below the form                                | major  | Prompt explicitly requires message positioned "under the form" for user feedback visibility.                  | content-1     |
| 7  | interaction-2 | Check if password length is less than 8 characters when Sign Up is clicked       | major  | Password length validation "if password is less than 8 characters" explicitly required by prompt.                       | interaction-1      |
| 8  | content-2     | Display the exact text "Password must be at least 8 characters" when password is less than 8 characters       | major  | Exact error message text "Password must be at least 8 characters" explicitly required by prompt.                 | interaction-2 |
| 9  | state-2     | Apply red color to the password length error message       | major  | Red color for password length error message explicitly required by prompt "show 'Password must be at least 8 characters' in red".                 | content-2 |
| 10 | layout-2      | Position the password length error message below the form                                | major  | Prompt explicitly requires message positioned "under the form" for user feedback visibility.                  | content-2     |
| 11 | interaction-3 | Compare password and confirm password values when Sign Up is clicked       | major  | Password comparison validation "if passwords match" explicitly required by prompt.                       | interaction-1      |
| 12 | state-3       | Disable the Sign Up button when passwords match and account is created                  | major  | Button disable "disable the Sign Up button" explicitly required by prompt after successful account creation.                                   | interaction-3     |
