Category: Game

Prompt style: Detailed Specification

Title: Chess Game

Prompt: Create a functional chess game with standard 8x8 board. All pieces move according to official chess rules: Pawns move forward one square (two on first move), capture diagonally, promote to Queen when reaching opposite end. Knights move in L-shape. Bishops move diagonally any distance. Rooks move horizontally/vertically any distance. Queens combine Bishop and Rook movement. Kings move one square in any direction. Implement castling (King moves two squares toward Rook, Rook jumps over). Implement en passant (Pawn captures Pawn that moved two squares). Highlight legal moves when piece is selected. Prevent moves that would put own King in check. Detect check (King under attack) and display warning. Detect checkmate (King in check with no legal moves) and end game. Detect stalemate (no legal moves but not in check) and declare draw. Track captured pieces for both sides. Display move history with algebraic notation. Include Undo button (goes back one full turn). Show whose turn it is. Timer shows elapsed time for each player. Offer Draw button sends draw proposal to opponent. Resign button immediately ends game. After game ends, show winner, total moves, game duration, and option to review move history. Pre-load with standard starting chess position.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| ID | Description | Weight | Rationale | Dependent On |
|----|-------------|--------|-----------|--------------|
| layout-1 | Display 8x8 chess board with alternating colored squares | major | Board establishes playing field | None |
| state-1 | Initialize pieces in standard starting position | major | Starting position defines game opening | layout-1 |
| content-1 | Display all 32 pieces in correct starting locations | major | Piece display shows game state | state-1 |
| interaction-1 | Select piece when clicked | major | Selection initiates move sequence | content-1 |
| visual-1 | Highlight selected piece | major | Highlight confirms selection | interaction-1 |
| state-2 | Calculate legal moves for Pawns (forward 1, or 2 on first move) | major | Pawn movement implements piece rules | interaction-1 |
| state-3 | Calculate legal diagonal captures for Pawns | major | Pawn capture differs from movement | state-2 |
| state-4 | Calculate legal L-shaped moves for Knights | major | Knight movement implements unique jump | interaction-1 |
| state-5 | Calculate legal diagonal moves for Bishops | major | Bishop movement follows diagonal lines | interaction-1 |
| state-6 | Calculate legal horizontal/vertical moves for Rooks | major | Rook movement follows straight lines | interaction-1 |
| state-7 | Calculate legal Queen moves (combine Bishop and Rook) | major | Queen combines two movement patterns | state-5, state-6 |
| state-8 | Calculate legal one-square moves for Kings | major | King has limited movement | interaction-1 |
| visual-2 | Highlight legal move squares when piece is selected | major | Legal move display guides player | state-2 |
| interaction-2 | Move piece to selected legal square when clicked | major | Move execution updates board state | visual-2 |
| state-9 | Implement castling move (King moves 2, Rook jumps over) | major | Castling requires special move logic | state-8 |
| state-10 | Prevent castling if King or Rook has moved previously | major | Castling restrictions enforce rules | state-9 |
| state-11 | Prevent castling if King passes through check | major | Castling safety check enforces rules | state-9 |
| state-12 | Implement en passant capture (Pawn captures Pawn behind) | major | En passant requires special capture logic | state-3 |
| state-13 | Enable en passant only immediately after Pawn moves two squares | major | En passant timing window enforces rules | state-12 |
| state-14 | Promote Pawn to Queen when reaching opposite end | major | Promotion implements piece upgrade | state-2 |
| state-15 | Detect check (King is under attack) | major | Check detection implements threat warning | state-7 |
| visual-3 | Display check warning when King is in check | major | Warning alerts player to danger | state-15 |
| state-16 | Prevent moves that would put own King in check | major | Self-check prevention enforces legal moves | state-15 |
| state-17 | Detect checkmate (King in check with no legal moves) | major | Checkmate detection implements win condition | state-15 |
| interaction-3 | End game and declare winner when checkmate occurs | major | Checkmate triggers game completion | state-17 |
| state-18 | Detect stalemate (no legal moves, not in check) | major | Stalemate detection implements draw condition | state-16 |
| interaction-4 | Declare draw when stalemate occurs | major | Stalemate ends game in tie | state-18 |
| content-2 | Display captured pieces for both sides | major | Capture tracking shows material balance | interaction-2 |
| state-19 | Add captured piece to appropriate side's collection | major | Capture accumulation tracks taken pieces | content-2 |
| content-3 | Display move history in algebraic notation | major | Move history provides game record | None |
| state-20 | Convert each move to algebraic notation format | major | Notation requires position-to-text conversion | content-3 |
| state-21 | Append move to history after execution | major | History accumulation creates game record | state-20 |
| visual-4 | Display Undo button | major | Undo enables move reversal | None |
| interaction-5 | Revert last full turn when Undo is clicked | major | Undo restores previous board state | visual-4 |
| content-4 | Display whose turn it is (White or Black) | major | Turn indicator shows current player | None |
| state-22 | Alternate turn between White and Black after each move | major | Turn tracking manages game flow | content-4 |
| content-5 | Display timer showing elapsed time for each player | major | Timer tracks thinking time | None |
| state-23 | Increment active player's timer while it's their turn | major | Time accumulation measures decision duration | content-5 |
| visual-5 | Display Offer Draw button | major | Draw offer enables tie proposal | None |
| interaction-6 | Send draw proposal when Offer Draw is clicked | major | Draw mechanism allows mutual agreement | visual-5 |
| visual-6 | Display Resign button | major | Resign allows conceding defeat | None |
| interaction-7 | Immediately end game with loss when Resign is clicked | major | Resignation triggers instant defeat | visual-6 |
| interaction-8 | Display results screen after game ends | major | Results show game outcome | interaction-3 |
| content-6 | Display winner on results screen | major | Winner identification shows outcome | interaction-8 |
| content-7 | Display total moves count on results screen | major | Move count quantifies game length | interaction-8 |
| content-8 | Display game duration on results screen | major | Duration shows time investment | interaction-8 |
| visual-7 | Display Review Move History button on results screen | major | Review enables game analysis | interaction-8 |
| interaction-9 | Show full move history when Review is clicked | major | History review provides post-game analysis | visual-7 |
