Category: Game

Prompt style: Feature_List

Title: Slot Aligner

Prompt: Build a slot machine alignment game with these features: Display three vertical slot reels side by side, each showing a single symbol from the set: "🍒", "🍋", "🍊", "⭐", "💎". Display a "Spin" button below the reels. When players click "Spin", all three reels spin by rapidly cycling through random symbols for 2 seconds, then each reel stops one at a time from left to right with 0.3 seconds between stops. Display a result label showing "Spinning..." while reels are moving. When all reels stop, check if all three symbols match. If all three match, display "JACKPOT!" in gold text. If any symbols don't match, display "No Match" in gray text.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display three vertical slot reels side by side       | major  | The reels provide the slot machine visual interface.                                         | None         |
| 2   | content     | Show single symbol on each reel from symbol set      | major  | Symbols from the set create the matching challenge.                                          | C1           |
| 3   | visual      | Display "Spin" button below reels                    | major  | The button gives players control to trigger the slot spin.                                   | None         |
| 4   | interaction | Spin all reels when button clicked                   | major  | Spinning creates the randomization mechanic.                                                 | C3           |
| 5   | state       | Cycle through random symbols rapidly for 2 seconds   | major  | The 2-second spin creates suspense and visual effect.                                        | C4           |
| 6   | state       | Stop each reel from left to right with 0.3s gaps     | major  | Sequential stopping creates the slot machine timing pattern.                                 | C5           |
| 7   | content     | Display "Spinning..." label while reels move         | major  | The label tells players the reels are currently spinning.                                    | C4           |
| 8   | state       | Check if all three symbols match when stopped        | major  | Checking match determines if the player won.                                                 | C6           |
| 9   | content     | Display "JACKPOT!" in gold when all match            | major  | Gold jackpot message celebrates a winning combination.                                       | C8           |
| 10  | content     | Display "No Match" in gray when symbols differ       | major  | Gray message indicates no winning combination.                                               | C8           |
| 11  | content     | Display score counter labeled "Score: 0" at top      | major  | The counter shows total accumulated points.                                                  | None         |
| 12  | state       | Add 10 points to score on jackpot                    | major  | Adding points rewards matching symbols.                                                      | C8           |
| 13  | state       | Add 0 points to score on no match                    | major  | No points added prevents rewarding non-matches.                                              | C8           |
| 14  | content     | Update displayed score after each spin               | major  | Updating display shows the current total score.                                              | C12, C13     |

## Justification

The slot aligner game works exactly as expected for slot machine matching. Three vertical slot reels display side by side, each showing a single symbol. A "Spin" button displays below the reels. A score counter labeled "Score: 0" displays at the top. When players click "Spin", all three reels spin by rapidly cycling through random symbols for 2 seconds. A result label displays "Spinning..." while reels move. Each reel stops one at a time from left to right with 0.3 seconds between stops. When all reels stop, the game checks if all three symbols match. If all three match, "JACKPOT!" displays in gold text and 10 points are added to the score. If any symbols don't match, "No Match" displays in gray text and 0 points are added. The score counter updates to show the accumulated total.
