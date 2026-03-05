Audio Visualizer
Example Audio Visualizer
Difficulty
Hard
Category
Multimedia Editing
Style
Feature List
Length
Moderate

**Prompt**

Create an audio visualizer. Let users upload an audio file or use their microphone.
Display animated vertical bars that react to audio frequencies in real-time using Canvas.
Add play/pause controls, volume slider, and color picker for the bars. Show current playback time.

**Difficulty: Hard**

| ID            | Description                                                             | Weight | Rationale                                                                                         | Dependent On |
| ------------- | ----------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------- | ------------ |
| visual-1      | Render a Canvas element for the visualization                           | major  | Canvas provides the performant 2D rendering context needed for real-time animated visualizations. | None         |
| visual-2      | Display a file upload input for loading audio files                     | major  | File upload provides users with a convenient way to load pre-recorded audio for visualization.    | None         |
| visual-3      | Display a button for starting microphone capture                        | major  | Microphone capture enables live audio input for real-time visualization.                          | None         |
| visual-4      | Display vertical bars on the Canvas representing audio frequencies      | major  | Vertical frequency bars are the primary visual representation in an audio visualizer.             | visual-1     |
| state-1       | Animate bar heights in real-time based on audio frequency data          | major  | Real-time animation is the defining characteristic that makes a visualizer responsive to audio.   | visual-4     |
| interaction-1 | Toggle audio playback when the user clicks the play/pause button        | major  | Play/pause control is essential for users to manage audio playback during visualization.          | None         |
| interaction-2 | Adjust audio volume when the user moves the volume slider               | minor  | Volume control allows users to adjust audio levels without leaving the application.               | None         |
| interaction-3 | Change bar colors when the user picks a new value from the color picker | major  | Color customization allows users to personalize the visual output of the visualizer.              | visual-4     |
| content-1     | Display the current playback time in seconds or MM:SS format            | major  | Displaying playback time provides essential temporal context during audio playback.               | None         |

Difficulty: Hard
ID
Description
Weight
Rationale
Dependent On
visual-1
Render a Canvas element for the visualization
major
Canvas provides the performant 2D rendering context needed for real-time animated visualizations.
None
visual-2
Display a file upload input for loading audio files
major
File upload provides users with a convenient way to load pre-recorded audio for visualization.
None
visual-3
Display a button for starting microphone capture
major
Microphone capture enables live audio input for real-time visualization.
None
visual-4
Display vertical bars on the Canvas representing audio frequencies
major
Vertical frequency bars are the primary visual representation in an audio visualizer.
visual-1
state-1
Animate bar heights in real-time based on audio frequency data
major
Real-time animation is the defining characteristic that makes a visualizer responsive to audio.
visual-4
interaction-1
Toggle audio playback when the user clicks the play/pause button
major
Play/pause control is essential for users to manage audio playback during visualization.
None
interaction-2
Adjust audio volume when the user moves the volume slider
minor
Volume control allows users to adjust audio levels without leaving the application.
None
interaction-3
Change bar colors when the user picks a new value from the color picker
major
Color customization allows users to personalize the visual output of the visualizer.
visual-4
content-1
Display the current playback time in seconds or MM:SS format
major
Displaying playback time provides essential temporal context during audio playback.
None
