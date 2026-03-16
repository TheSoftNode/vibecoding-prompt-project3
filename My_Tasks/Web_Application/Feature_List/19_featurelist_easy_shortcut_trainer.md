Category: Web_Application

Prompt style: Feature_List

Title: Token Allowance Manager

Prompt: Build a token allowance manager for managing ERC20 token spending permissions. At the top, display two tabs labeled "View Allowances" and "Set Allowance" arranged horizontally. Load the app with the View Allowances tab active by default. When a user clicks the "View Allowances" tab, show a table displaying three sample token allowances with columns for token name, spender address, and approved amount. When a user clicks the "Set Allowance" tab, switch the view to show a form with an input field labeled "Amount to Approve" and a "Set Approval" button below it, hiding the table while the form is displayed.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display two tabs                                          | major  | The tabs allow users to switch between viewing and setting allowances.                                           | None         |
| 2   | layout      | Position tabs at top arranged horizontally                | minor  | Positioning tabs at the top in a horizontal row makes navigation easy to find and use.                           | C1           |
| 3   | content     | Label tabs "View Allowances" and "Set Allowance"          | major  | Clear tab labels tell users what functionality each view provides.                                               | None         |
| 4   | state       | Load app with View Allowances tab active by default       | major  | Loading with a default active tab ensures users see content immediately when the app starts.                     | None         |
| 5   | interaction | Show table when user clicks "View Allowances" tab         | major  | Clicking the View tab switches to the allowances display view.                                                   | None         |
| 6   | visual      | Display table with three sample token allowances          | major  | The table shows existing token spending permissions for users to review.                                         | None         |
| 7   | content     | Show token name, spender address, and approved amount columns | major  | The three columns provide complete information about each token allowance.                                    | None         |
| 8   | interaction | Switch view when user clicks "Set Allowance" tab          | major  | Clicking the Set tab changes to the form view for setting new allowances.                                        | None         |
| 9   | visual      | Display form with input field when Set Allowance tab active | major  | The form provides controls for users to set new token allowances.                                              | None         |
| 10  | content     | Label input field "Amount to Approve"                     | minor  | The label tells users what value to enter for the allowance.                                                     | C9           |
| 11  | visual      | Display "Set Approval" button in form                     | major  | The button allows users to submit the new allowance amount.                                                      | None         |
| 12  | layout      | Position button below input field                         | minor  | Placing the button below the input follows standard form layout.                                                 | C9, C11      |
| 13  | state       | Hide table while form is displayed                        | major  | Hiding the table when showing the form prevents confusion by showing only one view at a time.                    | C8           |

## Justification

The token allowance manager works exactly as expected for managing ERC20 token spending permissions. At the top, two tabs labeled "View Allowances" and "Set Allowance" display arranged horizontally. The app loads with the View Allowances tab active by default. When users click the "View Allowances" tab, a table appears displaying three sample token allowances with columns for token name, spender address, and approved amount. When users click the "Set Allowance" tab, the view switches to show a form with an input field labeled "Amount to Approve" and a "Set Approval" button below it, hiding the table while the form is displayed.
