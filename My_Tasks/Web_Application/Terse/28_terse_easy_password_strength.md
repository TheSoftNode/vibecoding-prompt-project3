Category: Web_Application

Prompt style: Terse

Title: Live Password Strength Meter

Prompt: Password strength checker. Input field for password. As user types, show strength bar below: red for weak (under 6 chars), yellow for medium (6-10 chars), green for strong (11+ chars). Display strength label "Weak", "Medium", or "Strong" next to bar. Show requirements checklist: "At least 6 characters", "At least 11 characters" - checking items as met.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display password input field                         | major  | The input lets users type their password for strength evaluation.                            | None         |
| 2   | visual      | Display strength bar below input                     | major  | The bar provides visual feedback on password strength.                                       | None         |
| 3   | interaction | Update strength as user types                        | major  | Real-time updates give immediate feedback while composing passwords.                         | C1           |
| 4   | state       | Count password character length                      | major  | Character count determines which strength level applies.                                     | None         |
| 5   | visual      | Show red bar for weak passwords under 6 chars       | major  | Red warns users their password is too short and insecure.                                    | C4           |
| 6   | visual      | Show yellow bar for medium passwords 6-10 chars     | major  | Yellow indicates acceptable but not optimal password length.                                 | C4           |
| 7   | visual      | Show green bar for strong passwords 11+ chars       | major  | Green confirms the password meets strong security requirements.                              | C4           |
| 8   | content     | Display "Weak" label for under 6 chars              | major  | The weak label explicitly states the security level.                                         | C5           |
| 9   | content     | Display "Medium" label for 6-10 chars               | major  | The medium label explicitly states the security level.                                       | C6           |
| 10  | content     | Display "Strong" label for 11+ chars                | major  | The strong label explicitly states the security level.                                       | C7           |
| 11  | visual      | Display requirements checklist                       | major  | The checklist shows users specific criteria to meet.                                         | None         |
| 12  | content     | Show "At least 6 characters" requirement             | minor  | This requirement marks the minimum acceptable password length.                               | None         |
| 13  | content     | Show "At least 11 characters" requirement            | minor  | This requirement marks the strong password length threshold.                                 | None         |
| 14  | state       | Check "At least 6 characters" when length ≥ 6        | major  | Checking this item confirms users met the minimum requirement.                               | C4, C12      |
| 15  | state       | Check "At least 11 characters" when length ≥ 11      | major  | Checking this item confirms users met the strong requirement.                                | C4, C13      |

## Justification

The live password strength meter works exactly as expected for password validation. A password input field displays at the top. As users type, a strength bar appears below showing red for weak passwords under 6 characters, yellow for medium passwords between 6-10 characters, and green for strong passwords with 11 or more characters. Next to the bar, a strength label displays "Weak", "Medium", or "Strong" matching the current password length. Below the bar, a requirements checklist shows "At least 6 characters" and "At least 11 characters", checking each requirement as the password length meets or exceeds the threshold.
