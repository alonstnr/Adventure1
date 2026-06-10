# The Chemistry Teacher

A single-file, browser-based branching adventure inspired by the premise of
*Breaking Bad* Season 1. You are Walter White: diagnosed, broke, and about to
make a series of very bad decisions — or not. Up to you.

## Play

Open `index.html` in any modern browser. That's it — no install, no build,
no network. It works on phones.

## Features

- 5 chapters, ~75 scenes, 6 distinct endings shaped by your choices
- Four stats to manage — **Money**, **Heat**, **Family**, **Health** — that
  gate choices and trigger story interrupts at critical thresholds
- Inventory items that unlock options; 8 random events between chapters
- Relationship tracking for Skyler, Jesse, Hank, Marie, Walt Jr., Saul, and Tuco
- Save/load via a copyable save code (no localStorage, no cookies)

## Adding content

All story content lives in `SECTION 1: DATA` inside `index.html` — scenes,
choices, conditions, effects, items, and events are plain data objects. The
engine (`SECTION 2`) doesn't need changes to add chapters.

Content note: everything related to "the cook" is deliberately an abstract,
narrative-only black box, and must stay that way in any added scenes.
