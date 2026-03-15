Category: Multimedia_Editing

Prompt style: Casual

Title: Image Kaleidoscope

Prompt: Need a kaleidoscope effect maker for images. Show a file upload button labeled "Upload Image" at the top. Once uploaded, display the image transformed into a kaleidoscope pattern with 6 mirrored triangular sections arranged in a circle. Below the kaleidoscope, show a slider labeled "Sections" ranging from 4 to 12. When I move the slider, update the kaleidoscope pattern in real-time to show that many mirrored sections. Add a "Download Kaleidoscope" button at the bottom to save the kaleidoscope image.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #  | ID          | Description                                              | Weight | Rationale                                                                          | Dependent On |
|----|-------------|----------------------------------------------------------|--------|------------------------------------------------------------------------------------|--------------|
| 1  | visual      | Display file upload button at the top                    | major  | The upload button lets users select their image to transform.                      | None         |
| 2  | content     | Label button "Upload Image"                              | minor  | The label tells users what the button does.                                        | C1           |
| 3  | visual      | Display image transformed into kaleidoscope pattern      | major  | The kaleidoscope transformation creates the visual effect users want.              | None         |
| 4  | state       | Show 6 mirrored triangular sections in a circle          | major  | The 6-section pattern provides the initial kaleidoscope layout.                    | C3           |
| 5  | layout      | Arrange sections in a circle                             | major  | Circular arrangement creates the traditional kaleidoscope appearance.              | C4           |
| 6  | visual      | Display slider below kaleidoscope                        | major  | The slider provides control for adjusting the pattern complexity.                  | None         |
| 7  | content     | Label slider "Sections"                                  | minor  | The label tells users what the slider controls.                                    | C6           |
| 8  | state       | Set slider range from 4 to 12                            | minor  | The 4-12 range provides enough variation without excessive complexity.             | None         |
| 9  | interaction | Update kaleidoscope pattern in real-time as slider moves | major  | Real-time updates let users see the effect as they adjust sections.                | None         |
| 10 | visual      | Display "Download Kaleidoscope" button at the bottom     | major  | The download button lets users save their kaleidoscope creation.                   | None         |
| 11 | interaction | Save kaleidoscope image when button clicked              | major  | Downloading provides the final output for users to use elsewhere.                  | None         |

## Justification

The Image Kaleidoscope works as expected with real-time pattern adjustment. A file upload button labeled "Upload Image" displays at the top for users to select their photo. Once uploaded, the image displays transformed into a kaleidoscope pattern with 6 mirrored triangular sections arranged in a circle. Below the kaleidoscope, a slider labeled "Sections" appears ranging from 4 to 12. When users move the slider, the kaleidoscope pattern updates in real-time to show that many mirrored sections. A "Download Kaleidoscope" button at the bottom allows users to save the kaleidoscope image.
