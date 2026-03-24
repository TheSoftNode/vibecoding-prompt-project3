Category: Multimedia_Editing

Prompt style: Feature_List

Title: Image Slice Shuffler

Prompt: Build an image slice shuffler that randomly rearranges horizontal strips of uploaded images. Display an upload button at the top of the page. When users upload an image, show it on a canvas and automatically divide it into exactly 8 equal horizontal slices from top to bottom. Below the canvas, display a "Shuffle Slices" button. When users click the shuffle button, randomly rearrange the order of all 8 horizontal slices and redraw them on the canvas in their new positions, creating a scrambled glitch art effect where different parts of the image appear in wrong vertical positions. Each click produces a different random arrangement of the slices.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                               | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | --------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button at top of page                      | major  | Upload button lets users select an image to shuffle.                                                             | None         |
| 2   | layout      | Position upload button at top of page                     | minor  | Top positioning makes upload control immediately visible.                                                        | C1           |
| 3   | visual      | Display uploaded image on canvas                          | major  | Canvas shows the image that will be sliced and shuffled.                                                         | None         |
| 4   | state       | Divide image into exactly 8 equal horizontal slices       | major  | Eight slices create the segments that will be rearranged.                                                        | C3           |
| 5   | visual      | Display "Shuffle Slices" button below canvas             | major  | Shuffle button triggers the slice rearrangement effect.                                                          | None         |
| 6   | layout      | Position "Shuffle Slices" button below canvas            | minor  | Below positioning keeps the button separate from the image.                                                      | C5           |
| 7   | content     | Display "Shuffle Slices" label on button                  | minor  | Label clarifies the button's rearrangement function.                                                             | C5           |
| 8   | interaction | Rearrange slice order when button is clicked              | major  | Clicking triggers the slice shuffling effect.                                                                    | C5           |
| 9   | state       | Randomly determine new positions for all 8 slices         | major  | Random positioning creates the scrambled glitch effect.                                                          | C8           |
| 10  | state       | Redraw slices on canvas in new positions                  | major  | Redrawing shows the rearranged slices in their shuffled order.                                                   | C9           |
| 11  | state       | Generate different random arrangement each click          | major  | Each click produces a new shuffle pattern for variety.                                                           | C8           |

## Justification

The image slice shuffler works as a glitch art creator that scrambles horizontal strips of images. An upload button displays at the top of the page. When users upload an image, it appears on a canvas and automatically divides into exactly 8 equal horizontal slices from top to bottom. Below the canvas, a "Shuffle Slices" button displays. When users click the shuffle button, all 8 horizontal slices randomly rearrange their order and redraw on the canvas in their new positions, creating a scrambled glitch art effect where different parts of the image appear in wrong vertical positions. Each button click produces a different random arrangement of the slices.
