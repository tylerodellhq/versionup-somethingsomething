# Something Something HQ: what's new

## 2.2.1 — 29 Sep 2026
- **+ New** always starts at 30 fps. The suggestion based on your footage is gone. You can still pick another frame rate.

## 2.2.0 — 29 Sep 2026
**Sizes.** The same edit in different aspect ratios now lives on one row.
- Sequences that only differ by their size tag (e.g. `EG001_Example_9x16_PR003` and `EG001_Example_4x5_PR003`) show as one row with a tag for each size. Tap a tag to open that size.
- Older sequences with no size in their name show their size too, worked out from the frame (the name isn't changed).
- **+size** copies the sequence you're working on into other sizes (9x16, 4x5, 1x1, 16x9, 5x4), at the same version. Clips come across centred, so reframe after. If the original has no size in its name yet, HQ adds it from its frame size. No new Clockify entry.
- **Version up** asks "All sizes" or "Just this one" when an edit has more than one size.

**New sequence.** The "Version Up" heading is now **Sequences**, with a **+ New** button.
- Names it after the project, with an optional extra name and the size: `EG001_Test_Project_Cutdown_9x16_PR001`. Odd characters are tidied into underscores.
- Pick one or more sizes and a frame rate (30 fps unless you choose another).
- Goes straight into your Sequences bin.

**Undo** is now a proper button at the bottom. It undoes your last version up, "+ size" or "+ New".

**Tidier Sequences list.** The filter box hides behind a magnifier, the refresh button is gone (the list keeps itself up to date), and the "→ next name" line under each sequence is gone too.

**Brand tab**
- Every time you import, a reminder shows in red along the bottom: *Match the scale and thickness of your other scribbles. One colour on screen at a time. Don't stretch.*
- If you place a scribble on screen at the same time as one in a different colour, the reminder starts with a heads up.

## 2.1.1 — 27 Sep 2026
- **Fixed:** the selected colour on the Brand tab is outlined in Ivory again. Every outline is the same thickness.

## 2.1.0 — 27 Sep 2026
**New: the Brand tab.** HQ now has two tabs: **Job** (Clockify and Version Up) and **Brand**.

- **Every Something Something graphic in one place:** all 928 scribbles, arrows, circles, lines, bars, frames, corners, bursts, symbols, letters, numbers and the logo.
- **Pick a brand colour** (Carbon, Ivory, Magenta, Cyan, Buttercup) and everything shows in that colour. **Copy hex** copies the code, or use Premiere's eyedropper on the swatches.
- **Search** for what you need: "arrow", "star", "heart", "tick", "£", "?", or a single letter or number like "A" or "7".
- **★ Favourites:** tap the star on any asset to keep it handy.
- **Import** puts the asset in your chosen colour into a **Brand assets** bin, and saves the PNG in a **Brand assets** folder next to your project, so it travels with the project on the Drive. If a sequence is open, it's also placed at the playhead on the first free video track above V1. **Double-click** an asset to import it straight away.
- Assets import at 100%, so scribble thickness stays consistent, as the brand guidelines ask.
- The logo only comes in Carbon or Ivory, per the guidelines.
- Remembers your last tab, colour and category.
- Search and **Copy hex** share one row, and the Copy hex button takes on the selected colour.
- Every colour swatch has the same subtle outline, so Carbon shows up on Premiere's dark background.
- A smaller logo and slimmer tabs leave more room for the panel.
- A smaller download: the brand graphics are compressed better, with no change in quality.
- New plugin icon: the Something Something wordmark in Ivory.

**Job tab tweaks**
- Fixed: **"PR003 by <name>"** on version rows wasn't being saved. New versions now record who made them, and the status line says so if Premiere refuses.
- Versioning up while the panel is checking Clockify in the background no longer skips switching the timer to the new version.
- If you stopped your timer in Clockify itself, versioning up won't start it again.
- If your Clockify workspace doesn't let you create projects, HQ now says so, instead of blaming your API key.
- A divider between Clockify and Version Up.
- Sequences that aren't open are slimmer, so the one in your timeline stands out.

When you update, Creative Cloud may ask you to allow two new permissions: saving files (for the Brand assets folder) and the clipboard (for Copy hex).

## 2.0.7 — 27 Sep 2026
- **Clockify** now has its own heading above the timer, matching **Version Up**.
- **A thumbs up when your timer starts**, the same as when you version up, instead of a line of blue text. Versioning up no longer shows "Now timing PR…" either. The strip only shows text when something needs your attention.

## 2.0.6 — 26 Sep 2026
- **Fixed: the settings and refresh icons showed as black blobs** in Premiere. All the panel's icons now display properly.
- **New plugin icon:** the hand-drawn S from the Something Something logo, in Creative Cloud's plugin list and on the panel.
- Tidier About card in Settings.

## 2.0.5 — 26 Sep 2026
- **Exporting no longer stops the timer.** It keeps running until you press Stop, in the panel or in Clockify. Closing the project or quitting Premiere still stops it.
- **Settings cog** in the top right, in place of the **i**. Everything is in one place: your name, **Open new version in timeline** (moved here from the bottom of the panel), your Clockify connection, and an **About** card with the version number, update check and what's new.
- **Slimmer timer** at the top: time, client and version, and Start/Stop. The client picker only appears for a new job that needs one, and says when it's picked the client from the job code (e.g. "from BB").
- **The sequence open in your timeline has a yellow outline**, so the "In timeline now" label is gone.
- **A thumbs up when you version up.** The new version's row lights up blue with 👍 Done, shows the new PR number, then fades back. The bottom of the panel confirms what happened, with **Undo** next to it.
- Refresh is now an icon, and the sequence count sits at the bottom of the panel.

## 2.0.4 — 26 Sep 2026
- **No more stuck "Couldn't reach Clockify" error after sleep.** When your Mac wakes, the internet takes a few seconds to come back. The panel now waits quietly and checks Clockify again a few times, instead of showing a red error that stays on screen.
- Any "can't reach Clockify" message now clears itself once the connection is back, and a project lookup that failed offline fixes itself without pressing Retry.
- Closing a project while offline: the panel says the timer will stop once the connection is back, then stops it at the moment the project closed, not the moment the internet returned.
- Opening Premiere while offline with a timer left running: once online, the timer is stopped at the moment Premiere was last open.

## 2.0.3 — 26 Sep 2026
- **Fixed: the panel didn't see a timer already running in Clockify**, so pressing Start replaced it. The panel now always gets a fresh answer from Clockify instead of reusing an old one. Open a project whose timer is already running and the panel picks it up as that project's timer, with Stop ready.
- Checks all of your Clockify workspaces for a running timer, not just the one the panel uses. A timer in another workspace is shown with its workspace name.
- The ⚙ Clockify settings now show exactly what's running in Clockify, which helps if anything looks wrong.

## 2.0.2 — 26 Sep 2026
- **Stays in step with Clockify.** When Premiere opens, and every 30 seconds after, the panel checks what's actually running in your Clockify account. A timer left running, or started in the browser, shows up in the panel so you can see it and stop it. Stop one in the browser and the panel clears.
- **Closing a project stops the timer reliably.** Previously, if the stop request to Clockify didn't get through, the panel forgot about the timer while it carried on running in Clockify. Now it holds on until Clockify confirms, and keeps retrying. The timer ends at the moment you closed the project.
- **Premiere quit while timing:** next time it opens, the timer is stopped at the moment Premiere was last open.
- A timer that's running for something else (not the open project) is shown but never stopped automatically, only when you press Stop. If it's for the project you then open, it's treated as that project's timer.
- Tidier timer strip: Start and Stop now look exactly like the **Version up** buttons, and the **i** button sits at the top right next to the logo.

## 2.0.1 — 26 Sep 2026
- Test update to check the in-panel update banner. Nothing else has changed.

## 2.0.0 — 25 Sep 2026
Version Up is now **Something Something HQ**, with Clockify built in. Everything in Version Up works as before, and your name and settings carry over.

- **Timer strip** at the top of the panel: what you're timing, how long, and one Start/Stop button.
- **Start** takes the Premiere project name and finds the Clockify project with that exact name. If there isn't one yet, it creates it under the client you choose, then starts the timer.
- **Clients by job code.** The client list comes straight from Clockify. Once you've used a code with a client (BB014 → Beyond Boundaries), the next BB project picks that client for you. It only auto-picks when that code has only ever been used with that one client; otherwise you choose.
- **Version up = new entry.** Each version up closes the current Clockify entry and starts a new one named after the version (PR002, PR003 …), so time on each round of amends is tracked separately. If the edit is already in Clockify and you weren't timing, versioning up starts the timer.
- **Stops by itself** when an export finishes (from Premiere or Media Encoder), when you close or switch project, and if Premiere quits or crashes while timing (next time it opens, the timer is stopped at the moment Premiere was last open).
- **Leaves Clockify alone otherwise.** It only creates projects and time entries and stops its own timer. It never renames or changes clients, projects or anyone else's entries. If a different timer is already running, it asks before stopping it.

## 1.9.0 — 25 Sep 2026
- **Undo button.** After you version up, an **Undo PR003** button appears at the bottom of the panel. One click removes the new version and moves the previous one back out of the Old bin. If you've already made changes in the new version, it asks before deleting them.

## 1.8.3 — 25 Sep 2026
- **Check for updates** button in the **i** pop-up. It shows whether you're up to date, offers **Update now** if a new version is out, or says why it couldn't check.

## 1.8.2 — 25 Sep 2026
- Checks for updates once each time Premiere opens. If you're offline at the time, it keeps trying every few minutes until it gets through.

## 1.8.0 — 25 Sep 2026
- **Automatic update notices.** When a new version is out, a banner appears in the panel — click **Update** and Creative Cloud installs it. No more sending files around.

## 1.7.0 — 25 Sep 2026
- The first time the panel opens, it asks for your name.
- New versions are stamped with who made them and when, e.g. `PR003 by Tyler · 25 Sep`. This is saved in the project, so it's still there when someone else opens it from the shared drive.
- The **i** button opens a pop-up with the version number and your name.

## 1.6.0 — 25 Sep 2026
- Tidier title bar; version number moved behind the **i** button.
- Rounded **Version up** buttons.

## 1.5.0 — 25 Sep 2026
- First Something Something edition: logo and brand colours.

## 1.4.0 — 25 Sep 2026
- List sorted by what you're working on: the sequence in your timeline first, then the most recently edited, then the rest A–Z.
- The list scrolls, and there's a filter box to find a sequence by name.

## 1.3.0 — 25 Sep 2026
- Finds your sequences bin by name — `01_Sequences`, `SEQUENCES`, `Seqs` and so on all work.

## 1.1.0 — 25 Sep 2026
- Finds the Old bin however it's named — `0. Old`, `OLD`, `_old` and so on.

## 1.0.0 — 25 Sep 2026
- First release: one click duplicates a sequence, gives it the next `_PR` number and moves the previous version into the Old bin.
