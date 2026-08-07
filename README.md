# telstar-atari-rf-to-composite-pcb

A PCB file you can use to order a PCB to make your Atari 2600 or Telstar able to output composite video.

> **Note:** This is to convert RF to composite. You will need an HDMI converter if you are using HDMI.

## Parts for Telstar

- One Telstar (obviously)
- PCB board listed in files
- 6 × 15k ohm resistors
- 1 × 1.3k ohm resistor
- 1 × 27k ohm resistor
- 1 × 480 ohm resistor
- 1 × 75 ohm resistor
- 1 × 100 gain transistor
- 1 × 220 µF capacitor
- 1 × CD4049 chip

## How to Configure for Telstar

> **Note:** The PCB board is also configured to support Atari 2600. You will not use color. You must connect luma to each of the 3 luma signals.

If you refer to `whatwiresarewhat.png`, you will see 4 wires towards the bottom of the photo all running through the same encasing:

- **Red** is power
- **Black** is ground
- **Yellow** is inverted luma
- **Blue** is inverted sync

The yellow jack is video output.

Sync connects to two ports of the chip by default, as well as LUMA 2. Luma 1 and Luma 0 each connect to one different gate of the chip.

**Left header is power, right header is ground.**

Look at the circuit schematic listed in the GitHub files.

To the left are our inputs which are 4 inverted luma signals, and 2 inverted sync signals.

The junction after the 15k resistor network, where they all connect, is going to be where your CD4049 chip will reside.

Each input will be inverted with the CD4049 chip before their respective resistor.

The rest you can see for yourself, having a transistor and the last 75 ohm resistor being our load.

Once you have that, solder the composite out from the PCB board, to the yellow wire that is directly to the right of the RCA jack on the Telstar board.

Then you should be able to use the RCA jack to plug to an HDMI converter and you're all set!

## How to Order

To use, you must upload the gerber file to [JLCPCB](https://cart.jlcpcb.com). There you can order it.

## How to Configure for Atari 2600

Coming soon...
