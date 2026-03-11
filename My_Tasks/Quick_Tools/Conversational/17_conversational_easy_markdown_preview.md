Category: Quick_Tools

Prompt style: Conversational

Title: Live Markdown Previewer

Prompt: I need a markdown previewer with split view. On the left, show a textarea where I can type markdown syntax. On the right, display the rendered HTML preview. As I type in the textarea, update the preview in real-time. Support basic markdown: # for headings, **bold**, *italic*, and - for bullet lists.

Required libraries: react, tailwindcss, lucide-react, marked

## Rubric

| #   | ID          | Description                                              | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | -------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display textarea for markdown input                      | major  | Users need a text area to type their markdown syntax.                                                            | None         |
| 2   | visual      | Display preview area for rendered HTML                   | major  | The preview shows what the markdown will look like when formatted.                                               | None         |
| 3   | layout      | Position textarea on the left side                       | minor  | Left side for input keeps the split-view organized with a clear input-output flow.                               | None         |
| 4   | layout      | Position preview area on the right side                  | minor  | Right side for output completes the split layout so users can see both at once.                                  | None         |
| 5   | state       | Parse # syntax as heading                                | major  | Headings let users structure their documents with titles and sections.                                           | None         |
| 6   | state       | Parse **text** syntax as bold                            | major  | Bold formatting helps users emphasize key words or phrases.                                                      | None         |
| 7   | state       | Parse *text* syntax as italic                            | major  | Italics give users another way to add emphasis or style to their text.                                           | None         |
| 8   | state       | Parse - syntax as bullet list                            | major  | Bullet lists make it easy to create unordered lists without manual formatting.                                   | None         |
| 9   | content     | Display rendered HTML in preview area                    | major  | Showing the HTML output confirms that the markdown converted correctly.                                          | None         |
| 10  | interaction | Update preview in real-time as user types                | major  | Real-time updates mean users see their formatting immediately without clicking a button.                         | C1           |

## Justification

The application achieved a 90.00% pass rate with one specific failure. A textarea for markdown input displays on the left where users can type. A preview area for rendered HTML displays on the right. The tool parses markdown syntax, converting # to headings, **text** to bold, *text* to italic, and - to bullet lists. The rendered HTML displays in the preview area, updating in real-time as users type in the textarea, showing formatting changes immediately without delay. However, the model failed to position the preview area on the right side. Instead, the preview stacks below the textarea in a vertical layout, not on the right as required for the split-view design. This positioning issue caused the failure despite all other functionality working correctly.
