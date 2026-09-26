# Something Something HQ: what's new

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
