# Emberfall Chronicles — playable web build

🎮 **Play:** https://mobiclawtest-cell.github.io/

This repository hosts the compiled, playable build of **Emberfall Chronicles**, a retro 16-bit
top-down action-RPG designed for phones in portrait.

## Controls
- **D-pad** (left) — move, 8-way
- **A** — sword attack (3-hit combo) / place block
- **B** — dodge roll / hold to charge bow
- **X** — use quick item / place block
- **Y** — interact / hold to block
- **INV · MAP · JRNL · ⏸** — top-right small buttons

Keyboard fallback: WASD/arrows to move, **J** attack, **K** dodge, **L** item, **I** interact, **Esc** pause.

## How this repo works
`.github/workflows/deploy-game.yml` pulls the latest compiled build from the source repository
(`mobiclawtest-cell/emberfall-public`, branch `gh-pages`) and commits it here on every push,
on manual dispatch, and nightly at 04:00 UTC. GitHub Pages serves this repository's `main`
branch automatically as a user site.

## Source code
Full TypeScript source, engine, world generator, and build pipeline:
https://github.com/mobiclawtest-cell/emberfall-public
