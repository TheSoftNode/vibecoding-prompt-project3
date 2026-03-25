Category: Web_Application

Prompt style: Feature_List

Title: Text Character Counter

Prompt: Build a text character counter tool that analyzes user input in real-time. Display a text area labeled "Enter your text" at the top of the page. Below the text area, display three counters in a row: "Characters: 0", "Words: 0", and "Sentences: 0". When users type or paste text into the text area, immediately update all three counters to show the current count of characters (including spaces), words (separated by spaces), and sentences (ending with periods, question marks, or exclamation marks). Display a "Clear" button below the counters that, when clicked, empties the text area and resets all three counters back to 0.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                     | Weight | Rationale                                                                                      | Dependent On |
| --- | ----------- | --------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display text area                                               | major  | The text area provides the input field where users enter text for analysis.                    | None         |
| 2   | content     | Label text area "Enter your text"                               | minor  | The label tells users what action to take with the text area.                                  | C1           |
| 3   | layout      | Position text area at top of page                               | minor  | Top positioning makes the input field the first element users interact with.                   | C1           |
| 4   | content     | Display character counter showing "Characters: 0"               | major  | The character counter shows users how many characters are in their text.                       | None         |
| 5   | content     | Display word counter showing "Words: 0"                         | major  | The word counter shows users how many words are in their text.                                 | None         |
| 6   | content     | Display sentence counter showing "Sentences: 0"                 | major  | The sentence counter shows users how many sentences are in their text.                         | None         |
| 7   | layout      | Position three counters in a row below text area                | minor  | Row positioning groups the counters together for easy comparison.                              | C4, C5, C6   |
| 8   | interaction | Update counters when user types in text area                    | major  | Typing triggers real-time analysis of the text content.                                        | C1           |
| 9   | state       | Count total characters including spaces                         | major  | Counting all characters provides the full length measurement of the text.                      | C8           |
| 10  | state       | Count words separated by spaces                                 | major  | Counting words separated by spaces identifies individual word units in the text.               | C8           |
| 11  | state       | Count sentences ending with periods, question marks, or exclamation marks | major  | Counting sentence-ending punctuation identifies complete sentence units in the text.    | C8           |
| 12  | content     | Update character counter display immediately                    | major  | Immediate updates show the current character count in real-time as users type.                 | C9           |
| 13  | content     | Update word counter display immediately                         | major  | Immediate updates show the current word count in real-time as users type.                      | C10          |
| 14  | content     | Update sentence counter display immediately                     | major  | Immediate updates show the current sentence count in real-time as users type.                  | C11          |
| 15  | visual      | Display Clear button                                            | major  | The Clear button gives users control to reset the tool for new text analysis.                  | None         |
| 16  | layout      | Position Clear button below counters                            | minor  | Below positioning separates the reset action from the active counting display.                 | C7, C15      |
| 17  | interaction | Empty text area when Clear button clicked                       | major  | Clicking Clear removes all text from the input field.                                          | C15          |
| 18  | state       | Reset all counters to 0 when Clear button clicked              | major  | Resetting counters restores the initial state for analyzing new text.                          | C17          |

## Justification

The text character counter tool works as a real-time text analysis utility with immediate feedback. A text area labeled "Enter your text" displays at the top of the page. Below it, three counters display in a row showing "Characters: 0", "Words: 0", and "Sentences: 0". When users type or paste text into the text area, the tool immediately counts total characters including spaces, words separated by spaces, and sentences ending with periods, question marks, or exclamation marks, updating all three counter displays in real-time. A Clear button displays below the counters that, when clicked, empties the text area and resets all three counters back to 0, preparing the tool for new text analysis.
