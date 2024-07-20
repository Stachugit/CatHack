# CatHack Firmware for M5StickCPlus2

CatHack is a firmware designed for the M5StickCPlus2, incorporating a wide range of functionalities for infrared, SubGhz, WiFi, and Bluetooth operations. 

## Features

### Infrared Menu
- **tvbgone**: Turn off all nearby televisions.

### SubGhz Menu
- **SubSend**: Send .sub files from the Flipper Zero using the CC1101 module. Currently, only the RAW protocol is supported.
- **SubRecord**: Record signals from devices using the CC1101 module and save them to an SD card.
- **Jammer**: Jam selected frequencies.
- **Monitor**: Graphically display the received signal.

### WiFi Menu
- **Wardriving**: Collect information about networks and save them to an SD card.

### Bluetooth Menu
- **Skim check**: Check for the presence of credit card skimmers nearby.

### Settings Menu
- **Set freq**: Set the frequency for the SubRecord, Monitor, and Jammer programs.

## What Do You Need

- CC1101 module ([link here](#))
- Small version of micro SD card module ([link here](#))
- Double Sided Prototype Board, I am using a 3x7cm one ([link here](#))
- Soldering iron and some soldering skills

You can try to connect everything with cables, but it's better to solder it all nicely.

## Pinout

Below is the pinout diagram needed for the modules:

![Pinout Diagram](images/pinout.jpg)

| M5stickcplus2      | CC1101 | SD card module |
|--------------------|--------|----------------|
| GND                | GND    | GND            |
| G26                | CSN    | MOSI           |
| G36/G25            | GDO0   | MISO           |
| G0                 | SCK    | CLK            |
| 3v3                | Vcc    | 3v3            |
| G32 (bottom pin)   | MOSI   | -              |
| G33 (bottom pin)   | MISO   | -              |

## Installation and Setup

1. Download and upload the firmware from M5Burner.
2. Download this repository and unpack the Subfiles.zip to your SD card.
3. Insert the SD card into the module and you're done.

---

Feel free to reach out with any questions or suggestions!

**Contact**: stachu0 on Discord.


## Disclaimer

This software is intended for educational and research purposes only. The author is not responsible for any misuse of this software. Use it responsibly and in compliance with all applicable laws and regulations.
