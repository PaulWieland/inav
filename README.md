# ABOUT THIS FORK
This fork was made to remap the softserial pins for the Matek F405 Mini.
I wanted to use the F405 Mini without the PDB Hub, which means I could not use UART5.

This change allows the following setup for my Nano Goblin:

* UART 1 - Crossfire RX & Telemetry
* UART 3 - GPS
* UART 4 - Crossfire Bluetooth link (MSP). Allows iOS to update the iNav settings, upload of mission waypoints over the Crossfire bluetooth link.
* SoftSerial 1 - TBS Smart Audio
* SoftSerial 2 - RunCam serial camera control

UART2 is not usable because it was replaced with a softserial port. This was done because the hardware UART is inverted for SBUS.
