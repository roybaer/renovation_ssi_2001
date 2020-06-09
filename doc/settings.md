# Jumper settings

Both, the audio section and the joystick section of the card can be configured with jumpers.
This document lists all sensible jumper settings.

## Audio section

The audio section can be configured to use at most one out of four possible I/O port ranges.

Setting | Meaning
--------|--------
░░░░    | Audio disabled
█░░░    | Ports 280h to 29fh
░█░░    | Ports 2a0h to 2bfh
░░█░    | Ports 2c0h to 2dfh
░░░█    | Ports 2e0h to 2ffh

## Joystick section

The built-in IBM compatible analog joystick interface at port 201h can be en- or disabled and its sensitivity can be adjusted.
The jumper positions of vertical jumper banks are shown from left to right rather than from top to bottom.

Setting | Meaning
--------|--------
░       | Joystick disabled
█       | Joystick enabled

Setting | Meaning
--------|--------
░░░     | Normal sensitivity
█░░     | High sensitivity
░█░     | Normal sensitivity
░░█     | Low sensitivity
