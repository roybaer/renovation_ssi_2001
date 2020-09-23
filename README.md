# Renovation SSI-2001

This repository contains the design files for the _Renovation SSI-2001_ sound card, a replica of the _Innovation SSI-2001_ with some unobtrusive modifications that eliminate the dependency on vintage parts.
The Innovation SSI-2001 was an 8-bit ISA sound card from the late 1980s that was based on Commodore's SID synthesizer chip.

This modified design can optionally use an STM32 microcontroller, instead.
It can also use two NE556 dual timer ICs instead of a single NE558 quad timer IC for the integrated analog joystick interface.
All optional modern replacement components share the location of the vintage parts they replace, so that the modifications are largely invisible in combination with vintage parts.

## Front view

This picture shows the front of the card.

![Front view](img/photo_front.jpg)

There is also a picture of the [back side of the card](img/photo_back.jpg).

## Optional vintage components

You will need the following vintage components for a visually accurate replica:

- A SID chip (MOS 6581 or MOS 8580, the latter with a hidden voltage regulator)
- An NE558 quad timer IC for the joystick interface

## Bill of materials

The design files of this project combine multiple possible hardware configurations in the same schematic diagram and PCB layout.
Hence, the unmodified tool-generated BOM will not yield a sensible hardware configuration.
Please read the notes in the schematic diagram, decide which variant you want to build and adjust the BOM, accordingly.

## Configuration

Please consult the [settings document](doc/settings.md) for jumper settings.

## Additional notes

The planned adaptation of the [STM32-SID-PLAYER](https://github.com/Bakisha/STM32-SID-PLAYER) firmware for this card, i.e. the implementation of an ISA interface for the synthesizer core is still pending.
Right now, this card is therefore only usable in combination with either an original SID or a modern substitute like the SwinSID.

The exact DA15 and RCA connectors found on the original card are no longer available and have therefore been replaced by affordable modern variants.
Furthermore, the RCA jack and the mounting holes have been shifted to simplify the adaptation of the generic Keystone 9202 ISA bracket.


## License

The following license applies to the files in this repository:

This work is licensed under the Creative Commons Attribution-ShareAlike 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by-sa/4.0/ or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.
