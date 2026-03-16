Category: Web_Application

Prompt style: Feature_List

Title: Smart Contract Event Logger

Prompt: Build a smart contract event logger for tracking blockchain transaction events. At the top, display a form with an input field labeled "Event Name" where users can type the name of a blockchain event they want to log. Below the input field, show an "Add Event" button. When a user clicks the button, add the entered event name to a list of logged events displayed below the button, showing each event with a timestamp of when it was added. Display all logged events in a vertical list where each event shows the event name followed by the timestamp in parentheses.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display input field                                       | major  | The input field lets users type event names.                                                                     | None         |
| 2   | layout      | Position input field at top                               | minor  | Top positioning makes the form easy to find.                                                                     | C1           |
| 3   | content     | Label input field "Event Name"                            | minor  | The label tells users what to enter.                                                                             | C1           |
| 4   | visual      | Display "Add Event" button                                | major  | The button lets users add events to the log.                                                                     | None         |
| 5   | layout      | Position button below input field                         | minor  | Positioning below creates clear form flow.                                                                       | C1, C4       |
| 6   | interaction | Add event to list when user clicks button                 | major  | Clicking adds the event to the logged events.                                                                    | None         |
| 7   | state       | Generate timestamp when event is added                    | major  | Timestamp records when each event was logged.                                                                    | C6           |
| 8   | visual      | Display logged events in vertical list                    | major  | The list shows all logged events.                                                                                | None         |
| 9   | layout      | Position list below button                                | minor  | Positioning below creates clear vertical flow.                                                                   | C4, C8       |
| 10  | content     | Show event name for each logged event                     | major  | The event name identifies what was logged.                                                                       | None         |
| 11  | content     | Show timestamp in parentheses after event name            | major  | The timestamp shows when the event was added.                                                                    | None         |

## Justification

The smart contract event logger works exactly as expected for tracking blockchain transaction events. At the top, a form displays with an input field labeled "Event Name" where users can type the name of a blockchain event they want to log. Below the input field, an "Add Event" button appears. When users click the button, the entered event name gets added to a list of logged events displayed below the button, with each event showing a timestamp of when it was added. All logged events display in a vertical list where each event shows the event name followed by the timestamp in parentheses.
