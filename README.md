# BBC Master Mini EEPROM Cartridge

## Overview
A [LibrePCB](https://librepcb.org) format PCB design for an Acorn BBC Master 128 EEPROM cartridge which is small enough sit completely inside the Master's case, under the cartridge flap, safe from the children's prying fingers. I created this board as I needed to add more sideways ROMs to the machine in a child-proof way without sacrificing the Master's sideways RAM and couldn't find an existing solution. This was also a nice simple project to try creating a PCB which is something I've not done before, so there are no doubtless some mistakes.

![Cartridge front](docs/master-mini-cart-front.png?raw=true) ![Cartridge back](docs/master-mini-cart-back.png?raw=true)

The schematic is based on a modification for BBC Master ROM cartridges [(schematic on mdfs.net)](https://mdfs.net/Info/Comp/BBC/Circuits/Master/eprom.gif) as detailed in the StarDot forums [EEPROM - the Holy Grail of Sideways Rom](https://stardot.org.uk/forums/viewtopic.php?f=3&t=7393) thread. Please take time to read through this thread, in particular the need for the hardware write protect switch, links to software and details of how to program the EEPROM in place.

## Important
**Please note** that this project was only ever intended for my own use; it is an experiment. There is no guarantee that it is fit for any purpose, use it at your own risk.

**Warning: to avoid potentially damaging the Master, care is needed when inserting the cartridge:**
- The _front_ of the cartridge in marked on the silk screen. The board **must** be inserted with its _front_ side facing the Master's keyboard.

## Components

| Designator | Qty | Value | Description                                | Package |
|------------|-----|-------|--------------------------------------------|---------|
| C1, C2     | 2   | 100nF | Ceramic capacitor.                         |         |
| C3         | 1   | 47µF  | Electrolytic capacitor.                    |         |
| R1         | 1   | 10kΩ  | Resistor 5%                                |         |
| IC1        | 1   |       | Microchip AT28C256-15PU.                   | PDIP    |
| IC2        | 1   |       | 74HCT139.                                  | PDIP    |
| PL2        | 1   |       | 3 pin 2.54mm spaced header or SPDT switch. |         |

## Acknowledgements
- Contributors to the StarDot [EEPROM - the Holy Grail of Sideways Rom](https://stardot.org.uk/forums/viewtopic.php?f=3&t=7393) thread.
- [BBC Master ROM cartridge schematic (mdfs.net)](https://mdfs.net/Info/Comp/BBC/Circuits/Master/eprom.gif)

## License
The files in this repository are published under the CERN-OHL-P license.

Note that **this license does not apply** to the design of the circuit on which this is based. These are the work of others, see the acknowledgements section.
