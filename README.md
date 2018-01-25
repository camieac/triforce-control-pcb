# triforce-control-pcb

## Repository Navigation
This repository hosts the electronics hardware designs for the Triforce Fight Controller. Links to the main software repositories are below:

### [Triforce Control](https://github.com/TeamTriforceUK/triforce-control)

The Triforce Control firmware (mbed OS) runs on an LPC1768 (ARM Cortex M3). The firmware is responsible for controlling the robot.

### [Triforce Telemetry](https://github.com/TeamTriforceUK/triforce-telemetry)

The Triforce Telemetry repository hosts firmware (FreeRTOS) for the ESP8266 WiFi chip. This microcontroller works alongside the mbed to provide telemetry functionality via an HTTP server.

The ESP8266 allows us to communicate telemetry from Triforce to connected mobile devices (tablets, laptops, mobile phones). We also control non-safety critical settings such as LED lights from the mobile device.

## System Overview

### Microprocessors

| Device  | Firmware  | Language |
|---------|-----------|----------|
| [LPC1768](https://developer.mbed.org/platforms/mbed-LPC1768/) | [mbed OS](https://www.mbed.com/en/development/mbed-os/)   | C++      |
| [ESP8266](https://www.adafruit.com/product/2471) | [FreeRTOS](http://www.freertos.org/)  | C        |

### Sensors

| Sensor | Purpose                              | Communication |
|--------|--------------------------------------|---------------|
| [BNO055](https://learn.adafruit.com/adafruit-bno055-absolute-orientation-sensor/overview) | Orientation, direction, acceleration |  I2C          |

# PCB Spec

# Board Dimensions

| Width | Height | Thickness |
|-------|--------|-----------|
| 75mm  | 85mm   | 1.6mm     |

# Useful Links

## Enclosure

https://www.hammfg.com/files/parts/pdf/1455J1202.pdf
https://www.hammfg.com/part/1455J1202

## Generating gerber files

http://support.seeedstudio.com/knowledgebase/articles/1824574-how-to-generate-gerber-and-drill-files-from-kicad

## Contributing

We are open to any contributions in terms of ideas, suggestions, bug reports, development. Feel free to open GitHub issues regarding any contributions.

## Licensing

Licensed under CERN OHL v.1.2.
