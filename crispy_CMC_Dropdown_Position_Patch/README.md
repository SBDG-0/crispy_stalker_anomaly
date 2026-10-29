# Custom Mod Categories Dropdown Position Patch

### Requirements
- [Mod Configuration Menu - ravenascendant](https://www.moddb.com/mods/stalker-anomaly/addons/anomaly-mod-configuration-menu)
- [Custom Mod Categories - elseform](https://github.com/elseform/anomaly-mods/tree/release/Custom%20Mod%20Categories)

<br />

No original mod files are changed by this patch.

The script wraps CMC's existing layout method.

English/Russian string tables are supplied.

### Installation:
Install the ZIP from releases as a separate mod in MO2. 

Enable alongside CMC in Mod Organizer

#### What it does?
Adds the ability to reposition the dropdownlist on the mcm/settings page.

#### Changes:
- Adjust Horizontal offset and Vertical offset on this patch's MCM page, then Apply.
- Both use negative for left/up, positive for right/down and zero for native placement.
- Default slider ranges cover the entire normalized Anomaly UI canvas: X -1024..1024; Y -768..768. 
- These UI coordinates apply to both 16:9 and 21:9. 
- The actual allowed motion is calculated from the parent dialog's width/height and the full control group's dimensions, leaving a four-unit margin inside the window. 
- Controls remain inside their clickable parent frame. 
- Moving beyond that limit leaves the group at the window frame edge, so the slider number is the requested offset rather than necessarily the effective offset.
- Offsets are always relative to each layout's native geometry and never accumulate.
- CMC moves dropdowns and their labels together, including headers with both category and preset selectors.

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
