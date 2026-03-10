Category: Multimedia Editing

Prompt style: Feature List

Title: NFT Thumbnail Watermark Generator

Prompt: Build an NFT thumbnail generator with wallet address watermark. Upload an image file to display as preview. Show input field to enter Ethereum wallet address (0x format). As I type the wallet address, automatically validate it shows 42 characters starting with 0x and display "Valid" or "Invalid" status in green or red. Add watermark button that overlays the wallet address in bottom-right corner of the image in white text with 30% black background. Display character count showing current length out of 42 total as I type.

Required libraries: react, tailwindcss, lucide-react, html2canvas

## Rubric

| #   | ID          | Description                                                      | Weight | Rationale                                                                                                                         | Dependent On |
| --- | ----------- | ---------------------------------------------------------------- | ------ | --------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display upload button for image file                             | major  | The upload button gives users the starting point to select their NFT image.                                                       | None         |
| 2   | interaction | Display uploaded image as preview when file is selected          | major  | Uploading shows the image so users can see where the watermark will appear.                                                       | C1           |
| 3   | visual      | Display input field to enter Ethereum wallet address             | major  | The input field lets users type their wallet address that will become the watermark.                                              | None         |
| 4   | content     | Display placeholder "0x..." in wallet address input field        | minor  | The placeholder format guides users to enter a proper Ethereum address starting with 0x.                                          | C3           |
| 5   | state       | Validate wallet address has 42 characters starting with 0x       | major  | Validation checks the address format to make sure it matches Ethereum's standard length and prefix.                               | None         |
| 6   | content     | Display "Valid" status in green when address is correct          | major  | Green "Valid" tells users their wallet address format is right so they can proceed.                                               | C5           |
| 7   | content     | Display "Invalid" status in red when address is incorrect        | major  | Red "Invalid" alerts users their address format needs fixing before watermarking.                                                 | C5           |
| 8   | state       | Calculate character count as user types in input field           | major  | Counting characters helps users track how close they are to the required 42-character length.                                     | None         |
| 9   | content     | Display character count showing current length out of 42 total   | major  | Showing "X/42" gives users a clear progress indicator for typing the full address.                                                | C8           |
| 10  | visual      | Display "Add Watermark" button                                   | major  | The watermark button lets users trigger adding their address to the image once it's valid.                                        | None         |
| 11  | interaction | Add wallet address watermark in bottom-right corner when button clicked | major  | Clicking adds the watermark to the image at the specified position creating the final NFT thumbnail.                              | C2           |
| 12  | layout      | Position watermark text in bottom-right corner of image          | minor  | Bottom-right placement keeps the watermark visible but doesn't cover the main subject of most images.                             | None         |

## Justification

The NFT thumbnail watermark generator works as an easy two-feature tool for adding wallet address watermarks to NFT images. An upload button allows selecting an image file which displays as a preview. An input field with "0x..." placeholder lets users enter their Ethereum wallet address. As they type, the tool validates the address has 42 characters starting with 0x and displays "Valid" in green or "Invalid" in red. It also calculates and shows the character count as "X/42" so users know their progress. An "Add Watermark" button overlays the wallet address in the bottom-right corner of the image in white text with 30% black background, creating the final watermarked NFT thumbnail.
