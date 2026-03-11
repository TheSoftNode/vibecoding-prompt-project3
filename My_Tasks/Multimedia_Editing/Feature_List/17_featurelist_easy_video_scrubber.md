Category: Multimedia Editing

Prompt style: Feature_List

Title: Video Thumbnail Scrubber

Prompt: Build a video scrubber with these features:
- Upload a video file and display it in a video player with playback controls
- Show a timeline scrubber below the video where dragging a marker updates the video to that timestamp and displays a thumbnail preview of the frame at that position

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                  | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ------------------------------------------------------------ | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button for video file                         | major  | The upload button is how users load their video into the scrubber for timeline navigation.                       | None         |
| 2   | visual      | Display video player element                                 | major  | The video player shows the current frame and allows users to see the video content.                              | None         |
| 3   | visual      | Display playback controls on video player                    | major  | Playback controls (play, pause) let users control video playback in addition to scrubbing.                       | None         |
| 4   | visual      | Display timeline scrubber below video                        | major  | The timeline scrubber provides the interface for navigating to different video timestamps.                       | None         |
| 5   | layout      | Position timeline scrubber below the video player            | minor  | Placing the scrubber below creates a standard video editor layout with controls under the preview.               | None         |
| 6   | visual      | Display draggable marker on timeline                         | major  | The draggable marker is the handle users interact with to scrub through the video.                               | None         |
| 7   | interaction | Update video timestamp when marker is dragged                | major  | Updating the video to match the marker position lets users jump to any point in the timeline.                    | C6           |
| 8   | state       | Calculate current video frame from marker position           | major  | Calculating the frame from position is necessary to show the correct video timestamp.                            | None         |
| 9   | visual      | Display thumbnail preview of current frame                   | major  | The thumbnail shows a visual preview of what's at that timeline position before committing to that timestamp.    | None         |
| 10  | interaction | Update thumbnail preview when marker is dragged              | major  | Real-time thumbnail updates let users see exactly what frame they're scrubbing to while dragging.                | C6           |
| 11  | layout      | Position thumbnail preview near the timeline marker          | minor  | Placing the thumbnail near the marker keeps the preview close to the user's cursor for easy viewing.             | None         |

## Justification

The application achieved a 90.91% pass rate with one specific failure. An upload button allows users to load a video file. The video displays in a video player with playback controls (play, pause). Below the video, a timeline scrubber appears with a draggable marker. As users drag the marker along the timeline, the video updates to show the timestamp at that position, and a thumbnail preview displays showing the frame at that location. The thumbnail updates in real-time as the marker moves, providing visual feedback about what content is at each timeline position. However, the model failed to position the thumbnail preview near the timeline marker. Instead, the thumbnail appears in a fixed position above the timeline or in a separate preview panel to the side, not near the draggable marker as required. This positioning issue caused the failure despite all other functionality working correctly.
