Category: Multimedia_Editing

Prompt style: Feature_List

Title: Audio Reverse Player

Prompt: Build an audio reversal tool. Display a file upload button labeled "Upload Audio File" at the top. After uploading an audio file, show two audio players side by side: the left player labeled "Original" plays the normal audio, and the right player labeled "Reversed" plays the audio backwards. Each player should have play and pause controls. Display the audio duration in seconds below each player. Add a "Download Reversed Audio" button at the bottom to save the backwards version as a file.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display file upload button at the top                    | major  | The upload button lets users select their audio file.                              | None         |
| 2  | content     | Label button "Upload Audio File"                         | minor  | The label tells users what file type to upload.                                    | C1           |
| 3  | visual      | Display two audio players side by side                   | major  | Side-by-side players let users compare original and reversed audio.                | None         |
| 4  | layout      | Position left player on left side                        | minor  | Left positioning creates clear spatial separation.                                 | C3           |
| 5  | layout      | Position right player on right side                      | minor  | Right positioning creates clear spatial separation.                                | C3           |
| 6  | content     | Label left player "Original"                             | major  | The label tells users this player has the normal audio.                            | None         |
| 7  | content     | Label right player "Reversed"                            | major  | The label tells users this player has the backwards audio.                         | None         |
| 8  | visual      | Display play and pause controls on each player           | major  | Controls let users start and stop playback for comparison.                         | None         |
| 9  | state       | Play normal audio on Original player                     | major  | Normal playback provides the reference for comparison.                             | None         |
| 10 | state       | Play audio backwards on Reversed player                  | major  | Backwards playback creates the reversal effect users want.                         | None         |
| 11 | content     | Display audio duration in seconds below each player      | major  | Duration shows users the length of each audio track.                               | None         |
| 12 | visual      | Display "Download Reversed Audio" button at the bottom   | major  | The download button lets users save the backwards audio.                           | None         |
| 13 | interaction | Save reversed audio when Download button clicked         | major  | Downloading provides the final output for users to use elsewhere.                  | None         |

## Justification

The Audio Reverse Player works as expected with dual playback comparison. A file upload button labeled "Upload Audio File" displays at the top for users to select their audio. After uploading, two audio players appear side by side with the left player labeled "Original" and the right player labeled "Reversed". Each player has play and pause controls. The Original player plays the normal audio while the Reversed player plays the audio backwards. The audio duration in seconds displays below each player. A "Download Reversed Audio" button at the bottom allows users to save the backwards version as a file.
