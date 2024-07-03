# USBASP Programmer Module using altium designer

## Overview
USBasp is an in-circuit serial programmer designed for the Atmel AVR Microcontroller family. It is a low-cost programmer that converts hex files (.hex) into AVR microcontrollers, utilizing an Atmega8 or Atmega88 microcontroller and a few passive components. No special USB controller is required since the programmer uses a firmware-only USB driver.

## Features
- **No special USB controller required**
- **Programming speed up to 5Kbytes/sec**
- **Supported platforms**: Linux, Windows, Mac OS X
- **Read/write capabilities**: EEPROM, firmware, fuse bits, and lock bits
- **No special controllers or SMD components needed**
- **Low clock speed support**: SCK option for target with <1.5MHz clock speed
- **Status indicators**: Programming status and bus status easily identified
- **Easy interface**: Header pins for various ISP header pins
- **Dimensions**: 63.3 x 20.5 x 10.5mm
- **Weight**: 15g

## Description
USBasp is designed to program AVR microcontrollers directly via USB without requiring a special USB controller. The programming speed is up to 5Kbytes/sec, and it works across multiple platforms including Linux, Windows, and Mac OS X. The programmer allows for reading or writing the microcontroller's EEPROM, firmware, fuse bits, and lock bits, and supports targets with a low clock speed of less than 1.5MHz through the SCK option.

### How It Works
To program a microcontroller, we need to access four pins of the microcontroller, but our USB will have only two pins for communication. The USBasp programmer resolves this by utilizing a firmware-only USB driver in an Atmega8 or Atmega88 microcontroller, eliminating the need for a special USB controller.

### Compact Design
The USBasp programmer features a 10-pin ISP connection to interface with the microcontroller at a programming speed of 5KB/sec. The USB interface is achieved using an Atmega8 processor, and the remaining functionality is handled by firmware. The compact and elegant design includes a 10-pin male header for various ISP header pins, making interfacing easier.

### Compatibility
The USBasp programmer works with a wide variety of Atmel AVR microcontrollers, including the Atmega8a and Atmega168a. The USBasp driver is compatible with both 32 and 64-bit platforms, ensuring functionality on Windows, Mac OS X, and Linux.

## Schematic and PCB
![USBASP Schematic](schematic.png)
![USBASP PCB](pcb.png)

## License
This project is licensed under the Creative Commons Attribution-ShareAlike 4.0 International License. For more details, see the [LICENSE](LICENSE) file.

[![Creative Commons License](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-sa/4.0/)

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).
