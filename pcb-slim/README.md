# TeeShirt PCB

The PCB automatically applies power to the VBUS pin, but if you want to also send power to the RAW pin (#24), you can short JP1.

If you're relocating the USB port to the upper left of the PCB for the large sized (60%) builds, make sure you also soldering in 5.1k resistors, as well as connecting the data pins on the PCB (D+/D-) to the data pins/pads to the MCU with wires.