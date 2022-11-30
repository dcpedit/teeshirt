# TeeShirt PCB

<img width="600" alt="pcb-slim" src="https://user-images.githubusercontent.com/800930/204702761-ff5b40e0-e514-4277-8559-1164e2c33ebf.png">

The PCB automatically applies power to the VBUS pin, but if you want to also send power to the RAW pin (#24), you can short JP1.

![teeshirt_build-1](https://user-images.githubusercontent.com/800930/204702844-717b1569-ac3a-480a-893e-422eba853227.jpg)

If you're relocating the USB port to the upper left of the PCB for the large sized (60%) builds, make sure you also soldering in 5.1k resistors, as well as connecting the data pins on the PCB (D+/D-) to the data pins/pads to the MCU with wires.
