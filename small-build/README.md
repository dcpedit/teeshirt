# Small Build Guide

![teeshirt-8](https://user-images.githubusercontent.com/800930/204634106-3f1c62ce-4639-45f3-b919-df7657a722be.jpg)

This guide is based on the exact build that is pictured above.  Feel free to customize it to your fit your needs.

## Components

| Part | Count | Description |
| ---- | ----- | ----------- |
| Nice!Nano | 1 | Microcontroller |
| Battery | 1 | 3.7v litium (ex: 301230) |
| MCU headers | 2 | 1x12 pin (Mill Max 310-93-112-41-001000) |
| MCU pins | 24 | round (Mill Max 3320-0-00-15-00-00-03-0) |
| Diodes | 22 | BAV70 SMD |
| Switch sockets | 43 | Kailh hot swap sockets |
| OLED display | 1 | SSD1306 128x32 |
| OLED header | 1 | 1x4 pins |
| Switch plate | 1 | 1.5mm acrylic |
| OLED/MCU guard | 1 | 3mm transparent acrylic |
| Bottom plate | 1 | 3mm acrylic |
| M2x5mm standoff | 13 | 9 for the bottom, and 4 for the guard |
| M2x4mm screws | 26 | Wafer head screws |
| Stabalizers | 2 | 2u PCB mount |
| Keycaps | 43 | 37x1u, 2x1.25u, 2x1.5u, 2x2u |

## Adobe Illustrator Layers

| Name | Description | Material |
| ---- | ----------- | -------- |
| Clear guard | OLED/MCU window/guard | 3mm transparent acrylic |
| 2u Switch Plate | Switch plate for 2u spacebars | 1.5mm acrylic |
| 1u Switch Plate | Switch plate for 1u or 1.5u spacebars | 1.5mm acrylic |
| Bottom Plate | Keyboard bottom | 3mm acrylic |


## Assembly steps

This particular build does not use foam, but the foam layers are included in the Illustrator file.

### Solder diodes

Place a dab of solder on the single bottom pad of the diode on the PCB.  Then using tweesers, position the diode so that the legs line up with the pads.  Then using the point of one tweeser leg, gently hold the top of the diode in place while melting the dab of solder that was placed on the bottom pad previously.  With the diode now held in position, solder the top two legs to their respective pads.

### Solder switch sockets

Place some solder on one of the hot swap socket pads.  There should ben enough solder to make a small mound.  Place the socket into position and melt the mound of solder that was previously added while pressing down on the center of the socket.  Be sure to avoid touching any metalic parts to prevent burns.  Keep the soldering iron on the pad long enough for the solder to flow around the socket connector (usually around 3 to 4 seconds).  Now solder the other socket connector to the pad.

### Solder OLED header

There's only 10mm of space between the PCB and the clear acrylic guard, so the OLED + header cannot exceed this height.  For this build, I had to dremel/sand the plastic part of the header down to about 7mm.  I also had to remove the plastic spacer on the OLED pins and clip the pins to fit into the shorter header.  Insert the display into the header and make sure the total height is under 10mm before soldering the header onto the front of the PCB.

### Solder MCU headers and pins

As mentioned before, there's only 10mm of space between the PCB and the clear acrylic guard, so the total hight of the MCU after it's been mounted can't exceed this hight.  Place the two 1x12 headers on the top of the PCB and solder them into place.  

Now place a piece of masking tape over the headers and insert the pins into each hole.  Place the MCU over the pins (components facing down towards the PCB) and make sure it's seated flush against the masking tape.  You can now solder the pins.  Once the joints have cooled, SLOWLY wedge your fingertips into the gap under the MCU on BOTH sides until it's free from the header.  Pulling too hard and unevenly may bend the pins when one side suddenly becomes free.  With the MCU removed, you can now remove the masking tape.

### Attach battery

I'd suggest first placing the batter under the installed MCU to see what orientation makes the most sense.  For my build, it was with the battery wires exiting on the top left of the battery.  If you wish to cut the battery wires to the correct lenght, you can do that now, or just tuck the extra wire under the MCU.

With the MCU removed, solder the red wire into the B+ hole, and black wire into the B- hole.  Note that this build did not incorporate a power switch.

You can now reattach the MCU to the board.

### Install stabalizers

### Mount PCB into bottom plate

Attach 9 M2x5 standoffs to the bottom plate using the 4mm screws.  Now secure the PCB to the standoffs using another 9 screws.

![bottom-2](https://user-images.githubusercontent.com/800930/204677351-f58dc7f1-dbed-47c5-af47-207aa5c7b779.jpg)

### Install standoffs for clear guard

Attach 4 M2x5 to the switch plate using the 4mm screws.  Don't attach the actual clear guard yet since that's done at the end of the build.

### Install the switch plate and switches

Using your finger or a "switch plate support fork" to hold the plate 3.5mm away from the PCB, insert your switches.  It's important to keep that 3.5mm gap through the entire plate so that your switches are able to "snap" into place.

### Attach OLED display

Insert the OLED display into the header.  You can optional place a piece of foam tape under the display to hold it in place if it feels unstable.

### Install clear acrylic guard

Secure the guard to the standoffs using 4 M2x4 screws.

### Install keycaps
