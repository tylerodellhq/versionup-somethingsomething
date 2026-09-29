# Something Something HQ

The Something Something team's Premiere Pro panel. It has two tabs:

**Job**
- **Clockify** times each edit against the right Clockify project and client. Every `_PR` version gets its own entry, so each round of amends shows up separately. The timer stops when you close the project or quit Premiere.
- **Sequences** (Version Up) duplicates a sequence as the next version (`_PR002` → `_PR003`), moves the old one into the **0. Old** bin and records who made it. Undo is one click.
- **Sizes:** the same edit in several aspect ratios (`_9x16`, `_4x5`, `_1x1`, `_16x9`, `_5x4` before `_PR###`) sits on one row. **+ Size** duplicates into another size, scaled from the sequence you're copying (a 2160×3840 edit becomes 3840×2160 at 16x9). **+ New** makes a new sequence named after the project, at the sizes and frame rate you pick, and remembers the sizes for next time.

**Brand**
- All 928 Something Something graphics: scribbles, arrows, circles, lines, bars, frames, corners, bursts, symbols, letters, numbers and the logo.
- Every graphic is available in each brand colour: Carbon, Ivory, Magenta, Cyan or Buttercup. The logo comes in Carbon and Ivory only.
- Search, category filters, ★ favourites and **Copy hex**.
- **Import** (or double-click) saves the PNG in a *Brand assets* folder next to the project, adds it to a *Brand assets* bin and places it at the playhead.

Current version: **2.3.0**. See the [changelog](CHANGELOG.md) for what's new.

## Install

1. Download [SomethingSomethingHQ.ccx](SomethingSomethingHQ.ccx) (click it, then the download button) and double-click it. Creative Cloud installs it.
2. In Premiere: **Window › UXP Plugins › Something Something HQ**.
3. Enter your name when asked. It's shown on the versions you create.
4. Connect Clockify: click **⚙** (top right of the panel) › **Clockify** and paste your personal API key. In Clockify, get it from your profile picture › Preferences › Advanced › Generate. Each editor uses their own key, saved on their own computer only.

Needs Premiere Pro 25.6 or later. Creative Cloud doesn't show the plugin's icon for plugins installed from a .ccx file. That's expected, and the plugin still works.

## Naming

| | Example |
|---|---|
| Project starts with the job code (the letters pick the client) | `EG001_Example` |
| Sequences end with the size, then a version number | `EG001_Example_9x16_PR001` |
| Sequences sit loose in a bin with "Sequences" or "Seqs" in its name | `01_Sequences` |

## Updates

HQ checks this repo for updates. When a new version is out, a banner in the panel offers **Update**, so nobody needs to come back here.

Still on the old *Version Up — Something Something* panel? Click **Update** on its banner and it becomes HQ.

## Clockify safety

HQ only reads from Clockify, creates projects and time entries, and stops your own running timer. It never renames or edits clients, projects or anyone else's entries.

## Releasing (for maintainers)

1. Bump `version` in the plugin's `manifest.json` and build `SomethingSomethingHQ.ccx`.
2. Replace the .ccx here, add a section to `CHANGELOG.md`, and set the same version in `latest.json`.
3. Push to `main`. Panels pick up the new version from `latest.json` the next time they check.

Only people with write access to this repo can publish updates.
