---
status: pending
title: Tic Tac Toe app (two players, scores, animations and sound)
---

1. **Game logic** – create `src/lib/tictactoe.ts` with winner detection (3 rows, 3 columns, 2 diagonals), returning the winner and the winning line, plus draw detection. Outcome: a pure, reusable helper.
2. **Sound effects** – create `src/lib/sound.ts` using the browser's built-in audio (no files needed) for short tones: place X, place O, win, draw. Include a mute flag stored in local storage. Outcome: sounds play on moves and results, and can be muted.
3. **Board components** – create `src/components/Board.tsx` and `src/components/Square.tsx`. Squares are large, accessible buttons; marks animate in (scale/fade); winning squares are highlighted with a pulse. Outcome: a clean, minimal 3x3 board.
4. **Scoreboard** – create `src/components/Scoreboard.tsx` showing X wins, Draws and O wins, highlighting the current player's turn. Outcome: scores persist across rounds (kept in local storage so refresh doesn't reset).
5. **Game page** – replace the contents of `src/routes/index.tsx` with the game: state for board, current player, scores and result. Include a status line ("X's turn", "O wins!", "Draw"), a "Next round" button (loser/alternating player starts), a "Reset scores" button, and a sound mute toggle. Outcome: fully playable two-player game on one device.
6. **Look and feel** – update `src/routes/__root.tsx` and `src/styles/global.css` (keeping the Tailwind import first) with a minimal light theme: neutral background, centered card, generous spacing, X and O in two distinct accent colors, custom keyframes for mark pop-in and win pulse, responsive down to mobile. Update the page title in `index.html` to "Tic Tac Toe".
7. **Check** – verify a win in each direction, a draw, that clicks on filled squares or after the game ends are ignored, scores update once per round, and mute works.
