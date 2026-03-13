Category: Quick_Tools

Prompt style: Feature_List

Title: Rhyme Finder

Prompt: Build a rhyme finder tool. Display an input field where users type a word, with a "Find Rhymes" button next to it. When pressing Enter or clicking the button, show up to 5 rhyming words in a list below the input, with the matching ending highlighted in blue on each word. If no rhymes are found, display "No rhymes found" in gray text.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display input field for typing word                       | major  | The input field lets users enter the word they want to find rhymes for.                                          | None         |
| 2   | content     | Display "Find Rhymes" button                              | major  | The button gives users the control to trigger the rhyme search.                                                  | None         |
| 3   | interaction | Show rhyming words when Enter key is pressed              | minor  | Pressing Enter gives users a keyboard shortcut for triggering the search.                                        | C1           |
| 4   | interaction | Show rhyming words when "Find Rhymes" button is clicked   | major  | Clicking the button displays the rhyme results.                                                                  | C2           |
| 5   | state       | Limit results to maximum of 5 rhyming words               | minor  | Limiting to 5 keeps the results manageable without overwhelming users.                                           | None         |
| 6   | content     | Display rhyming words in list below input                 | major  | The list shows users which words rhyme with their typed word.                                                    | None         |
| 7   | visual      | Highlight matching ending in blue on each rhyme           | minor  | Blue highlighting draws attention to the part of the word that rhymes.                                           | C6           |
| 8   | content     | Display "No rhymes found" when no matches exist           | minor  | The message tells users the search didn't find any rhyming words.                                                | None         |
| 9   | visual      | Display "No rhymes found" in gray text                    | minor  | Gray color makes the no-results message appear less harsh than an error.                                         | C8           |
| 10  | layout      | Position button next to input field                       | minor  | Placing the button beside the input creates a compact search interface.                                          | None         |
| 11  | layout      | Position results list below input field                   | minor  | Showing results below the input maintains clear top-to-bottom flow.                                              | None         |

## Justification

The Rhyme Finder works exactly as expected with rhyme search and highlighted endings. An input field displays where users can type a word, with a "Find Rhymes" button positioned next to it. When users press Enter or click the button, up to 5 rhyming words appear in a list below the input, with the matching ending highlighted in blue on each word. If no rhymes are found, "No rhymes found" displays in gray text.
