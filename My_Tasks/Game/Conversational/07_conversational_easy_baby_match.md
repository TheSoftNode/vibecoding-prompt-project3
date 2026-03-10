Category: Game

Prompt style: Conversational

Title: Baby Animal Matching Game

Prompt: I want a baby education game to teach animal names. Show an animal image in the center with a name label below it. Sometimes the name matches the animal, sometimes it doesn't. Add two buttons at the bottom: a green checkmark button on the left and a red X button on the right. When the name matches the animal (like a cat image with "Cat" label), tapping the checkmark is correct. When the name doesn't match (like a dog image with "Cat" label), tapping the X is correct. After tapping either button, show "Correct!" in green or "Wrong!" in red text below the buttons. Then automatically show the next animal after 1 second. Use these 4 animals in sequence: Cat with "Cat", Dog with "Bird", Cow with "Cow", Bird with "Dog".

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                      | Weight | Rationale                                                                                                                    | Dependent On |
| --- | ----------- | -------------------------------------------------------------------------------- | ------ | ---------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display animal image in the center                                              | major  | The animal image provides the visual element that children identify and match with the name label.                           | None         |
| 2   | content     | Display name label below the animal image                                       | major  | The name label shows the text that children must verify matches or doesn't match the displayed animal.                       | None         |
| 3   | visual      | Display green checkmark button                                                  | major  | The green checkmark button provides the interface for children to indicate the name matches the animal.                      | None         |
| 4   | visual      | Display red X button                                                            | major  | The red X button provides the interface for children to indicate the name doesn't match the animal.                          | None         |
| 5   | layout      | Position checkmark button on the left and X button on the right at bottom       | minor  | Left-right positioning with checkmark on left and X on right creates intuitive yes/no choice layout for young children.      | None         |
| 6   | state       | Determine if name matches animal for each card                                  | major  | Match determination defines whether checkmark or X is the correct answer for the current animal-name pair.                   | None         |
| 7   | interaction | Show "Correct!" in green text when correct button is tapped                     | major  | Green "Correct!" provides positive reinforcement feedback when children make the right choice.                               | None         |
| 8   | interaction | Show "Wrong!" in red text when incorrect button is tapped                       | major  | Red "Wrong!" provides corrective feedback when children make the wrong choice.                                               | None         |
| 9   | state       | Automatically advance to next animal after 1 second                             | major  | Automatic progression keeps the game moving and maintains engagement for young children without requiring navigation clicks. | None         |
| 10  | content     | Display 4 animals in sequence: Cat with "Cat", Dog with "Bird", Cow with "Cow", Bird with "Dog" | major  | The specific animal-name pairs provide both matching examples (Cat/Cat, Cow/Cow) and mismatching examples (Dog/Bird, Bird/Dog) to teach name recognition. | None         |

## Justification

The baby animal matching game works exactly as expected with animal images and name labels that children verify as matching or not matching. An animal image displays in the center with a name label shown below it. At the bottom, a green checkmark button appears on the left and a red X button appears on the right. The game shows four animals in sequence: Cat with "Cat" label (matching), Dog with "Bird" label (not matching), Cow with "Cow" label (matching), and Bird with "Dog" label (not matching). When children tap the checkmark for matching pairs or the X for non-matching pairs, "Correct!" appears in green below the buttons. When they tap the wrong button, "Wrong!" appears in red. After tapping either button, the game automatically advances to the next animal after 1 second to keep young children engaged.
