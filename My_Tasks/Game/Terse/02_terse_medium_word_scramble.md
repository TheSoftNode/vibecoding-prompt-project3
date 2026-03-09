Category: Game

Prompt style: Terse

Title: Word Scramble Game

Prompt: Word scramble game with 10 preset words. Display scrambled letters with input and Submit button. Show "Correct!" in green or "Wrong!" in red below input. Award 10 points for correct, 5 bonus if under 10 seconds. Timer at top-right counts up from 0, score at top-left. Skip button loads next word. After all 10 words, show results screen with final score and time breakdown per word. Highlight fastest solve in gold. Restart button reshuffles words. On initial load, show first scrambled word, timer at 0, score at 0.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                                                 | Weight | Rationale                                                                      | Dependent On |
| --- | ----------- | --------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| 1   | content     | Display scrambled letters with input field and Submit button                | major  | Scrambled letters present the puzzle while input and button enable submission. | None         |
| 2   | interaction | Show "Correct!" in green below input when guess matches word, or "Wrong!" in red when it doesn't | major  | Immediate colored feedback confirms whether the answer was right or wrong.     | C1           |
| 3   | layout      | Position timer counting up from 0 at top-right and score at top-left        | major  | Top corner positioning keeps key metrics visible during gameplay.              | None         |
| 4   | state       | Calculate and display score as 10 points per correct answer plus 5 bonus for answers under 10 seconds | major  | Score combines base points with time-based bonuses requiring conditional logic. | None         |
| 5   | state       | Increment timer by 1 second every second and stop when Submit is clicked    | major  | Timer evolves continuously and captures solve duration at submission.          | C3           |
| 6   | interaction | Load next scrambled word when Skip button is clicked                        | major  | Skip lets players move forward when stuck on a word.                           | C1           |
| 7   | state       | Reset timer to 0 when next word is loaded                                   | major  | Timer reset ensures each word starts with clean time tracking.                 | C6           |
| 8   | interaction | Display results screen showing final score and time breakdown per word after all 10 words complete | major  | Results screen transitions to completion and shows performance details.        | None         |
| 9   | content     | Display time breakdown showing solve time for each of the 10 words on results screen | major  | Per-word timing provides detailed performance breakdown.                       | C8           |
| 10  | visual      | Highlight the fastest solve time in gold on the results screen              | major  | Gold highlighting draws attention to the best individual performance.          | C9           |
| 11  | state       | Identify fastest time by finding minimum value across all 10 solve times    | major  | Finding minimum requires comparison across all recorded times.                 | C10          |
| 12  | interaction | Reset game with reshuffled words when Restart button is clicked             | major  | Restart creates new game with randomized word order for replayability.         | C8           |
