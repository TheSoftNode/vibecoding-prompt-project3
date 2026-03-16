Category: Multimedia_Editing

Prompt style: Feature_List

Title: Audio Reverse Player

Prompt: Build an audio reversal tool. Display a file upload button labeled "Upload Audio File" at the top. After uploading an audio file, show two audio players side by side. Label the left player "Original" and make it play the normal audio. Label the right player "Reversed" and make it play the audio backwards. Each player should have play and pause controls. Display the audio duration in seconds below each player.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display file upload button                               | major  | Users need a way to select their audio file for reversal.                          | None         |
| 2  | layout      | Position upload button at the top                        | minor  | Top positioning makes the upload control easy to find first.                       | C1           |
| 3  | content     | Label button "Upload Audio File"                         | minor  | A clear label helps users know what file type to upload.                           | C1           |
| 4  | visual      | Display two audio players after upload                   | major  | Dual players let users compare original and reversed audio side by side.           | None         |
| 5  | layout      | Position players side by side                            | major  | Side-by-side layout makes comparison between original and reversed easy.           | C4           |
| 6  | content     | Label left player "Original"                             | major  | The label tells users which player has the normal audio.                           | None         |
| 7  | content     | Label right player "Reversed"                            | major  | The label tells users which player has the backwards audio.                        | None         |
| 8  | visual      | Display play and pause controls on each player           | major  | Controls let users start and stop playback for comparison.                         | None         |
| 9  | interaction | Play audio when play button clicked on each player       | major  | Playing audio lets users hear the original and reversed versions.                  | None         |
| 10 | state       | Play audio backwards on Reversed player                  | major  | Backwards playback creates the reversal effect users want to hear.                 | None         |
| 11 | content     | Display audio duration in seconds below each player      | major  | Duration information shows users the length of each audio track.                   | None         |

## Justification

The Audio Reverse Player works as expected with dual playback comparison. A file upload button labeled "Upload Audio File" displays at the top for users to select their audio. After uploading, two audio players appear side by side with the left player labeled "Original" and the right player labeled "Reversed". Each player has play and pause controls. The Original player plays the normal audio while the Reversed player plays the audio backwards. The audio duration in seconds displays below each player.
