Category: Web Application

Prompt style: Conversational

Title: User Signup Form

Prompt: Need a signup form with username, password, and confirm password fields. When the user clicks the Sign Up button, if the password is less than 8 characters show 'Password must be at least 8 characters' under the form. If passwords do not match show 'Passwords do not match' under the form. If passwords match, show 'Account created successfully!' in green under the form and then keep the Sign Up button disabled after successful account creation.

Required libraries: react, tailwindcss

## Rubric

| #   | ID          | Description                                                                                             | Weight | Rationale                                                                                                                                                         | Dependent On |
| --- | ----------- | ------------------------------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Render three input fields labeled username, password, and confirm password                              | major  | These three specific fields are the core data collection elements required to support the full signup validation flow described in the prompt.                    | None         |
| 2   | visual      | Display a Sign Up button                                                                                | major  | The button serves as the trigger for all validation logic and state changes defined in the prompt.                                                                | None         |
| 3   | interaction | Check if password length is less than 8 characters when the user clicks on the Sign Up button           | major  | This check implements the first validation rule to prevent weak passwords from being accepted.                                                                    | None         |
| 4   | content     | Label an error message with the exact text "Password must be at least 8 characters" when password is less than 8 characters | major  | Using this exact message ensures users receive consistent, unambiguous guidance directly matching the requirement, helping them understand and correct the issue. | None         |
| 5   | layout      | Position the error messages below the form                                                              | minor  | Placing feedback under the form keeps all validation results in one consistent, visible location for better usability.                                            | C4           |
| 6   | interaction | Check if passwords do not match when the user clicks on the Sign Up button                              | major  | This comparison enforces confirmation accuracy, a standard security practice in account creation.                                                                 | None         |
| 7   | content     | Label an error message with the exact text "Passwords do not match" when passwords do not match         | major  | The precise wording gives users clear direction on the specific mismatch issue without ambiguity.                                                                 | None         |
| 8   | layout      | Position the password mismatch error message below the form                                             | minor  | Consistent positioning under the form unifies all feedback and improves readability.                                                                              | C7           |
| 9   | content     | Label a success message with the exact text "Account created successfully!" when passwords match        | major  | This exact success message provides definitive confirmation that both validations passed and account creation completed.                                          | None         |
| 10  | interaction | Display a success message in green if the passwords are valid when the user clicks on the sign up button| minor  | Green color delivers immediate positive visual feedback that distinguishes success from error states.                                                             | None         |
| 11  | layout      | Position the success message below the form                                                             | minor  | Placing the success message under the form maintains visual consistency with all other feedback messages.                                                         | C9           |
| 12  | state       | Disable the Sign Up button when an account is successfully created                                      | minor  | Disabling the button prevents duplicate submissions and communicates that the action has been successfully completed.                                             | None         |
