# OpenBCI Toolkit for LabVIEW

**OpenBCI** stands for open-source brain-computer interface (BCI). The **OpenBCI Cyton** board is a versatile and affordable analog-to-digital converter (Texas Instrument’s ADS1299) that can be used to sample electrical brain activity (EEG), muscle activity (EMG), heart rate (ECG), and more. It is compatible with any type of electrode and is supported by an ever-growing, open-source framework of signal processing applications. http://openbci.com/

This Toolkit Communication between the **OpenBCI Cyton** board and the computer is wireless and is carried on by the OpenBCI DONGLE.

This toolkit handles the communication with the **OpenBCI Cyton** board and the **OpenBCI DONGLE**, by implementing the [OpenBCI communication protocol](http://docs.openbci.com/OpenBCI%20Software/04-OpenBCI_Cyton_SDK) in LabVIEW, to write (configuration) and read (configuration, raw EEG data and acceleration data) from the **OpenBCI Cyton** board. There are two hardware versions for the board: 8bit (based on ATmega328P) and 32 bits (based on PIC32MX250F128B); both versions possess 8 channels than can be extended to 16 channels using the [OpenBCI Daisy Module](http://docs.openbci.com/Hardware/02-Cyton#openbci-cyton-openbci-daisy-module).

This toolkit (v 1.1.2) has been tested in the 8bit and 32bit versions with 8 and 16 channels.

## Installation
To install the **BLE Toolkit for LabVIEW**, the **VI Package Manager 2017** by [JKI](http://jki.net/) is needed.
1. Download and install [VI Package Manager](https://vipm.jki.net/get)
2. Download and install the last VI package for the **OpenBCI Toolkit for LabVIEW** from https://github.com/rcassani/OpenBCI-Toolkit-LabVIEW/releases

## Preparation
Follow the steps provided in the [Cyton getting started guide](http://docs.openbci.com/Tutorials/01-Cyton_Getting%20Started_Guide) to assure your board and dongle are working properly, identify the number of the **COM port** that is used.

## Example
One example: `simple_continous_read.vi` is provided with the **OpenBCI Toolkit for LabVIEW**. The
example is located in: `<LabVIEW>\examples\OpenBCI\Examples\ble_scan_devices.vi`

being `<LabVIEW>` your LabVIEW folder, for example `C:\Program Files (x86)\National Instruments\LabVIEW 2013`


![alt text](https://user-images.githubusercontent.com/8238803/38782839-7b3000a8-40c7-11e8-939e-0f24bfb2b4e5.png)
`simple_continous_read.vi` Front Panel

## Creating VI Package file
Alternatively, the files in this repository can be used to build the VI Package for the **OpenBCI Toolkit for LabVIEW**.
