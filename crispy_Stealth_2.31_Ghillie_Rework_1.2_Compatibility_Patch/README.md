# Stealth + Ghillie Rework Compatibility Patch

### Requirements
- [Stealth 2.31 - bvcx](https://www.moddb.com/mods/stalker-anomaly/addons/stealth1)
- [Ghillie Rework 1.2 - jaggervorog](https://www.moddb.com/mods/stalker-anomaly/addons/ghillie-rework)


### Installation:
Install the ZIP from releases as a separate mod in MO2. 

Enable it and give it HIGHER file priority (larger Priority number) than Stealth, Ghillie Rework and the old Ghillie-Stealth patch. 

The old compatibility patch can be disabled.

#### Changes:
- Keeps Stealth 2.31 lighting/weather, entity-specific campfire illumination, target-specific weight/crouch handling,<br /> observer NVG contribution, memory, muzzle handling, HUD and debug code. 
- Keeps the original game-version guard around NPC muzzle callbacks; does not force 1.5.2-only hooks onto 1.5.3.

- Adds Ghillie 1.2 slot-13 ghillie_outfit detection, terrain matching (earth/dirt/grass/bush), <br />visibility and firing-alert MCM settings, its 10-distance threshold, distance curve, <br />crouch influence and 3-second unsuppressed-shot alert. 
- Alert is extended by every qualifying shot. Ghillie's extra crouch multiplier is intentionally retained.
- Camouflage policy: use the Ghillie formula when equipped on qualifying terrain, <br />otherwise retain Stealth's original stationary outfit camouflage. 
- This fallback combines the systems; it differs from the old Ghillie patch, which discarded native outfit camouflage entirely.
- Equipment refresh works without an outfit and does not depend on the triggering item being an outfit. 
- Terrain is unknown after loading until the first footstep reports a material; no terrain bonus is granted before then. 
- Firing-alert state resets on load.

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
