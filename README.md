# CatHack Firmware for M5StickCPlus2
![CatHack Logo](images/cathack.png)
CatHack is a powerful and versatile firmware designed for the M5StickCPlus2, offering a comprehensive suite of tools for infrared, SubGhz, WiFi, and Bluetooth operations. This firmware transforms your M5StickCPlus2 into a multi-functional hacking device, perfect for security researchers, hobbyists, and tech enthusiasts.

## 📸 Device Setup
<div style="display: flex; justify-content: space-around;">
  <img src="images/PXL_20240721_174404806.MV.jpg" width="45%" alt="CatHack Device Setup">
  <img src="images/res.jpg" width="45%" alt="CatHack Result">
</div>

Check out the [3D model of my setup](https://www.tinkercad.com/things/jRt2EwITRLK-cathack?sharecode=Apvaz9IlzPh7Pgl7gSoIbn_yxP5yHBEyyqrAIA4JWxM) for a detailed view!

## 🚀 Features
### 📺 Infrared Menu
- **TVBGone**: Turn off all nearby televisions with a single click.

### 📡 SubGhz Menu
- **SubSend**: Transmit .sub files from Flipper Zero using the CC1101 module (currently supports RAW protocol).
- **SubRecord**: Capture signals from devices using the CC1101 module and save them to an SD card.
- **Jammer**: Disrupt selected frequencies.
- **Monitor**: Visualize received signals in real-time.

### 🌐 WiFi Menu
- **Wardriving**: Collect and log information about nearby networks.

### 🦷 Bluetooth Menu
- **Skim Check**: Detect potential credit card skimmers in your vicinity.

### ⚙️ Settings Menu
- **Set Frequency**: Configure the frequency for SubRecord, Monitor, and Jammer functionalities.


## 🐬 Flipper Zero Compatibility
CatHack supports .sub files with RAW protocol from Flipper Zero. All necessary files, including compatible Flipper Zero files, are included in the subfiles.zip package. Simply download and extract these files to your SD card to use them with CatHack.


<img src="images/files.png" width="30%" alt="">

## 🔮 Planned Future Features
- **IR Send**: Send recorded IR codes or codes from Flipper Zero.
- **IR Record**: Record IR codes.
- **Deauther**: WiFi deauthentication tool.
- **Bad Portal**: Create fake login pages for security testing.
- **BLE Spam**: Spam advertising packets over Bluetooth Low Energy.
- **Web Interface**: Network interface for adding/removing files.
- **NFC/RFID Read**: Read NFC/RFID tags and save data to SD card.
- **NFC/RFID Emulate**: Emulate NFC/RFID tags using saved data.

## 🛠️ Required Components
- Curved pin headers
  ![Curved Pin Headers](images/M50-3930642_SPL.webp)
- CC1101 module
  <img src="images/original.jpg" width="150" alt="CC1101 Module">
- Compact micro SD card module
  <img src="images/the-mini-sd-card-module-micro-sd-card-module.jpg" width="150" alt="SD Card Module">
- Double-Sided Prototype Board (3x7cm recommended)
  <img src="images/ct09300-02-thumbnail-1080x1080-70.jpg" width="150" alt="Prototype Board">
- Soldering iron and proficiency in soldering

While it's possible to connect components using cables, soldering is recommended for a more reliable and compact setup.

## 📊 Pinout Diagram
![Pinout Diagram](images/pinout.jpg)

| M5StickCPlus2      | CC1101 | SD Card Module |
|:------------------:|:------:|:--------------:|
| GND                | GND    | GND and CS     |
| G26                | CSN    | MOSI           |
| G36/G25            | GDO0   | MISO           |
| G0                 | SCK    | CLK            |
| 3v3                | Vcc    | 3v3            |
| G32 (bottom pin)   | MOSI   | -              |
| G33 (bottom pin)   | MISO   | -              |

⚠️Remember to connect CS to GND on the SD card module, otherwise it will not work⚠️

## 📥 Installation Guide
1. Download and flash the firmware using M5Burner.
2. Download the [Subfiles.zip](https://drive.google.com/file/d/1TZCD_Jr_Pu78nF93ItqeqHZLEuuWagby/view?usp=sharing) and extract its contents to your SD card.
   ⚠️ Note: Some files may not be compatible as only the RAW protocol is currently supported. ⚠️
3. Insert the SD card into the module, and you're ready to go!


## How i did it
<img src="images/1.jpg" width="45%" alt="">
<img src="images/2.jpg" width="45%" alt="">
<img src="images/3.jpg" width="45%" alt="">
<img src="images/4.jpg" width="45%" alt="">

## 📞 Support
If you have any questions or suggestions, feel free to reach out:
- Discord: stachu0

## ⚠️ Disclaimer
This software is intended for educational and research purposes only. The author bears no responsibility for any misuse of this software. Use it responsibly and in compliance with all applicable laws and regulations.

---
🐱 Happy Hacking with CatHack! 🐱
