# Medium Build Guide

This guide is based on the exact build that is pictured above.  Feel free to customize it to your fit your needs.

## Components

| Part | Count | Description |
| ---- | ----- | ----------- |
| Elite-C | 1 | Microcontroller |
| Diodes | 22 | BAV70 SMD |
| Switch sockets | 42 | Kailh hot swap sockets |
| OLED | 1 | SSD1306 128x32 |
| Rotary encoder | 1 | EC11 |
| Encoder knob | 1 | No more than 20mm diameter |
| Plate foam | 1 | 3.5mm (or 1.5mm + 2mm) EVA |
| Bottom foam | 1 | 1.5mm EVA |
| Switch plate | 1 | 1.5mm acrylic |
| Stabalizers | 2 | 2u PCB mount |
| Keycaps | 42 | 36x1u, 2x1.25u, 2x1.5u, 2x2u |
| Acrylic case layers | 7 | 3mm white acrylic (top & bottom layer is transparent gray)
| M2x13mm standoff | 10 | Case perimeter |
| M2x6mm standoff | 9 | PCB mount |
| M2x3mm screw | 9 | PCB mount bottom |
| M2x4mm screw | 19 | PCB mount top & case bototm |
| M2x8mm screw | 10 | Case top |
| Non-slip bottom | 1 | 1.5mm adhesive neoprene

## Adobe Illustrator Layers

| Name | Quantity | Material |
| ---- | ----------- | -------- |
| #1 Top 1u Clear | 1 | 1.5mm transparent acrylic |
| #2 Top spacer | 1 | 1.5mm acrylic |
| #3 - #4 Mid spacer | 2 | 1.5mm acrylic |
| #5 - #6 Bottom spacer | 2 | 1.5mm acrylic |
| #7 Bottom | 2 | 1.5mm acrylic |
| Bottom Foam | 1 | 1.5mm EVA |
| Bottom Rubber | 1 | 1.5mm adhesive neoprene |
| Plate Foam | 1-2 | 3.5mm EVA (or 1.5mm + 2mm EVA) |
| 2u Plate Floating | 1 | 1.5mm acrylic |

## Assembly steps

### Solder diodes

Place a dab of solder on the single bottom pad of the diode on the PCB.  Then using tweesers, position the diode so that the legs line up with the pads.  Then using the point of one tweeser leg, gently hold the top of the diode in place while melting the dab of solder that was placed on the bottom pad previously.  With the diode now held in position, solder the top two legs to their respective pads.

### Solder switch sockets

Place some solder on one of the hot swap socket pads.  There should ben enough solder to make a small mound.  Place the socket into position and melt the mound of solder that was previously added while pressing down on the center of the socket.  Be sure to avoid touching any metalic parts to prevent burns.  Keep the soldering iron on the pad long enough for the solder to flow around the socket connector (usually around 3 to 4 seconds).  Now solder the other socket connector to the pad.

### Solder MCU

Solder the Elite-C directly to the bottom of the PCB.


### Solder rotary encoder

Insert rotary into the front of the PCB and bend all the legs inwards.  After soldering the pins, you can also bend the 2 metal support flaps inwards as well.

### Solder OLED header

There's only 10mm of space between the PCB and the transparent acrylic top layer, so the OLED + header cannot exceed this height.  For this build, I had to dremel/sand the plastic part of the header down to about 7mm.  I also had to remove the plastic spacer on the OLED pins and clip the pins to fit into the shorter header.  Insert the display into the header and make sure the total height is under 10mm before soldering the header onto the front of the PCB.

### Install stabalizers

### Case assembly

* Attach the 10 M2x13mm standoffs around the perimeter of the bottom case layer with the M2x4mm screws
* Assemble 9 PCB mounts by screwing a M2x3mm screw into one end of a M2x6mm standoff.  Then take the mount assembly and slip it into the mount holes on the bottom case layer so that all the screw heads are on the bottom.
* Slip #5 - #6 bottom spacer layers over the perimeter standoffs
* Put the bottom foam into the case
* Mount the PCB into the case standoffs using M2x4mm screws
* Slip #3 - #4 mid spacer layers over the perimeter standoffs
* Put the plate foam onto the PCB
* Put the switch plate on top of the plate foam, making sure the switch holes are lined up
* Push all the switches into the hotswap sockets (note north vs. south facing)
* Insert OLED display into the header
* Slip #2 top spacer layer over the perimeter standoffs
* Slip #1 top clear layer over the perimeter standoffs
* Secure all case layers with the M2x8mm screws

### Install neoprene bottom

Remove the paper on the adhesive side of the neoprene, and carefully lay it over the bottom of the case. Start on one side while smoothing air bubbles out.  You may have to stretch the neoprene during this process to get the screw heads to line up with the holes.

### Install keycaps