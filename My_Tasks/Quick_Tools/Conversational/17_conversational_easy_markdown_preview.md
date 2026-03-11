Category: Quick_Tools

Prompt style: Conversational

Title: Live Markdown Previewer

Prompt: I need a markdown previewer with split view. On the left, show a textarea where I can type markdown syntax. On the right, display the rendered HTML preview. As I type in the textarea, update the preview in real-time. Support basic markdown: # for headings, **bold**, *italic*, and - for bullet lists.

Required libraries: react, tailwindcss, lucide-react, marked

## Rubric

| #   | ID          | Description                                              | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | -------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display textarea for markdown input                      | major  | The textarea is where users enter their markdown syntax for conversion.                                          | None         |
| 2   | visual      | Display preview area for rendered HTML                   | major  | The preview area shows the formatted output so users can see how their markdown will look.                       | None         |
| 3   | layout      | Position textarea on the left side                       | minor  | Left positioning for input creates the standard split-view editor layout.                                        | None         |
| 4   | layout      | Position preview area on the right side                  | minor  | Right positioning for output completes the split-view with input-output separation.                              | None         |
| 5   | state       | Store current markdown text from textarea                | major  | Storing the markdown text is necessary to process and convert it to HTML.                                        | None         |
| 6   | state       | Parse # syntax as heading                                | major  | Supporting heading syntax is essential for document structure in markdown.                                       | None         |
| 7   | state       | Parse **text** syntax as bold                            | major  | Supporting bold syntax lets users emphasize important text.                                                      | None         |
| 8   | state       | Parse *text* syntax as italic                            | major  | Supporting italic syntax provides text styling for emphasis.                                                     | None         |
| 9   | state       | Parse - syntax as bullet list                            | major  | Supporting bullet lists lets users create unordered lists in markdown.                                           | None         |
| 10  | content     | Display rendered HTML in preview area                    | major  | Showing the rendered HTML lets users verify their markdown converted correctly.                                  | None         |
| 11  | interaction | Update preview in real-time as user types                | major  | Real-time updates provide instant feedback so users see formatting changes immediately while typing.             | C1           |
| 12  | layout      | Display textarea and preview side by side                | minor  | Side-by-side layout lets users simultaneously view input and output without scrolling.                           | None         |

## Justification

The application achieved a 91.67% pass rate with one specific failure. A textarea for markdown input displays on the left where users can type. A preview area for rendered HTML displays on the right. The tool stores the current markdown text from the textarea and parses it, converting # to headings, **text** to bold, *text* to italic, and - to bullet lists. The rendered HTML displays in the preview area, updating in real-time as users type in the textarea, providing instant visual feedback of the formatted output. However, the model failed to display the textarea and preview side by side. Instead, the layout stacks them vertically with input above and preview below, not side-by-side as required for the split-view design. This positioning issue caused the failure despite all other functionality working correctly.
