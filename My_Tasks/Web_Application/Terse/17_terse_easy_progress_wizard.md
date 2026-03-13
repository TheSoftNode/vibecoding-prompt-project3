Category: Web_Application

Prompt style: Terse

Title: Multi-Step Progress Wizard

Prompt: 3-step wizard starting at step 1. Steps: "Personal Info", "Preferences", "Review". Show all three step labels horizontally. Highlight current step in blue, completed steps in green, future steps in gray. Below the step labels, show "Next" button. Clicking "Next" advances to next step, updates highlighting. On step 3, change button to "Finish".

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                           | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display "Personal Info" step label                    | major  | Users need to see all three step names to understand the workflow.                                               | None         |
| 2   | content     | Display "Preferences" step label                      | major  | Users need to see all three step names to understand the workflow.                                               | None         |
| 3   | content     | Display "Review" step label                           | major  | Users need to see all three step names to understand the workflow.                                               | None         |
| 4   | layout      | Position three step labels horizontally               | minor  | Horizontal layout creates a left-to-right flow showing workflow progression.                                     | None         |
| 5   | visual      | Highlight current step in blue                        | major  | Blue highlighting shows users which step they're currently on.                                                   | None         |
| 6   | visual      | Highlight completed steps in green                    | major  | Green highlighting shows which steps have already been finished.                                                 | None         |
| 7   | visual      | Highlight future steps in gray                        | major  | Gray highlighting shows which steps haven't been reached yet.                                                    | None         |
| 8   | content     | Display "Next" button                                 | major  | The button text tells users how to move forward through the wizard.                                              | None         |
| 9   | state       | Start wizard on step 1 (Personal Info)                | major  | Starting at step 1 puts users at the beginning of the workflow.                                                  | None         |
| 10  | interaction | Advance to next step when "Next" button is clicked    | major  | Clicking Next moves users forward through the step sequence.                                                     | None         |
| 11  | state       | Update step highlighting when advancing to next step  | major  | Updating colors shows progress as users move forward through steps.                                              | None         |
| 12  | interaction | Change button to "Finish" on step 3                   | major  | Changing to Finish tells users the wizard is ready to complete.                                                  | None         |
| 13  | layout      | Position button below step labels                     | minor  | Putting the button below keeps navigation separate from step indicators.                                         | None         |

## Justification

The application achieved a 92.31% pass rate with one specific failure. Three step labels "Personal Info", "Preferences", and "Review" display horizontally across the top. The wizard starts on step 1 with "Personal Info" highlighted in blue, "Preferences" and "Review" in gray. A "Next" button displays on screen. When clicked, the wizard advances to step 2, updating the highlights so "Personal Info" turns green (completed), "Preferences" turns blue (current), and "Review" stays gray (future). Clicking Next again advances to step 3, where "Personal Info" and "Preferences" are green, "Review" is blue, and the button changes to "Finish". However, the model failed to position the "Next" or "Finish" button below the step labels. Instead, the button appears to the right of the labels in the same horizontal row, not below as required. This positioning issue caused the failure despite all other functionality working correctly.
