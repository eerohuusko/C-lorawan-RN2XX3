N2XX3 lib

http://ww1.microchip.com/downloads/en/DeviceDoc/40001811A.pdf

This is the shell of a C wrapper-library around the serial command API, over UART, for Microchip RN2483 and RN2903 LoRaWAN using Tindie breakout.

This project uses a RN2903A, on a breakout purchased from Azzy's Electronics on Tindie.

[Azzys Electronics](http://drazzy.com/e/)

[Azzys Electronics on Tindie](https://www.tindie.com/stores/DrAzzy/)

[Assembled breakout w RN2903 or RN2483](https://www.tindie.com/products/DrAzzy/lorawan-rn2483rn2903-breakout-board-assembled/)

This breakout is directly powered and connected by a Raspberry Pi Zero with Wifi and Ble (not a ZeroW, but technically the same).  The wiring for this is shown on the Tindie site above, where you can buy the breakouts, or below for convenience.

The setup, used is the top one pictured below:
![Wiring Diagram](http://drazzy.com/e/products/img/RN2483diagram2.jpg)


On the RPi, UART must be enabled and the serial console must be turned off. 

RN2XX3 modules do not have flow-control, so you can ignore the RTS/CTS pads on the breakout.

Here's the setup, using AdaFruit T Cobbler, RPi Zero and breakout:

![RPI Zero and RN3903 over UART](https://github.com/miguellan/python-lorawan-RN2XX3/blob/master/RN2903.jpg?raw=true)

The goal of this project, is to create a simple library, and starting point, for anyone evaluating RN2XX3 LoRaWAN chips.  If you found this repo helpful, and want to contribute.  Please fork, and create a pull request with your changes, and it will be merged.

