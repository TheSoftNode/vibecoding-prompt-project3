Category: Quick_Tools

Prompt style: Feature_List

Title: Rhyme Finder

Prompt: Build a rhyme finder tool. Display an input field where users can type a word. When pressing Enter or clicking a "Find Rhymes" button, search a predefined dictionary of 100 common words and display up to 5 words that rhyme with the input by matching the last 2 or more letters. Show matching rhymes in a list below the input with the matching ending highlighted in blue. If no rhymes are found, display "No rhymes found" in gray text.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display input field for typing word                       | major  | The input field is where users type the word they want rhymes for.                                               | None         |
| 2   | visual      | Display "Find Rhymes" button                              | major  | The button triggers the rhyme search when clicked.                                                               | None         |
| 3   | interaction | Trigger search when Enter key is pressed                  | minor  | Pressing Enter gives users a keyboard shortcut instead of clicking the button.                                   | None         |
| 4   | interaction | Trigger search when "Find Rhymes" button is clicked       | major  | Clicking the button starts the rhyme matching process.                                                           | None         |
| 5   | state       | Search predefined dictionary of 100 common words          | major  | The dictionary provides the word pool to search through for rhymes.                                              | None         |
| 6   | state       | Match words by last 2 or more letters                     | major  | Matching ending letters finds words that rhyme by sound similarity.                                              | None         |
| 7   | state       | Limit results to 5 rhyming words maximum                  | minor  | Limiting to 5 keeps the list short and prevents overwhelming users with too many results.                        | None         |
| 8   | visual      | Display matching rhymes in list below input               | major  | The list shows users which words rhyme with their input word.                                                    | None         |
| 9   | content     | Highlight matching ending in blue on each rhyme           | minor  | Highlighting the ending shows users exactly which part of the word matches.                                      | C6           |
| 10  | content     | Display "No rhymes found" when no matches exist           | minor  | The message tells users when the search came up empty.                                                           | None         |
| 11  | visual      | Display "No rhymes found" in gray text                    | minor  | Gray color makes the message appear softer than an error.                                                        | C10          |

## Justification

The rhyme finder tool works exactly as expected with dictionary search and highlighted matches. An input field displays where users can type a word. A "Find Rhymes" button appears next to the input. When users press Enter or click the button, the tool searches a predefined dictionary of 100 common words and matches words by comparing the last 2 or more letters. Up to 5 rhyming words display in a list below the input, with the matching ending highlighted in blue on each word. If no rhymes match the input word, "No rhymes found" displays in gray text instead of showing an empty list.
