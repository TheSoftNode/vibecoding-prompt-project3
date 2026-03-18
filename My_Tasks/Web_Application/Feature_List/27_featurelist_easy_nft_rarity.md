Category: Web_Application

Prompt style: Feature_List

Title: NFT Rarity Score Calculator

Prompt: Build an NFT rarity score calculator. Display input fields for three traits: "Background" (Common/Rare/Legendary), "Eyes" (Common/Rare/Legendary), and "Hat" (Common/Rare/Legendary). Each trait selection should be a dropdown. Display a Calculate button below the inputs. When clicked, calculate rarity score: Common = 1 point, Rare = 3 points, Legendary = 5 points. Sum all trait points and display "Total Rarity: X points" with classification: 3-4 points = "Common NFT", 5-8 points = "Rare NFT", 9+ points = "Legendary NFT".

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display dropdown for Background trait                | major  | The Background dropdown lets users select the first trait rarity.                            | None         |
| 2   | content     | Label Background dropdown                            | minor  | The label identifies this dropdown as the Background trait selector.                         | C1           |
| 3   | content     | Show Common/Rare/Legendary options in Background     | major  | These options provide the rarity choices for the Background trait.                           | C1           |
| 4   | visual      | Display dropdown for Eyes trait                      | major  | The Eyes dropdown lets users select the second trait rarity.                                 | None         |
| 5   | content     | Label Eyes dropdown                                  | minor  | The label identifies this dropdown as the Eyes trait selector.                               | C4           |
| 6   | content     | Show Common/Rare/Legendary options in Eyes           | major  | These options provide the rarity choices for the Eyes trait.                                 | C4           |
| 7   | visual      | Display dropdown for Hat trait                       | major  | The Hat dropdown lets users select the third trait rarity.                                   | None         |
| 8   | content     | Label Hat dropdown                                   | minor  | The label identifies this dropdown as the Hat trait selector.                                | C7           |
| 9   | content     | Show Common/Rare/Legendary options in Hat            | major  | These options provide the rarity choices for the Hat trait.                                  | C7           |
| 10  | visual      | Display Calculate button below inputs                | major  | The Calculate button triggers the rarity score computation.                                  | None         |
| 11  | interaction | Calculate score when Calculate button clicked        | major  | Clicking Calculate computes the total rarity points from selected traits.                    | C10          |
| 12  | state       | Assign 1 point for Common, 3 for Rare, 5 for Legendary| major | Point values determine the numerical score for each trait rarity level.                     | None         |
| 13  | state       | Sum all three trait points                           | major  | Adding trait points gives the total rarity score for the NFT.                                | C12          |
| 14  | content     | Display "Total Rarity: X points" with calculated sum | major  | Showing the total points tells users their NFT's rarity score.                               | C13          |
| 15  | state       | Classify 3-4 points as "Common NFT"                  | major  | Classification helps users understand if their NFT is common tier.                           | C13          |
| 16  | state       | Classify 5-8 points as "Rare NFT"                    | major  | Classification helps users understand if their NFT is rare tier.                             | C13          |
| 17  | state       | Classify 9+ points as "Legendary NFT"                | major  | Classification helps users understand if their NFT is legendary tier.                        | C13          |
| 18  | content     | Display classification text below total              | major  | Showing the classification gives users the tier rating for their NFT.                        | C15, C16, C17|

## Justification

The NFT rarity score calculator works exactly as expected for evaluating trait combinations. Three dropdown inputs display labeled "Background", "Eyes", and "Hat", each showing Common, Rare, and Legendary options. A Calculate button displays below the inputs. When users select traits and click Calculate, the app assigns points (Common = 1, Rare = 3, Legendary = 5) to each trait, sums the three trait points, and displays "Total Rarity: X points". The app then classifies the score as "Common NFT" for 3-4 points, "Rare NFT" for 5-8 points, or "Legendary NFT" for 9+ points, displaying the classification below the total.
