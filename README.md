# phobgcc - quick reference

> **Note**
> This site is neither officially affiliated with nor has been endorsed by the PhobGCC developer team. Its purpose is to be a personal quick-reference guide. I have decided to make it publically available, however there is **no guarantee** of completeness, correctness or being up-to-date. The author claims no responsibility for anyone using any of the information below.

## Latest Software Versions
* **For V1 Boards**: [https://github.com/PhobGCC/PhobGCC-SW/archive/refs/tags/v0.28.zip](https://github.com/PhobGCC/PhobGCC-SW/archive/refs/tags/v0.28.zip)
* **For V2 Boards**: [https://github.com/PhobGCC/PhobGCC-SW/releases/download/v0.28/phobgcc_rp2040_v0.28.uf2](https://github.com/PhobGCC/PhobGCC-SW/releases/download/v0.28/phobgcc_rp2040_v0.28.uf2)

## User Guides

* **Programming Guide for V1 Boards** (updating software): [https://github.com/PhobGCC/PhobGCC-doc/blob/main/For_Users/Phob_Programming_Guide.md](https://github.com/PhobGCC/PhobGCC-doc/blob/main/For_Users/Phob_Programming_Guide.md)
* **Programming Guide for V2 Boards** (updating software): [https://github.com/PhobGCC/PhobGCC-doc/blob/main/For_Users/Phob2_Programming_Guide.md](https://github.com/PhobGCC/PhobGCC-doc/blob/main/For_Users/Phob2_Programming_Guide.md)
* **Calibration & Configuration Guide**: [https://github.com/PhobGCC/PhobGCC-doc/blob/main/For_Users/Phob_Calibration_Guide_v0.28.md](https://github.com/PhobGCC/PhobGCC-doc/blob/main/For_Users/Phob_Calibration_Guide_v0.28.md)

## Tips

### Use Springless Triggers With Smash Ultimate


Smash Ultimate ignores digital trigger press. Analog trigger value of ≥ 79 is required to activate shield. To achieve this on triggers with springs removed:
1. Switch trigger mode to 5 or 6 (AB+L or AB+R)
2. If using SmashScope - adjust (increase) the value until analog value is ≥ 79; if connected to Switch, adjust (increase) the value until pressing the trigger results in Shield (LB+Du/Dd or RB+Du/Dd). 

### Adjusting Analog Diagonals Values


By default diagonals are set to x = ±7000, y = ±7000. These should be versatile for most use cases. However, it's worth trying to other values to see if they feel better or are more suitable for your playstyle.

> **Note**
> These may be out-of-date | historical | etc etc. Values presented below were mentioned by the corresponding user in PhobGCC discord as their preferred values at the time. This obviously might have changed.

**Rienne's Recommended Analog Diagonals Values**

Mentioned on Feb 18, 2023:

* North (top|high) corners: set y = 7250
* South (bottom|low) corners: set y = 6750

**CarVac's Preference (Falcon)**

Mentioned on Aug 22, 2022: 

* Lower cotrol stick diagonals with y ≤ 7000 (jab cancel values). 
* This allows to jab, return to crouch, jab by holding down and back (as an example).

**Frosts's Preference (Ice Climbers)**

Mentioned on Aug 22, 2022:

* South (bottom|low) corners - set y = 6875

## Commands Quick Reference

|Command|Buttons|
|-------|-------|
|Safe Mode on\off|AXY+Start|
|Display Version|AZ+Du|
|Soft Reset|ABZ+Start|
|Auto-Initialize|AXY+Z|
|Increase/Decrease Rumble|AB+Du/Dd|
|Show Current Rumble Setting|AB+Start|
|Analog Stick Calibration|AXY+L|
|C-Stick Calibration|AXY+R|
|Advance Calibration|A or L or R|
|Undo Calibration|Z|
|Skip to Notch Adjustment|Start|
|Notch Adjustment CW/CCW|X/Y|
|Notch Adjustment Reset|B|
|Analog X-Axis Snapback Filtering|AX+Du/Dd|
|Analog Y-Axis Snapback Filtering|AY+Du/Dd|
|Analog X-Axis Waveshaping|LX+Du/Dd|
|Analog Y-Axis Waveshaping|LY+Du/Dd|
|Analog X-Axis Smoothing|RX+Du/Dd|
|Analog Y-Axis Smoothing|RY+Du/Dd|
|Show Analog Filtering Settings|L+Start|
|C-Stick X-Axis Snapback Filtering|AXZ+Du/Dd|
|C-Stick Y-Axis Snapback Filtering|AYZ+Du/Dd|
|C-Stick X-Axis Waveshaping|LXZ+Du/Dd|
|C-Stick X-Axis Waveshaping|LXZ+Du/Dd|
|C-Stick X-Axis Offset|RXZ+Du/Dd|
|C-Stick Y-Axis Offset|RYZ+Du/Dd|
|Show C-Stick Settings|R+Start|
|Swap X with Z|XZ+Start|
|Swap Y with Z|YZ+Start|
|Swap X with L|LX+Start|
|Swap Y with L|LY+Start|
|Swap X with R|RX+Start|
|Swap Y with R|Ry+Start|
|Toggle L Trigger Mode|AB+L|
|Toggle R Trigger Mode|AB+R|
|L-trigger Offset|LB+Du/Dd|
|R-Trigger Offset|RB+Du/Dd|

## 3rd Party Resources

### SmashScoppe


* **Download Link**: [https://goomwave.com/wp-content/uploads/2020/06/SmashScope.zip](https://goomwave.com/wp-content/uploads/2020/06/SmashScope.zip)
* **Video Guide**: [https://youtu.be/XzgS1aDb7TQ](https://youtu.be/XzgS1aDb7TQ)

#### SmashScoppe on Dolphin

1. Do not use the Slippi Dolphin build, instead download mainline Dolhin at [https://dolphin-emu.org/download/](https://dolphin-emu.org/download/) (Windows/MacOS). On Linux - either use your distribution's pre-built package or [build it yourself](https://wiki.dolphin-emu.org/index.php?title=Building_Dolphin_on_Linux).
2. If using a Mayflash, OEM or any other 2/4 port GCC adapter - use Port 1. In Dolphin controller settings, disable all Wiimotes.

### Install Slippi and Overclock Adapter on Arch Linux (or Arch-based distros)

Here's a [guide I wrote for myself](https://gist.github.com/SirToffski/be41fa9a7e2a2629fad811da80f1a685) to use as a reference (it's easy to forget all the steps). It should be up-to-date and revelant as of April 12, 2023.

