# The Chemistry Teacher

A single-file, Sierra-style graphical adventure inspired by the premise of
*Breaking Bad* Season 1. You walk Walter White through painted VGA-era rooms:
diagnosed, broke, and about to make a series of very bad decisions — or not.
Up to you.

## Play

Open `index.html` in any modern browser. That's it — no install, no build,
no network. It works on phones.

**Controls**

- **Arrow keys / WASD** — walk
- **Enter / Space** — advance text, interact with the highlighted hotspot
- **Click / tap** — walk somewhere, or straight to a hotspot
- **Esc** — save/load
- On touch screens an on-screen D-pad and action button appear

After each scene's narration, your choices appear in the room as glowing
markers, characters, and doors. Walk up to one — the status line at the
bottom shows what it means — and press Enter to commit.

## Features

- 5 chapters, ~75 scenes, 6 distinct endings shaped by your choices
- 12 hand-painted rooms (all art drawn in code — no image files) with
  procedural pixel-art characters; Walt's sprite changes with the story
- Four stats — **Money**, **Heat**, **Family**, **Health** — that gate
  choices and trigger story interrupts at critical thresholds
- Inventory items that unlock options; 8 random events between chapters
- Relationship tracking for Skyler, Jesse, Hank, Marie, Walt Jr., Saul, and Tuco
- Save/load via a copyable save code (no localStorage, no cookies)

## Adding content

All story content lives in `SECTION 1: DATA` inside `index.html` — scenes,
choices, conditions, effects, items, events, rooms, and staging are plain
data objects. The engine (`SECTION 2`) doesn't need changes to add chapters;
new scenes only need a `STAGES` entry (room + hotspot positions) to appear
on screen.

Content note: everything related to "the cook" is deliberately an abstract,
narrative-only black box, and must stay that way in any added scenes.
