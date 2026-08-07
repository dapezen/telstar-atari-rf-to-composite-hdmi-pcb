# telstar-atari-rf-to-composite-pcb
A PCB file you can use to order a PCB to make your Atari 2600 or Telstar able to output composite video.

NOTE: THIS IS TO CONVERT RF TO COMPOSITE YOU WILL NEED HDMI DECODER IF YOU ARE USING HDMI.

PARTS FOR TELSTAR
One tesltar (obviously)
PCB board listed in files
6 15k ohm resistors
1 1.3k ohm resistor
1 27k ohm resistor
1 480 ohm resistor
one 75 ohm resistor
one 100 gain transistor
one 220 uF capacitor.
1 cd4049 chip



HOW TO CONFIGURE FOR TELSTAR
Note: THE PCB BOARD IS ALSO CONFIGURED TO SUPPORT ATARI 2600. YOU WILL NOT USE COLOR. YOU MUST CONNECT LUMA TO EACH OF THE 3 LUMA SIGNALS.
If you refer to what whatwiresarewhat.png. You will see 4 wires towards the bottom of the photo all running through the same encasing. Red is power, black is ground, yellow is inverted luma, and blue is inverted sync. The yellow jack is video output.
Sync connects to two ports of the chip by default, as well as LUMA 2. Luma 1, and Luma 0 each connect to one different gate of the chip.
LEFT HEADER IS POWER, RIGHT HEADER IS GROUND
Look at the Circuit Shematic listed in github files.
To the left are our inputs which are 4 inverted luma signals, and 2 inverted sync signals.
The junction after the 15k resistor network where they all connect is going to be where your cd4049 chip is going to be.
Each input must be inverted with the cd4049 chip after their respective resistor.
The rest you can see for yourself, having a 100 gain transistor and the last 75 ohm resistor being our load.

HOW TO ORDER
To use you must upload the gerber file to https://cart.jlcpcb.com. There you can order it.

HOW TO CONFIGURE FOR ATARI 2600
Coming soon...
