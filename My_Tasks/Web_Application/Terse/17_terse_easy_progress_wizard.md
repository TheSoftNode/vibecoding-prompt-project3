Category: Web_Application

Prompt style: Terse

Title: Multi-Step Progress Wizard

Prompt: 3-step wizard. Steps: "Personal Info", "Preferences", "Review". Show all three step labels horizontally. Highlight current step in blue, completed steps in green, future steps in gray. Show "Next" button. Clicking "Next" advances to next step, updates highlighting. On step 3, change button to "Finish".

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display "Personal Info" step label                    | major  | This label identifies the first step in the wizard flow.                                                         | None         |
| 2   | content     | Display "Preferences" step label                      | major  | This label identifies the second step in the wizard flow.                                                        | None         |
| 3   | content     | Display "Review" step label                           | major  | This label identifies the final step in the wizard flow.                                                         | None         |
| 4   | layout      | Position three step labels horizontally               | minor  | Horizontal layout creates a left-to-right progression showing the workflow sequence.                             | None         |
| 5   | visual      | Highlight current step in blue                        | major  | Blue highlighting shows users which step they're currently on in the wizard.                                     | None         |
| 6   | visual      | Highlight completed steps in green                    | major  | Green highlighting shows which steps have already been finished as users progress forward.                       | None         |
| 7   | visual      | Highlight future steps in gray                        | major  | Gray highlighting indicates steps that haven't been reached yet in the workflow.                                 | None         |
| 8   | visual      | Display "Next" button                                 | major  | The Next button is the primary control for advancing through the wizard steps.                                   | None         |
| 9   | state       | Start wizard on step 1 (Personal Info)                | minor  | Starting at step 1 ensures users begin at the beginning of the workflow.                                         | None         |
| 10  | interaction | Advance to next step when "Next" button is clicked    | major  | Clicking Next moves the user forward through the wizard sequence.                                                | C8           |
| 11  | state       | Update step highlighting when advancing to next step  | major  | Updating highlights when advancing shows progress by marking the previous step green and the new step blue.      | None         |
| 12  | visual      | Display "Finish" button on step 3                     | major  | Changing to Finish on the last step signals that the wizard is complete and ready to submit.                     | None         |
| 13  | layout      | Position "Next" or "Finish" button below step labels  | minor  | Placing the button below the labels keeps navigation controls separate from the step indicator.                  | None         |

## Justification

The application achieved a 92.31% pass rate with one specific failure. Three step labels "Personal Info", "Preferences", and "Review" display horizontally across the top. The wizard starts on step 1 with "Personal Info" highlighted in blue, "Preferences" and "Review" in gray. A "Next" button displays on screen. When clicked, the wizard advances to step 2, updating the highlights so "Personal Info" turns green (completed), "Preferences" turns blue (current), and "Review" stays gray (future). Clicking Next again advances to step 3, where "Personal Info" and "Preferences" are green, "Review" is blue, and the button changes to "Finish". However, the model failed to position the "Next" or "Finish" button below the step labels. Instead, the button appears to the right of the labels in the same horizontal row, not below as required. This positioning issue caused the failure despite all other functionality working correctly.
