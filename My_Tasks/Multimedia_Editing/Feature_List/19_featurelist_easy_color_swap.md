Category: Multimedia_Editing

Prompt style: Feature_List

Title: Image Slice Shuffler

Prompt: Build an image slice shuffler that randomly rearranges horizontal strips of uploaded images. Display an upload button at the top of the page. When users upload an image, show it on a canvas and automatically divide it into exactly 8 equal horizontal slices from top to bottom. Below the canvas, display a "Shuffle Slices" button. When users click the shuffle button, randomly rearrange the order of all 8 horizontal slices and redraw them on the canvas in their new positions, creating a scrambled glitch art effect where different parts of the image appear in wrong vertical positions. Each click produces a different random arrangement of the slices.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | content     | Display upload button                                     | major  | Upload button lets users choose which image to shuffle.                                                          | None         |
| 2   | content     | Display canvas                                            | major  | Canvas provides space for displaying the image.                                                                  | None         |
| 3   | content     | Display uploaded image on canvas                          | major  | Uploaded image shows what will be shuffled.                                                                      | C2           |
| 4   | state       | Divide image into exactly 8 equal horizontal slices       | major  | Dividing into 8 slices creates the pieces to rearrange.                                                          | C3           |
| 5   | content     | Display "Shuffle Slices" button                           | major  | Shuffle button triggers the rearrangement.                                                                       | C4           |
| 6   | content     | Display "Shuffle Slices" label on button                  | minor  | Label tells users what the button does.                                                                          | C5           |
| 7   | interaction | Rearrange slice order when button is clicked              | major  | Clicking shuffles the slices.                                                                                    | C5           |
| 8   | state       | Determine random positions for all 8 slices               | major  | Random positions create the glitch effect.                                                                       | C7           |
| 9   | state       | Redraw slices on canvas in new positions                  | major  | Redrawing updates the canvas with the shuffled result.                                                           | C8           |
| 10  | state       | Generate different random arrangement each click          | major  | Different arrangements each time keep it interesting.                                                            | C7           |

## Justification

The image slice shuffler works as a glitch art creator that scrambles horizontal strips of images. An upload button displays at the top of the page. When users upload an image, it appears on a canvas and automatically divides into exactly 8 equal horizontal slices from top to bottom. Below the canvas, a "Shuffle Slices" button displays. When users click the shuffle button, all 8 horizontal slices randomly rearrange their order and redraw on the canvas in their new positions, creating a scrambled glitch art effect where different parts of the image appear in wrong vertical positions. Each button click produces a different random arrangement of the slices.
