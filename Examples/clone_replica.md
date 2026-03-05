# Clone/Replica

### Wordle Clone

## Prompt

Create a clone of Wordle. Use a fixed 5-letter target word stored in code. The player should have up to six guesses displayed in a visible 6x5 grid. After each guess, provide letter feedback with three states: green for correct position, yellow for correct letter in the wrong position, and gray for letters not in the word. Include a visible on-screen keyboard that updates letter colors based on guess results.

## Rubric

| ID            | Description                                                                                                      | Weight | Rationale                                      | Dependent On |
| ------------- | ---------------------------------------------------------------------------------------------------------------- | ------ | ---------------------------------------------- | ------------ |
| visual-1      | Render a visible 6×5 grid on initial page load                                                                   | major  | Grid structure defines gameplay.               | None         |
| layout-1      | Position on-screen keyboard below or beside the grid                                                             | major  | Keyboard is required for input.                | None         |
| interaction-1 | Allow the user to enter letters using the on-screen keyboard                                                     | major  | User interaction drives gameplay.              | None         |
| state-1       | Store a fixed 5-letter target word in code                                                                       | major  | Target word is required to evaluate guesses.   | None         |
| state-2       | Evaluate each guess and assign each letter one of three states: correct position, wrong position, or not in word | major  | Core game mechanic depends on this logic.      | state-1      |
| visual-2      | Apply distinct visual styles to grid cells reflecting the letter state                                           | major  | Feedback must be visually distinguishable.     | state-2      |
| state-3       | Update keyboard key styling to reflect evaluated letter states                                                   | major  | Keyboard must stay synchronized with feedback. | state-2      |
| content-1     | Prevent more than six guesses from being entered                                                                 | major  | Guess limit is part of game rules.             | None         |
| content-2     | Display a visible win or loss message when the game ends                                                         | minor  | Clear termination state improves completeness. | state-2      |
