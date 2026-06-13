# Mixed Fest '26 — Race Control

Static site and tools for the **BHHHC Mixed Festival 2026** — 19–21 June 2026, The Cow's Roast, near Berkhamsted. 7-a-side mixed hockey on grass and astro, Wild West / Junetoberfest theme.

**Live site:** `https://<your-username>.github.io/<repo>/`

## What's in here

- **`index.html`** — the hub page. Links the three tools below.
- **`mixed_fest_announcer.html`** — the Dispatch Desk: an auto foghorn and Wild West announcer that runs the whole day's timing (matches, breaks, Beer Race, Big Finale) so you don't need an MC.
- **`handout_pack.html`** — rules, housekeeping, camping zones and timings for captains.

## Running the announcer on the day

1. Open `mixed_fest_announcer.html` in Chrome on the laptop wired into the PA.
2. Click **Go on air** once (this unlocks the sound), then hit **Test foghorn** and **Test voice** through the speakers.
3. The 2026 schedule is built in. Check it under **Schedule — paste from Tournify**; **Restore 2026 schedule** brings it back if you change anything.
4. When registration's done, click **Start the day**. It runs itself from there. Nudge it with **Pause** or **±30s** if the day drifts (e.g. around the long lunch).

Keep the laptop **awake and plugged in**, and keep a copy of the file saved locally as an offline backup in case signal drops.

## Updating the schedule (e.g. next year)

Export the match schedule from Tournify (Excel), then in the announcer open the **Schedule** panel and enter one fixture per line:

```
time, field, team A, team B, umpire
```

Lines sharing a time become one round. Add a 6th value for a longer match (e.g. the finale `16:15, Grass 2, 1st A, 1st B, Committee, 50`). Start a line with `!` for an event, e.g. `12:15, ! Beer Race, 50`. Click **Load this schedule**.

## A note on privacy

This repo is **public** so GitHub Pages can host it for free. Don't commit anything containing personal data — registration responses, phone numbers or email addresses. The announcer stores its schedule and settings in the browser, not in the repo, so nothing sensitive ends up here.

---

Babs · Hunt · Clare · Becca · Kate — mixedfestival@berkohockeyclub.com
