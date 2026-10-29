# MCM Remembers Last Tab + Custom Mod Categories Compatibility Patch

### Requirements
- [Mod Configuration Menu - ravenascendant](https://www.moddb.com/mods/stalker-anomaly/addons/anomaly-mod-configuration-menu)
- [Custom Mod Categories - elseform](https://github.com/elseform/anomaly-mods/tree/release/Custom%20Mod%20Categories)
- [MCM Remembers Last Tab v1.2 - turretrider](https://www.moddb.com/mods/stalker-anomaly/addons/mcm-remembers-last-tab)

### Installation:

Install the ZIP from releases as a separate mod in MO2. 

Enable this mod below both originals in Mod Organizer,
<br />It has to have priority over the scripts from turretrider.

#### What it does?
Adds Custom Mod Category compatibility into MCM Remembers Last Tab scripts.

#### Changes:
- Live search respects CMC's search suppression, and queues tree rebuilds through CMC's next-frame refresh.
- Apply saves the current page and reopens it on the next UI frame, replacing CMC's return to the category overview.
- Restart-required settings retain the original close/restart flow. 
- Search is cleared when reopening; ordinary category-list scrolling is restored when the category still matches.
- Remembers the category overview separately from a settings page, so stale last_path values do not reopen the wrong page.
- Scroll offsets are restored only when the category and page match. 
- Search text is not persisted; search-result offsets are discarded because reopening uses the normal category list.
- The right-hand settings pane scroll is saved separately and restored after Apply and reopening the same page, including when its category has changed.
- All Mods stays selected after Apply and reopening. 
- Saved category browsing is preserved when the selected mod still belongs to that list; otherwise its current category is used.
- Removed categories fall back to the category overview. Reassigned pages use their current category.
- Existing Enable and Remember Scroll settings remain available. The legacy page is imported on first use without its unqualified scroll offset.

<br />

---
This software is provided "as is", without warranty of any kind. 
<br />  It is free to use, modify, and distribute under one condition: 
<br />  You must credit the author (SavageBulldog) and include a link back to the original repository.
```
https://github.com/SBDG-0/crispy_stalker_anomaly
```
---
made with ❤️ by SavageBulldogOG
