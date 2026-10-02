---
title: Better Preview
---


A keyboard-driven photo culling app for macOS. Point it at the folder your trips live in,
make one decision per photo, and end up with a portfolio in the order you want it seen.

**Contact: maxbogdanoff@gmail.com** — questions, bugs and feature requests all welcome.
Please include your macOS version and the app version (Better Preview ▸ About).

---

## Getting started

1. **Open a folder.** `⌘O`, or drag a folder from Finder onto the window. Choose the folder
   that *holds* your trips, not a single trip — each subfolder shows up in the sidebar.
2. **Pick a trip** in the sidebar, then press `Return` to go to single-photo view.
3. **Press `S`** to pick a photo, or `→` to skip it. Work through the trip.
4. **Open Picks** in the sidebar once a few trips are done. It holds every pick from every
   trip. Press `S` again to promote the best to Shortlist, then Shortlist to Portfolio.
5. **Open Portfolio** in grid view and drag the photos into order.
6. **Export ▸ Copy Portfolio to Folder…** writes them out numbered in that order.

## Keyboard

| Key | What it does |
|---|---|
| `S` (or `Space` in single view) | Promote one rung: undecided → pick → shortlist → portfolio |
| `D` | Demote one rung |
| `X` | Reject (press again in the grid to un-reject) |
| `U` | Clear the decision |
| `←` `→` | Previous / next photo — `→` is how you skip |
| `↑` `↓` | Move a whole row in the grid |
| `Space` in the grid | Quick Look, exactly like Finder |
| `Return` | Switch between grid and single view |
| `Escape` | Back to the grid |
| `⌘O` | Open folder |
| `⇧⌘P` `⇧⌘L` `⇧⌘K` | Jump to Portfolio / Shortlist / Picks |
| `⌘⌥1`–`4` | Decision filter: All / Undecided / Picked / Rejected |
| `⌘⌥0` | Clear the filter bar |
| `⌥⌘I` | Show or hide the preview pane |
| `⌘A` / `⌘D` | Select all / deselect all |
| `⇧⌘H` | Show hidden folders |

In the grid these keys act on the whole selection at once.

---

## Common questions

**Where are my decisions stored?**
In a hidden file called `.betterpreview.json`, in the folder you opened. Move the folder and
your decisions move with it. Back it up and they are backed up. Delete it and every decision
is cleared — your photos are not touched.

**Does it change my photos?**
No. Image files are never modified or re-encoded. Files move only when you choose one of the
two Export commands, and both report what they did.

**I opened a folder and it says "No Photos".**
You probably opened a folder that only contains other folders. That is the intended way to
use the app — click one of the trips in the sidebar to see its photos.

**Can I undo a decision?**
Press `D` to demote one rung, or `U` to clear the decision entirely. Decisions are not
destructive, so there is nothing to recover.

**The portfolio will not let me drag photos into order.**
Dragging is only allowed when the filter bar is cleared (`⌘⌥0`). Reordering a filtered list
would renumber photos you cannot see.

**Which formats are supported?**
JPEG, HEIC, PNG, TIFF, and camera RAW: CR2, CR3, NEF, ARW, RAF, RW2, ORF, DNG, PEF, SRW and
others macOS can decode.

**I shoot RAW + JPEG and see everything twice.**
Open the **Type** menu in the filter bar and choose **RAW Only** or **JPEG Only**. It hides
one half of every matched pair and leaves unpaired files alone.

**A trip I am done with is cluttering the sidebar.**
Right-click it and choose **Hide Folder**, or select it and press Delete. Nothing on disk
changes. **View ▸ Show Hidden Folders** (`⇧⌘H`) brings them back, dimmed, so you can unhide.

**Why does it need access to my folders?**
To list and display the photos, and to write the decisions file next to them. The app is
sandboxed and can only reach folders you hand it yourself. It has no network access at all.

## Requirements

macOS 15 or later. Apple silicon and Intel.
