Category: Quick_Tools

Prompt style: Feature_List

Title: Rhyme Finder

Prompt: Build a rhyme finder tool. Display an input field with placeholder text "Enter a word..." where users type a word, with a "Find Rhymes" button next to it. When pressing Enter or clicking the button, search through a predefined list of common words to find words that rhyme with the input, then show up to 5 matching rhymes in a list below the input. If no rhymes are found, display "No rhymes found" in gray text.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display input field for typing word                       | major  | The input field provides the visual interface for users to enter text.                                           | None         |
| 2   | visual      | Display placeholder text "Enter a word..." in input field | minor  | Placeholder text provides helpful guidance on what users should type.                                            | C1           |
| 3   | visual      | Display "Find Rhymes" button                              | major  | The button provides a visible trigger element for initiating the search.                                         | None         |
| 4   | interaction | Show rhyming words when Enter key is pressed              | minor  | Pressing Enter gives users a keyboard shortcut for triggering the search.                                        | C1           |
| 5   | interaction | Show rhyming words when "Find Rhymes" button is clicked   | major  | Button click interaction provides an explicit trigger that works across all devices and input methods.           | C3           |
| 6   | state       | Search and identify rhyming words from word list           | major  | The rhyme-matching algorithm finds words with matching endings.                                                  | None         |
| 7   | state       | Limit results to maximum of 5 rhyming words               | minor  | Limiting to 5 keeps the results manageable without overwhelming users.                                           | C6           |
| 8   | content     | Display rhyming words in list below input                 | major  | The list shows users the dynamic search results data.                                                            | None         |
| 9   | content     | Display "No rhymes found" message when no matches exist   | minor  | The message communicates the empty search result state to users.                                                 | None         |
| 10  | interaction | Show "No rhymes found" in gray text when search returns no results | minor  | Gray styling provides subtle visual feedback for empty search results without appearing as an error.             | C9           |
| 11  | layout      | Position button next to input field                       | minor  | Placing the button beside the input creates a compact search interface.                                          | None         |
| 12  | layout      | Position results list below input field                   | minor  | Showing results below the input maintains clear top-to-bottom flow.                                              | None         |

## Justification

The Rhyme Finder works exactly as expected with straightforward rhyme search functionality. An input field displays where users can type a word, with a "Find Rhymes" button positioned next to it. When users press Enter or click the button, up to 5 rhyming words appear in a list below the input. If no rhymes are found, "No rhymes found" displays in gray text.
