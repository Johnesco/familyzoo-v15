# v15 — Scoring & Endgame

Points for seeing the zoo. `use scoring` turns on the SCORE command, rooms carry what a visit is worth, and `award` banks it once.

## What this step adds

- `use scoring` in the story header
- `score visit worth 5` on a room
- `award visit` inside `after the player entering`
- Why awarding is idempotent — revisiting pays nothing
- The SCORE command, for free

## The source

The whole step is one file: [`familyzoo-v15.story`](../familyzoo-v15.story). Read it top to bottom — it is the previous step plus what is listed above.

## Running it

```bash
npx sharpee play
npx sharpee test          # replays familyzoo-v15.tests.json
```

Chord language reference: <https://sharpee.net/chord/>
