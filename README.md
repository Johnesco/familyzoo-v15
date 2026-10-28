# Family Zoo — v15: Scoring & Endgame

Points for seeing the zoo. `use scoring` turns on the SCORE command, rooms carry what a visit is worth, and `award` banks it once.

Step 15 of sixteen in the [Family Zoo](https://github.com/Johnesco/familyzoo) tutorial for [Chord](https://sharpee.net/chord/), the authoring language of the [Sharpee](https://sharpee.net) interactive fiction engine.

## What this step adds

- `use scoring` in the story header
- `score visit worth 5` on a room
- `award visit` inside `after the player entering`
- Why awarding is idempotent — revisiting pays nothing
- The SCORE command, for free

## The source

The whole step is one file: [`familyzoo-v15.story`](./familyzoo-v15.story) — the step before it plus the ideas above. Where it sits in the trail is on the [group page](https://johnesco.github.io/familyzoo/#familyzoo-v15).

## Playing and testing

```bash
npx sharpee play
npx sharpee test          # replays familyzoo-v15.tests/
python ../tools/build.py familyzoo-v15 --force
```

## Engine

Pinned in `package.json`, held across the whole `@sharpee/*` scope by an `overrides` block.

The 0.9.x TypeScript edition this replaced is kept in [`legacy/`](./legacy).
