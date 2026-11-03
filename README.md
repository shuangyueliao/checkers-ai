# Checkers AI · English Draughts vs Minimax

Free single-file HTML5 board game. Classic English draughts (8x8, dark
squares) against a real minimax alpha-beta AI — three difficulty levels
(Easy / Normal / Hard), Hard running iterative-deepening search with capture
extension, always under 1.5 seconds per move. Mandatory jumps, branching
multi-jump chains with dashed path previews, kings with crown markers,
sliding move animations with tumbled captured pieces, procedural wood board,
WebAudio synthesized sounds and per-difficulty win/loss/draw records. One
HTML file, zero external assets.

**Play:** https://shuangyueliao.github.io/checkers-ai/

- Mouse / touch / arrow keys, procedural canvas graphics, no dependencies
- Rules: men move diagonally forward, jumps are forced and chains must run
  to completion, crowning ends the move, kings move and jump both ways,
  no legal move loses, 40 quiet king moves each side or threefold
  repetition draws
- AI: Easy (depth 2 + 25% random), Normal (depth 5), Hard (depth 7),
  evaluation = material + king bonus + position tables + edge safety

## Run

Open `index.html` in any modern browser, or serve the folder statically.
Everything (graphics, sounds, AI) is generated locally — no network needed
except the optional portal SDK, which loads only on crazygames /
gamedistribution / gd.games domains.

## Files

- `index.html` — the entire game (≈43 KB, self-contained)
- `.nojekyll` — disables GitHub Pages Jekyll processing
- `store/` — submission materials (description + distributable zips)
