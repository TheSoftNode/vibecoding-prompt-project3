Category: Multimedia_Editing

Prompt style: Casual

Title: Image Orbit Animator

Prompt: Load default center image. Upload second image that orbits around it in a circle. Speed slider controls orbit animation. Draw line connecting the two images.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                 | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | state       | Load tool with default center image                         | major  | Loading with a default image shows users what the center anchor looks like immediately.                          | None         |
| 2   | visual      | Display center image at canvas center                       | major  | Positioning at center creates the anchor point for the orbiting image to circle around.                          | None         |
| 3   | visual      | Display upload button for orbiting image                    | major  | The upload button lets users select their own image to animate in orbit.                                         | None         |
| 4   | interaction | Display uploaded image when user uploads                    | major  | Showing the uploaded image lets users see what's orbiting around the center.                                     | None         |
| 5   | state       | Animate uploaded image in circular orbit around center      | major  | Circular orbit creates the rotating animation effect around the center image.                                    | C4           |
| 6   | visual      | Display speed slider for orbit animation                    | major  | The slider gives users control over how fast the image orbits.                                                   | None         |
| 7   | interaction | Adjust orbit speed when slider moves                        | major  | Changing speed lets users customize the animation to their preference.                                           | C6           |
| 8   | state       | Keep both images visible during orbit animation             | major  | Both images must stay visible so users see the complete orbit effect.                                            | C5           |
| 9   | visual      | Draw line connecting center and orbiting images             | major  | The connecting line visualizes the relationship between the two images.                                          | None         |
| 10  | state       | Update line position as orbiting image moves                | major  | The line must track the moving image to maintain the connection throughout orbit.                                | C5, C9       |
| 11  | layout      | Position line endpoints at image centers                    | major  | Connecting at centers keeps the line properly attached to both images.                                           | C9           |
| 12  | state       | Maintain constant orbit radius during animation             | minor  | Consistent radius creates a smooth circular path rather than an erratic wobble.                                  | C5           |

## Justification

The Image Orbit Animator creates a dynamic animation where one image orbits around another with a connecting line. The tool loads with a default center image positioned at the canvas center. An upload button lets users select a second image which displays and animates in a circular orbit around the center image at a constant radius. A speed slider controls how fast the orbit animation runs. As the slider moves, the orbit speed adjusts accordingly. Both images remain visible during the animation. A line draws connecting the center and orbiting images with endpoints at each image's center. The line position updates continuously as the orbiting image moves, tracking the animation to maintain the visual connection.
