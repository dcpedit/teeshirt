# Large Build Guide

![Large-1](https://user-images.githubusercontent.com/800930/204630745-fb1a190e-5a30-441b-8503-5a56ddbc61a6.jpg)

This guide is based on the exact build that is pictured above.  Feel free to customize it to your fit your needs.

## Components

| Part | Count | Description |
| ---- | ----- | ----------- |
| Elite-C | 1 | Microcontroller |
| Wires | 2 | Connects data lines to PCB |
| Pin | 1 | For power connection |
| 5.1k resistor| 2 | Through hole pulldown resistors for USB-C |
| Diodes | 22 | BAV70 SMD |
| Switch sockets | 42 | Kailh hot swap sockets |
| OLED | 1 | SSD1306 128x32 |
| Rotary encoder | 1 | EC11 |
| Encoder knob | 1 | No more than 20mm diameter |
| Plate foam | 1 | 3.5mm (or 1.5mm + 2mm) EVA foam |
| Bottom foam | 1 | thickness varies |
| Switch plate | 1 | 1.5mm acrylic |
| OLED window | 1 | 3mm transparent acrylic |
| Stabalizers | 2 | 2u PCB mount |
| Keycaps | 42 | 36x1u, 2x1.25u, 2x1.5u, 2x2u |

## Adobe Illustrator Layers

| Name | Description | Material |
| ---- | ----------- | -------- |
| Window | OLED window | 3mm or 1.5mm transparent acrylic |
| Plate 2u | Switch plate for 2u spacebars | 1.5mm acrylic |
| Plate 1u | Switch plate for 1u or 1.5u spacebars | 1.5mm acrylic |
| Foam Plate | Switch plate foam | 3.5mm foam (ex: 1.5mm + 2mm EVA) |
| Foam Bottom | Case foam | Thickness depends on case (ex: 1mm EVA) |


## Assembly steps

Note that only the rotary encoder and OLED components are on the front of the PCB.  All other components are on the back.

### Solder diodes

![teeshirt_build-1](https://user-images.githubusercontent.com/800930/204630873-d411653c-2c77-4267-ba2b-42ecb0db7cc2.jpg)

Place a dab of solder on the single bottom pad of the diode on the PCB.  Then using tweesers, position the diode so that the legs line up with the pads.  Then using the point of one tweeser leg, gently hold the top of the diode in place while melting the dab of solder that was placed on the bottom pad previously.  With the diode now held in position, solder the top two legs to their respective pads.

### Solder switch sockets

Place some solder on one of the hot swap socket pads.  There should ben enough solder to make a small mound.  Place the socket into position and melt the mound of solder that was previously added while pressing down on the center of the socket.  Be sure to avoid touching any metalic parts to prevent burns.  Keep the soldering iron on the pad long enough for the solder to flow around the socket connector (usually around 3 to 4 seconds).  Now solder the other socket connector to the pad.


### Solder 5.1k resistors

![teeshirt_build-2](https://user-images.githubusercontent.com/800930/204630957-ace9f2de-4552-497d-b77c-9ad3dfd51f0e.jpg)

Bend the legs of each resistor and place them into position on the back of the PCB.  Orientation does not matter.  Bend the legs outwards to keep them in place, and flip the PCB over to the front to solder them in.  Clip protruding legs with flush cutters.

### Prep Data Wires

Strip both ends of 2 wires and solder them to the D+ and D- holes on the Elite-C.  Keep the wires and solder joints as flush as possible on the back side of the MCU.  I use flush cutters to snip off any of the wire that protrotrudes BEFORE soldering.  Then I use a minimal amount of solder to fill the hole but not create a mound that sticks too far out.

Tip: make sure the wire is long enough to reach the D+/D- holes on the PCB before cutting them.  Use different color wires to easily differentiate between positive and negative.

### Solder MCU

Move your MCU into position and place the power pin through the VBUS hole to make sure it's ligned up to the VBUS hole on the PCB.  Solder the Elite-C directly to the bottom of the PCB.  Then solder the data wires to the PCB making sure that D+ and D- match on both ends.

Tip: route wires so that they can lay as flat as possible against the MCU/PCB.

### Solder power pin to MCU

Place the power pin back into the VBUS hole on the MCU so that it goes all the way through the PCB.  Solder both sides of the pin and clip off the extra.  Don't use too much solder so that the pin can be clipped as close to the PCB as possible.

### Solder rotary encoder

![teeshirt_build-3](https://user-images.githubusercontent.com/800930/204631045-a462198e-3c04-4382-855b-4ebf5dabbf25.jpg)


Insert rotary into the front of the PCB and bend all the legs inwards.  After soldering the pins, you can also bend the 2 metal support flaps inwards as well.

### Solder OLED display

For this particular build, the OLED display is soldered right up against the PCB so that it's as low-profile as possible.  This allows for the OLED window to be attached directly onto the switch plate.  Using headers would add too much height to use a window, or would require a different window design which utilizes standoffs.  (There's only 5mm of space between the top of the PCB and the top of the switch plate)

Place a strip of electrical tape on the PCB where the OLED screen will touch the PCB.  Solder the connection pins to the OLED screen, or if they're already pre-soldered, remove the plastic spacer from the pins.  Place the OLED into position on the front of the PCB and flip it over while holding the display in place with your finger or with heat resistant tape.  Place just enough solder on one of the legs to hold in in place and check that the display is not crooked.  Once everything is straight, solder the other legs in place.

### Install stabalizers

![teeshirt_build-4](https://user-images.githubusercontent.com/800930/204631089-7975df50-24e2-487b-b143-29ad0b87ae12.jpg)

### Place bottom foam into case

![teeshirt_build-5](https://user-images.githubusercontent.com/800930/204631188-4d0fae8f-84ad-4b77-a003-ad95730c5e91.jpg)

### Mount PCB into the case

![teeshirt_build-6](https://user-images.githubusercontent.com/800930/204631222-334b8354-3e6b-4881-9209-896454485441.jpg)

### Lay plate foam on top of PCB

![teeshirt_build-7](https://user-images.githubusercontent.com/800930/204631253-5c81fe26-5f26-4869-97af-43bc12b2da99.jpg)


### Attach OLED window to switch plate

Using glue of your choice, place a dab of it on each corner and glue the window into position while making sure it's centered over the plate hole.

### Position switch plate on top of foam

![teeshirt_build-8](https://user-images.githubusercontent.com/800930/204631314-45af0e46-ce2f-44d8-a119-79afce2f8eff.jpg)


### Install switches

![teeshirt_build-9](https://user-images.githubusercontent.com/800930/204631362-22a622c3-47e4-4cff-a989-c10673f6b338.jpg)


### Install rotary encoder knob

### Install keycaps
