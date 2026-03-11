Category: Multimedia Editing

Prompt style: Conversational

Title: Audio Waveform Trimmer

Prompt: I need an audio trimming tool that shows a visual waveform. When I upload an audio file, display its waveform as a series of vertical bars representing amplitude over time. Below the waveform, show two draggable markers labeled "Start" and "End" positioned at 0% and 100% by default. As I drag these markers along the timeline, highlight the section between them in blue to show the trim selection.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                       | Weight | Rationale                                                                                                              | Dependent On |
| --- | ----------- | ----------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button for audio file                              | major  | Without an upload button, users can't load their audio file into the trimmer.                                          | None         |
| 2   | visual      | Display waveform as vertical bars representing amplitude          | major  | The waveform visualization shows the audio structure so users can identify where to trim.                              | None         |
| 3   | layout      | Position waveform above the trim markers                          | minor  | Placing the waveform above markers creates a clear top-to-bottom flow from visualization to controls.                  | None         |
| 4   | visual      | Display "Start" marker on timeline                                | major  | The Start marker is essential for users to set where their trimmed audio should begin.                                 | None         |
| 5   | visual      | Display "End" marker on timeline                                  | major  | The End marker is essential for users to set where their trimmed audio should end.                                     | None         |
| 6   | content     | Display label "Start" on first marker                             | minor  | Labeling the marker "Start" clarifies its purpose so users don't confuse it with the End marker.                       | None         |
| 7   | content     | Display label "End" on second marker                              | minor  | Labeling the marker "End" makes it immediately clear which boundary it controls.                                       | None         |
| 8   | state       | Set Start marker to 0% position by default                        | minor  | Starting at 0% means the full audio is selected initially, giving users the full range to trim from.                   | None         |
| 9   | state       | Set End marker to 100% position by default                        | minor  | Ending at 100% ensures the full audio is selected by default before users adjust the trim points.                      | None         |
| 10  | interaction | Move Start marker position when dragged along timeline            | major  | Draggable Start marker lets users interactively choose where the trimmed audio begins.                                 | C4           |
| 11  | interaction | Move End marker position when dragged along timeline              | major  | Draggable End marker lets users interactively choose where the trimmed audio ends.                                     | C5           |
| 12  | visual      | Highlight section between Start and End markers in blue           | major  | Blue highlighting shows exactly which portion of the audio will be kept after trimming.                                | None         |

## Justification

The application achieved a 91.67% pass rate with one specific failure. An upload button allows users to load an audio file, which then displays as a waveform of vertical bars showing amplitude over time. The waveform appears above the timeline controls. Two markers labeled "Start" and "End" appear on the timeline, positioned at 0% and 100% by default. Users can drag the Start marker and End marker along the timeline to adjust trim points. The section between the markers highlights in blue to show the selected trim area for trimming. However, the model failed to position the waveform above the trim markers. Instead, the waveform appears to the left side with markers on the right in a horizontal layout, not above as required for the top-to-bottom flow. This positioning issue caused the failure despite all other functionality working correctly.
