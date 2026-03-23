# PVS Nachtmahr V2
A thermal monocular, based on the original Idea of Lupus Worax, that use N6 thermal core

The idea here is to have a modified version of the Nachtmahr (https://www.printables.com/model/1259454-pvs-nachtmahr-50hz-thermal-vision-light-weight-dvr) , that will work with an N6 thermal core, and use the same "new" control hardware: rotary encoders and push buttons.
Why to use this, instead of the Gremlin V2? 
Well.. first of all, because it has more space... 😉
Second, it can use a DVR (sometimes very very handy). Last but not least, I really loved the idea of an internal rechargeable battery.

This is a WIP, completely based on the great work of Lupus Worax. Many guides can be found on his discord channel (https://discord.com/channels/1336624444369670154)

### ESP Firmware
The last firmware to use can be found here: https://discord.com/channels/1336624444369670154/1337755087228895282 
| Action | Single Click / Rotation | Shift Held (Thumb Button - GPIO 7) |
| :--- | :--- | :--- |
| **Rotate Encoder** | **Digital Zoom** (1x to 8x) | **Brightness** (0-127) |
| **Short Press (Encoder)** | **Cycle Palettes** (5 modes) | **Cycle Contrast** (Incremental) |
| **Long Press (Encoder)** | **Image Enhancement** (1.5s) | **Dead Pixel Correction** (5s) |
| **Short Press (Thumb)** | **Manual Calibration** (NUC) | — |
| **Long Press (Thumb)** | **Toggle Auto-Calibration** (3s) | **Toggle WiFi/OTA** (5s) |

### Build guide
Building the Nachtmahr v2 is very similar to V1, and you can find the guide [here](https://docs.google.com/document/d/1FID4HvsZnoMsb9pfEZISi7Dp_-eUuumutZ-1HBHcEDI/edit?usp=drive_link). The main difference is related to the 2 push buttons (the one for DVR and the one on the main body). You have to cut out 2 of the 4 pins (check with a multimeter which one to keep), and file the button so it can fit perfectly in the home. Sold the 2 wires before inserting it, and then you're good to go.
The complete wiring schematics can be found [here](https://github.com/tommasodidonato/nachtmahr_V2/blob/main/wiring%20nachtmahr%202.jpg)

### Printing tips
You can use whatever material you like best. PLA is ok, as long as you don't plan to leave it in the car during the hot season. The images you see here refer to my build in ASA. I strongly suggest 4 walls, infill at least 15%, line height 0.2 is ok. For TPU, I printed with 0.16 line height. 
Supports are mandatory for many parts, settings depend on your printer (I used tree structure, 0.4 distance from x/y, density 70%). If you plan to use ASA or other shrinking materials, print accordingly; I strongly suggest to do a dimensional test print before printing everything. I also enlarged the screw holes with a drill before the assembly (it will saves you a lot of heachaches)

### General tips
Charge your LiPo batteries separately before assembling the power block. 
**Remember to remove the A and B resistance** from the boost converter. Before going on, double check with a multimeter that the booster output is really 5V... 
When glueing the power button and the rotary encoder, do not use normal super glue (if it goes into the button, then you will have to change it!). I suggest the gel one.
