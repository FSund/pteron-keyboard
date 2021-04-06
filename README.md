# pteron keyboard
An ergonomic keyboard heavily inspired by the [Atreus](https://github.com/technomancy/atreus), [Iris](https://github.com/keebio/iris-case) and [Atreis](https://github.com/dekonnection/atreis) keyboards.

The name *Pteron* is the Ancient greek word for wing (and feather). This was inspired by *Chiroptera*, the scientific name (or order) of bats.
> The name “Chiroptera” derives from Ancient Greek: χείρ – cheir, “hand” and πτερόν – pteron, “wing”.
https://en.wikipedia.org/wiki/Bat#Etymology

<img src="https://github.com/FSund/pteron-keyboard/blob/master/builds/20201002_141317.jpg" width="640">

Check the [builds](/builds/builds.md) folder for more photos. 
The 56-key version shown in the photo above is built using 9 mm brass spacers. It can theoretically be built using spacers as small as 5 mm, but that requires very strict cable management.

## PCB
A PCB version of the pteron is in progress here: https://github.com/kraken-jokes/pteron-pcb

## Styles
#### 38 keys
<img src="https://github.com/FSund/zuboard/blob/master/images/38key-switch-plate-filled.png" width="560">

#### 44 keys
<img src="https://github.com/FSund/zuboard/blob/master/images/44key-switch-plate-filled.png" width="560">

#### 56 keys
<img src="https://github.com/FSund/zuboard/blob/master/images/56key-switch-plate-filled.png" width="560">

## Laser cutting
The default switch plate is designed for laser cutting with a kerf of 0.1 mm. The switch holes are designed for Cherry MX style switches, and should allow for switch top removal on both Cherry MX/Gateron/etc. and Kailh BOX switches. 

There is an alternative switch plate with square holes (`case/switch-plate-square-holes.svg`), which does not allow switch top opening, but which might add some stability to the switches.

I would recommend using 3 mm thick acrylic for stiffness, which means that the switches have to be glued in, since Cherry MX-style switches are designed for a plate thickness of ~1.5 mm.

#### Conversion
The .svg-files can be converted to dxf by first saving as .eps (via for example [Inkscape](https://inkscape.org/)) and then using the following [pstoedit](http://pstoedit.net/) command

    pstoedit -f "dxf_s: -mm -splineasbezier" infile.eps outfile.dxf

## Firmware
Firmware is available here: https://github.com/qmk/qmk_firmware/tree/master/keyboards/handwired/pteron

## Design
The initial inspiration was the [Atreis](https://github.com/dekonnection/atreis) keyboard, but I wanted some more stagger on the ring and pinky fingers. I ended up with a stagger of -0.7 u for the two outer columns, followed by -0.2 u, 0, -0.3 u and -0.4 u. I also removed the top thumb key, and added a key to the thumb cluster. 

## Licensing
> These works are licensed under the Creative Commons Attribution-ShareAlike 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by-sa/4.0/ or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.

This means you can run Group Buys of these designs, as long as you credit where the design came from (this repo).
