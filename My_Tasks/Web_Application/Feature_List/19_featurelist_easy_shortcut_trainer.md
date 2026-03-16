Category: Web_Application

Prompt style: Feature_List

Title: Token Allowance Manager

Prompt: Build a token allowance approval form for ERC20 token permissions. Display two tabs labeled "Home" and "Set Allowance" arranged horizontally at the top. Load the app with the Home tab active by default showing a welcome message saying "Select Set Allowance to approve tokens". When a user clicks the Set Allowance tab, hide the welcome message and display a form with an input field labeled "Amount to Approve" and a Submit button below it. When the Submit button is clicked, validate the amount is a positive number and display "Allowance approved" if valid or "Please enter a valid positive number" if invalid.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                                | Weight | Rationale                                                                                       | Dependent On |
| --- | ----------- | ------------------------------------------------------------------------------------------ | ------ | ----------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display two tabs                                                                           | major  | The tabs allow users to navigate between home and form views.                                   | None         |
| 2   | layout      | Position tabs at top arranged horizontally                                                 | minor  | Positioning tabs at the top in a horizontal row makes navigation easy to find and use.          | C1           |
| 3   | content     | Label tabs "Home" and "Set Allowance"                                                      | major  | Clear tab labels tell users what each view provides.                                            | C1           |
| 4   | state       | Load app with Home tab active by default                                                   | major  | Loading with a default active tab ensures users see content immediately when the app starts.    | None         |
| 5   | content     | Show welcome message "Select Set Allowance to approve tokens" on Home tab                  | major  | The welcome message guides users on what to do next.                                            | None         |
| 6   | interaction | Switch view when user clicks "Set Allowance" tab                                           | major  | Clicking the Set tab changes to the form view for approving allowances.                         | None         |
| 7   | interaction | Hide welcome message when Set Allowance tab is clicked                                     | minor  | Hiding the message when showing the form prevents confusion by showing only one view at a time. | C6           |
| 8   | interaction | Display form with input field when Set Allowance tab clicked                               | major  | The form with input field allows users to enter token allowances.                               | C6           |
| 9   | content     | Label input field "Amount to Approve"                                                      | minor  | The label tells users what value to enter for the allowance.                                    | C8           |
| 10  | interaction | Display Submit button when Set Allowance tab clicked                                       | major  | The button allows users to submit the allowance for validation.                                 | C6           |
| 11  | layout      | Position button below input field                                                          | minor  | Placing the button below the input follows standard form layout.                                | C8, C10      |
| 12  | interaction | Validate amount when user clicks Submit button                                             | major  | Clicking Submit triggers validation to check if the entered value is acceptable.                | None         |
| 13  | interaction | Check if entered amount is a positive number                                               | major  | Validation ensures only valid numeric allowance values are accepted.                            | C12          |
| 14  | content     | Display "Allowance approved" if valid or "Please enter a valid positive number" if invalid | major  | Feedback messages tell users whether their input was accepted or what they need to fix.         | C13          |

## Justification

The token allowance approval form works as expected for ERC20 token permissions. Two tabs labeled "Home" and "Set Allowance" display arranged horizontally at the top. The app loads with the Home tab active by default showing a welcome message saying "Select Set Allowance to approve tokens". When users click the Set Allowance tab, the welcome message hides and a form displays with an input field labeled "Amount to Approve" and a Submit button below it. When the Submit button is clicked, the app validates the amount is a positive number and displays "Allowance approved" if valid or "Please enter a valid positive number" if invalid.
