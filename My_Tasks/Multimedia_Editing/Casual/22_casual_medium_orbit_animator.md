Category: Multimedia_Editing

Prompt style: Casual

Title: Image Orbit Animator

Prompt: Upload center image. Upload orbiting image. Radius slider adjusts distance. Speed slider controls orbit. Line connects both.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                 | Weight | Rationale                                                                                                        | Dependent On |
| --- | ----------- | ----------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button for center image                      | major  | The upload button lets users select the center anchor image.                                                     | None         |
| 2   | interaction | Display center image at canvas center after upload          | major  | Positioning at center creates the anchor point for the orbiting image to circle around.                          | None         |
| 3   | visual      | Display upload button for orbiting image                    | major  | The upload button lets users select their own image to animate in orbit.                                         | None         |
| 4   | interaction | Display orbiting image when user uploads                    | major  | Showing the uploaded image lets users see what's orbiting around the center.                                     | None         |
| 5   | state       | Animate orbiting image in circular path around center       | major  | Circular orbit creates the rotating animation effect around the center image.                                    | C4           |
| 6   | visual      | Display radius slider for orbit distance                    | major  | The radius slider gives users control over how far from center the image orbits.                                 | None         |
| 7   | interaction | Adjust orbit distance when radius slider moves              | major  | Changing radius lets users customize the orbit size.                                                             | C6           |
| 8   | visual      | Display speed slider for orbit animation                    | major  | The speed slider gives users control over how fast the image orbits.                                             | None         |
| 9   | interaction | Adjust orbit speed when speed slider moves                  | major  | Changing speed lets users customize the animation pace.                                                          | C8           |
| 10  | state       | Keep both images visible during orbit animation             | major  | Both images must stay visible so users see the complete orbit effect.                                            | C5           |
| 11  | visual      | Draw line connecting center and orbiting images             | major  | The connecting line visualizes the relationship between the two images.                                          | None         |
| 12  | state       | Update line position as orbiting image moves                | major  | The line must track the moving image to maintain the connection throughout orbit.                                | C5, C11      |
| 13  | layout      | Position line endpoints at image centers                    | major  | Connecting at centers keeps the line properly attached to both images.                                           | C11          |

## Justification

The Image Orbit Animator creates a dynamic animation where one image orbits around another with adjustable distance and speed. An upload button lets users select a center image which displays at the canvas center. A second upload button lets users select an orbiting image which displays and animates in a circular path around the center image. A radius slider adjusts the orbit distance from the center. A speed slider controls how fast the orbit animation runs. Both images remain visible during the animation. A line draws connecting the center and orbiting images with endpoints at each image's center. The line position updates continuously as the orbiting image moves, tracking the animation to maintain the visual connection.
