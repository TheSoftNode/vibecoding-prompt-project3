Category: Game

Prompt style: Casual

Title: Coin Flip Game

Prompt: Coin flip game, super simple. Click Flip button, coin shows either Heads or Tails randomly. Animate the flip with a quick spin. Track streak of same result (like 5 Heads in a row). Show current streak and best streak ever. Reset stats button.

Required libraries: react, tailwindcss, framer-motion

## Rubric

| ID            | Description                                                                 | Weight | Rationale                                                                      | Dependent On |
| ------------- | --------------------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------ | ------------ |
| visual-1      | Display a Flip button                                                       | major  | Flip button triggers coin randomization.                                       | None         |
| interaction-1 | Generate random result of Heads or Tails when Flip is clicked              | major  | Random generation creates unpredictable coin flip outcome.                     | visual-1     |
| content-1     | Display result showing either Heads or Tails                                | major  | Result display shows flip outcome.                                             | interaction-1 |
| visual-2      | Animate coin flip with spinning motion                                      | major  | Spin animation enhances visual feedback and engagement.                        | interaction-1 |
| content-2     | Display current streak count showing consecutive same results               | major  | Current streak tracks ongoing consistency of outcomes.                         | None         |
| state-1       | Increment streak when flip result matches previous result                   | major  | Streak increment requires comparison between current and previous flip.        | content-2    |
| state-2       | Reset streak to 1 when flip result differs from previous result             | major  | Streak reset enforces consecutive requirement for streak counting.             | content-2    |
| content-3     | Display best streak ever achieved                                           | major  | Best streak provides historical peak performance metric.                       | None         |
| state-3       | Update best streak when current streak exceeds previous best               | major  | Best streak update requires comparison between current and maximum values.     | content-3    |
| visual-3      | Display a Reset Stats button                                                | major  | Reset button enables statistics clearing.                                      | None         |
| interaction-2 | Reset current streak and best streak to zero when Reset Stats is clicked   | major  | Stats reset provides fresh start functionality.                                | visual-3     |
