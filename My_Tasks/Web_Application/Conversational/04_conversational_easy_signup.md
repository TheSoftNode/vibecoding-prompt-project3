Category: Web Application

Prompt style: Conversational

Title: User Signup Form

Prompt: Need a simple signup form with username, password, and confirm password fields. On Sign Up click, if any field is empty show 'All fields are required' in red under the form. If passwords match show 'Account created successfully!' in green under the form and disable the Sign Up button; otherwise show 'Passwords do not match' in red under the form.

Required libraries: react, tailwindcss

## Rubric

| #  | ID            | Description                                                                | Weight | Rationale                                                                                                     | Dependent On  |
| -- | ------------- | -------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------- | ------------- |
| 1  | visual-1      | Render three input fields labeled username, password, and confirm password | major  | Three specific fields (username, password, confirm password) are explicitly required by prompt for validation workflow. | None          |
| 2  | interaction-1 | Check if any field is empty when Sign Up is clicked       | major  | Empty field validation "if any field is empty" explicitly required by prompt.                       | visual-1      |
| 3  | content-1     | Display the exact text "All fields are required" when any field is empty       | major  | Exact error message text "All fields are required" explicitly required by prompt.                 | interaction-1 |
| 4  | state-1     | Apply red color to the empty fields error message       | major  | Red color application for empty fields error message explicitly required by prompt.                 | content-1 |
| 5  | layout-1      | Position the empty fields error message below the form                                | major  | Prompt explicitly requires message positioned "under the form" for user feedback visibility.                  | content-1     |
| 6  | interaction-2 | Compare password and confirm password values when Sign Up is clicked       | major  | Password comparison validation "if passwords match" explicitly required by prompt.                       | visual-1      |
| 7  | content-2     | Display the exact text "Account created successfully!" when passwords match       | major  | Exact success message text "Account created successfully!" explicitly required by prompt.                 | interaction-2 |
| 8  | state-2     | Apply green color to the success message       | major  | Green color application for success message explicitly required by prompt.                 | content-2 |
| 9  | layout-2      | Position the success message below the form                                | major  | Prompt explicitly requires message positioned "under the form" for user feedback visibility.                  | content-2     |
| 10 | state-3       | Disable the Sign Up button when passwords match and account is created                  | major  | Button disable "disable the Sign Up button" explicitly required by prompt.                                   | content-2     |
| 11 | content-3     | Display the exact text "Passwords do not match" when passwords do not match       | major  | Exact error message text "Passwords do not match" explicitly required by prompt.                 | interaction-2 |
| 12 | state-4     | Apply red color to the password mismatch error message and position it below the form       | major  | Red color application and positioning "show 'Passwords do not match' in red under the form" explicitly required by prompt.                 | content-3 |
