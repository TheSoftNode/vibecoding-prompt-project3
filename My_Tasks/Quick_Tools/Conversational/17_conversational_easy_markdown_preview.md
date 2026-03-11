Category: Quick_Tools

Prompt style: Conversational

Title: Live Markdown Previewer

Prompt: I need a markdown previewer with split view. On the left, show a textarea labeled "Markdown Input" where I can type markdown syntax. On the right, display the rendered HTML preview. As I type in the textarea, update the preview in real-time. Support basic markdown: # for headings, ** for bold, * for italic, and - for bullet lists.

Required libraries: react, tailwindcss, lucide-react, marked

## Rubric

| #   | ID          | Description                                              | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | -------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display textarea for markdown input                      | major  | Users need a text area to type their markdown syntax.                                                            | None         |
| 2   | content     | Display label "Markdown Input" on textarea               | minor  | The label tells users what the text area is for.                                                                 | None         |
| 3   | visual      | Display preview area for rendered HTML                   | major  | The preview shows what the markdown will look like when formatted.                                               | None         |
| 4   | layout      | Position textarea on the left side                       | minor  | Left side for input keeps the split-view organized with a clear input-output flow.                               | None         |
| 5   | layout      | Position preview area on the right side                  | minor  | Right side for output completes the split layout so users can see both at once.                                  | None         |
| 6   | state       | Parse # syntax as heading                                | major  | Headings let users structure their documents with titles and sections.                                           | None         |
| 7   | state       | Parse **bold** syntax as bold text                       | major  | Bold formatting helps users emphasize key words or phrases.                                                      | None         |
| 8   | state       | Parse *italic* syntax as italic text                     | major  | Italics give users another way to add emphasis or style to their text.                                           | None         |
| 9   | state       | Parse - syntax as bullet list                            | major  | Bullet lists make it easy to create unordered lists without manual formatting.                                   | None         |
| 10  | state       | Display rendered HTML in preview area                    | major  | Showing the HTML output confirms that the markdown converted correctly.                                          | None         |
| 11  | interaction | Update preview in real-time as user types                | major  | Real-time updates mean users see their formatting immediately without clicking a button.                         | C1           |

## Justification

The application achieved a 90.91% pass rate with one specific failure. A textarea labeled "Markdown Input" displays on the left where users can type. A preview area for rendered HTML displays on the right. The tool parses markdown syntax, converting # to headings, **bold** to bold text, *italic* to italic text, and - to bullet lists. The rendered HTML displays in the preview area, updating in real-time as users type in the textarea, showing formatting changes immediately without delay. However, the model failed to position the preview area on the right side. Instead, the preview stacks below the textarea in a vertical layout, not on the right as required for the split-view design. This positioning issue caused the failure despite all other functionality working correctly.
