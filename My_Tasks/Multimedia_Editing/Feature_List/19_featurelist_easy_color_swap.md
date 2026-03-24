Category: Multimedia_Editing

Prompt style: Feature_List

Title: Image Slice Shuffler

Prompt: Build an image slice shuffler that randomly rearranges horizontal strips of uploaded images. Display an upload button at the top of the page. When users upload an image, show it on a canvas and automatically divide it into exactly 8 equal horizontal slices from top to bottom. Below the canvas, display a "Shuffle Slices" button. When users click the shuffle button, randomly rearrange the order of all 8 horizontal slices and redraw them on the canvas in their new positions, creating a scrambled glitch art effect where different parts of the image appear in wrong vertical positions. Each click produces a different random arrangement of the slices.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                                  | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button                                            | major  | The upload button helps users bring their image into the shuffler for slice rearrangement.                                 | None         |
| 2   | layout      | Position upload button at top of page                            | minor  | Positioning at the top makes the upload button easy to find so users can start shuffling quickly.                          | C1           |
| 3   | visual      | Display canvas                                                   | major  | The canvas provides a rendering surface for displaying the original and shuffled image slices.                             | None         |
| 4   | interaction | Display uploaded image on canvas after user uploads             | major  | Showing the image after upload lets users see what they uploaded before shuffling begins.                                  | C1           |
| 5   | state       | Divide image into exactly 8 equal horizontal slices              | major  | Dividing into exactly 8 equal slices creates the precise number of pieces needed for rearrangement.                        | C4           |
| 6   | state       | Divide slices from top to bottom                                 | minor  | Top-to-bottom division establishes the vertical orientation needed for horizontal slice shuffling.                         | C5           |
| 7   | visual      | Display "Shuffle Slices" button                                  | major  | The shuffle button gives users the control to trigger the rearrangement effect.                                            | None         |
| 8   | layout      | Position "Shuffle Slices" button below canvas                    | minor  | Placing button below the canvas creates clear workflow from viewing to action.                                             | C3, C7       |
| 9   | content     | Label button "Shuffle Slices"                                    | minor  | The label communicates what action the button performs.                                                                    | C7           |
| 10  | interaction | Rearrange slice order when button is clicked                     | major  | Clicking the button triggers the slice rearrangement that creates the glitch art effect.                                   | C7           |
| 11  | state       | Randomize positions for all 8 slices                             | major  | Random positioning creates the unpredictable scrambled appearance that defines the glitch art aesthetic.                   | C10          |
| 12  | state       | Redraw slices on canvas in new positions                         | major  | Redrawing updates the canvas with the shuffled result so users can see the glitch art effect.                              | C11          |
| 13  | state       | Generate different random arrangement on each click              | major  | Different arrangements each time provide variety and replayability for creating multiple glitch art variations.            | C10          |

## Justification

The image slice shuffler works as a glitch art creator that scrambles horizontal strips of images. An upload button displays at the top of the page. When users upload an image, it appears on a canvas and automatically divides into exactly 8 equal horizontal slices from top to bottom. Below the canvas, a "Shuffle Slices" button displays. When users click the shuffle button, all 8 horizontal slices randomly rearrange their order and redraw on the canvas in their new positions, creating a scrambled glitch art effect where different parts of the image appear in wrong vertical positions. Each button click produces a different random arrangement of the slices.
