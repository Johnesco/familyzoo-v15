# Family Zoo — v15 — Timed Events (Daemons & Fuses)

The PA system makes scheduled announcements, feeding time arrives on a timer, and goats bleat until fed. Introduces the SchedulerPlugin and its two primitives — daemons that tick every turn and fuses that count down.

Step 15 of the [Family Zoo](https://github.com/Johnesco/familyzoo) tutorial — a progressive walkthrough of the [Sharpee](https://sharpee.net) TypeScript interactive fiction engine, from a single room to a full multi-file story.

## What this step teaches

- SchedulerPlugin registration in onEngineReady
- Daemon interface with condition() and run() that returns events
- Fuse interface with turns, repeat, and originalTurns for re-arming
- game.message events with narrate: true for auto-rendered text
- Gotchas around turn offsets and the fuse skipNextTick behavior

## Playing

Open `play.html`, or preview the folder:

```bash
python -m http.server 8000 --directory familyzoo-v15
```

## Building

This is a **frozen 0.9.x TypeScript version**. The built player in this folder is the published artifact; it is re-laid from `browser/` by the workspace build:

```bash
python ../tools/build.py familyzoo-v15
python C:/code/ifhub/tools/ship.py familyzoo-v15
```

The authoring tree for every version lives in the [familyzoo](https://github.com/Johnesco/familyzoo) repo.
