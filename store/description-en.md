# Checkers AI — Store Submission Materials

## Short description (CrazyGames / GameDistribution / itch.io)

Classic English checkers (draughts) against a real minimax AI. Forced
jumps, branching multi-jump chains, crowning kings. Three difficulty levels
on a handcrafted wood board. Can you out-think the machine?

(186 characters)

## Details

- Genre: Board game / Strategy / Casual / Classic
- Controls: Mouse / Touch — tap a piece, then tap a highlighted square to
  move; multi-jumps prompt you hop by hop. Keyboard: arrows move the
  cursor, Enter/Space selects and moves, Esc deselects.
- Rules: Standard English draughts — you play red and move first; men step
  diagonally forward; jumps are mandatory and chains must run to completion
  (you pick the path at forks); crowning ends the move; kings move and jump
  in all four diagonal directions; a side with no legal move loses; 40
  quiet king moves per side or a threefold repetition is a draw.
- AI: Easy (depth-2 search, 25% random moves), Normal (depth 5), Hard
  (depth 7) — negamax with alpha-beta pruning, capture extension, move
  ordering and iterative deepening with a hard time cutoff, so every move
  is ≤ 1.5 seconds. Evaluation: piece count, king bonus, advancement /
  center position tables and edge safety.
- Features: Sliding piece animation with tumbled flying captures, crown
  markers, last-move highlight, forced-capture indicators, dashed jump-path
  preview, KING! effects, per-difficulty W/L/D records saved locally, mute
  toggle, responsive canvas for portrait and landscape.
- Tech: Vanilla JavaScript, Canvas, WebAudio (all sounds synthesized).
  Single-file HTML5, no external assets, works offline once loaded.
  No frameworks, no tracking, no external links.

## Tags
checkers, draughts, board game, strategy, ai, minimax, classic, casual, abstract, single-file

## CrazyGames submission checklist
- [x] Self-contained index.html (SDK loads only on crazygames domains)
- [x] gameplayStart / gameplayStop / loadingStart / loadingStop / happytime events wired
- [x] Responsive (canvas scales to any screen, portrait-friendly, mouse/touch/keyboard)
- [x] No external links inside gameplay, no analytics
- [ ] Cover: TBD (1280x720)
- [ ] Screenshots: TBD

## GameDistribution
- Upload checkers-ai-gd.zip (contains index.html only), kind: html

## itch.io
- Upload zip (checkers-ai-itch.zip), mark "This file is playable in browser",
  entry file: index.html, viewport 480x480 (responsive), kind: html
- Pricing: $0 (donations optional)
