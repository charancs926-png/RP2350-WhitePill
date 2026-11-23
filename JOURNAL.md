---
title: "RP2350 WhitePill"
github: "https://github.com/charancs926-png/RP2350-WhitePill"
description: "A custom RP2350 Devboard"
created_at: "2026-11-21"
total_time: "7h"
---

# November 21, 2026: Schematic: Session 1

Started designing my first RP based custom DevBoard, I went for the most modern / latest MCU, i.e. RP2350A, thought of using RP2040 but why the downgrade hence RP2350A.
<br>
I used Raspberry's open source schematic and docs to make WhitePill...
<br>
Drawing the schematic, first by laying out the basic components, like Memory Flash, MCU pinouts, RGB LED, Crystal Oscillator, USB C, Decoupling capacitors.
<br>
![](https://fabricate.hackclub-assets.com/35ce2b9fa5e4ee182aef2e79b84047053932a079b4cde9c724507079de83a4f6/image-png/image.png)
<br>
Also got a sanity check side by side using Claude and GPT.

**Total time spent: 1h 36m**

# November 21, 2026: Schematic Session 2

Continued with the left over schematic, added external SD card, & battery management. 
<br>
referred a couple of designs and routed the power & battery management, hope i don't blow up my PCB.
<br>
verified & sanity checked the Schematic, ready for PCB routing : ) yayy !
<br>
![](https://fabricate.hackclub-assets.com/25dd66cc578b694b66a753e109277299c81ee1fe771518bdd0562793953a6b52/image-png/image.png)
<br>
Did a little tidying up, making it look Polished enough... didn't draw boxes as it makes weirdly neat.
<br>

**Total time spent: 1h 12m**

# November 23, 2026: Routed the PCB

Decided to try routing the board using 2 layer JLCPCB Fab.
<br>
I assigned all footprints and imported everything to the PCB editor. Then I started positioning and laying out the components on the board, it's still not done yet but this is how it's looking for now (focused on the decoupling capacitors, definitely not even close to finished yet :/
<br>
then routed the missing traces (had to change some existing routes positions and add some vias but didn't change too much), added one more GND pin to each header, added silkscreen and also filleted the PCB corners.
<br>
![](https://fabricate.hackclub-assets.com/1cb08fdbde082206222eb7e9ef07a7f066517f4743cd3bcee3b5ec6eb5332559/image-png/image.png)
<br>
![](https://fabricate.hackclub-assets.com/032e7c7049c1658fc3ad2cc503deca7e31d9079328784c77d284564165e8ea6f/image-png/image.png)
<br>
![](https://fabricate.hackclub-assets.com/bb945968b39cd2ca67d8c20ea204ae533705c0469151d09b956b5958edf67e52/image-png/image.png)

**Total time spent: 3h 12m**

# November 23, 2026: DRC and Project File Organization

After running a quick DRC, found a couple of errors, like POWER_FLAGS, Trace Not connected, & Unused Vias, after fixed that and actually sort of tidying up the routings, I ran the DRC and got 0 errors.. ;)
<br>
Went forward with gerber generation, and re checking the schematic and pcb design.
<br>
Then I organized my files on the basis of
- PCB
- firmware
- docs
- journal
- production ( contains the gerber files )
- BOM.csv
- ReadMe.md
<br>
![](https://fabricate.hackclub-assets.com/12d6ad8184ee871df2034157d2299c0a4f10f19521bdbc56aff549700b507203/image-png/image.png)

**Total time spent: 1h**
