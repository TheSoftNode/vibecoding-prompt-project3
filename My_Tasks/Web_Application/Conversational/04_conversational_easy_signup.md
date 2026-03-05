Category: Web Application

Prompt style: Conversational

Title: User Signup Form

Prompt: Need a simple signup form with username, password, and confirm password fields. On Sign Up click, if any field is empty show 'All fields are required' in red under the form. If password is less than 8 characters show 'Password must be at least 8 characters' in red under the form. If passwords match show 'Account created successfully!' in green under the form and disable the Sign Up button; otherwise show 'Passwords do not match' in red.

Required libraries: react, tailwindcss

## Rubric

| ID            | Description                                                                | Weight | Rationale                                                                                                     | Dependent On  |
| ------------- | -------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------- | ------------- |
| visual-1      | Render three input fields labeled username, password, and confirm password | major  | Three specific fields (username, password, confirm password) are explicitly required for validation workflow. | None          |
| visual-2      | Display a Sign Up button                                                   | major  | Sign Up button explicitly triggers validation checks as specified in prompt.                                | None          |
| interaction-1 | Check if any field is empty when Sign Up is clicked       | major  | User clicking Sign Up button triggers empty field validation as specified in prompt.                       | visual-2      |
| content-1     | Display the exact text "All fields are required" when any field is empty       | major  | Exact error message wording "All fields are required" is explicitly specified in prompt.                 | interaction-1 |
| state-1     | Apply red color to the empty fields error message       | major  | Red color visually signals empty field validation failure as explicitly specified in prompt.                 | content-1 |
| layout-1      | Position the empty fields error message below the form                                | major  | Prompt explicitly requires message positioned 'under the form' for user feedback visibility.                  | content-1     |
| interaction-2 | Check if password length is less than 8 characters when Sign Up is clicked       | major  | Password length validation explicitly specified in prompt.                       | interaction-1      |
| content-2     | Display the exact text "Password must be at least 8 characters" when password is less than 8 characters       | major  | Exact error message wording "Password must be at least 8 characters" is explicitly specified in prompt.                 | interaction-2 |
| state-2     | Apply red color to the password length error message       | major  | Red color visually signals password length validation failure as explicitly specified in prompt.                 | content-2 |
| layout-2      | Position the password length error message below the form                                | major  | Prompt explicitly requires message positioned 'under the form' for user feedback visibility.                  | content-2     |
| interaction-3 | Compare password and confirm password values when Sign Up is clicked       | major  | Password comparison validation logic explicitly specified in prompt.                       | interaction-1      |
| state-3       | Disable the Sign Up button when passwords match and account is created                  | major  | Button state change (disable) after successful account creation prevents duplicate submissions.                                   | interaction-3     |
