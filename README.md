# Open Microscropy and AI Workshop

In this repository, you will find the materials for the [Open Microscopy and AI Workshop](https://www.epfl-open-microscopy.com/) at EPFL.

Content:
- [Build our own fluorescence microscope with OpenUC2](#build-our-own-fluorescence-microscope-with-openuc2)
- [Build your deconvolution algorithm with Pyxu](#build-your-deconvolution-algorithm-with-pyxu)
- [Build your deep-learning analysis pipeline with deepImageJ & SAMJ](#build-your-deep-learning-analysis-pipeline-with-deepimagej--samj)


## Build our own fluorescence microscope with OpenUC2

Our goal is to replicate [this experiment](https://openuc2.github.io/docs/Toolboxes/DiscoveryFluorescence/LED_Fluoresence_microscope/) (LED-Powered Fluorescence Microscope).

TODO
- Flashing and testing LED matrix
- Using ImSwitch to control the microscope


### 1) Installing the Raspberry Pi (done prior to workshop)

We will be using a Raspberry Pi to control the microscope. We first need to flash (i.e. install) the Raspberry Pi with the software that will allow us to control the microscope. You can follow [these instructions](https://openuc2.github.io/docs/ImSwitch/ImSwitchOnRaspi/#how-to-use-the-pre-built-image) to flash the Raspberry Pi.

After flashing the SD card, insert it into the Raspberry Pi and for a bit for the Raspberry Pi to boot up (green LED should be stable). You should be a new WiFi network called `openuc2-unknown` that you can connect to. The password is `copepode`. 

You can test the connection to ImSwitch for interactive with the microscope, as described [here](https://openuc2.github.io/docs/ImSwitch/ImSwitchOnRaspi/#connecting-to-the-raspberry-pi).

### 2) Installing the Electronics (done prior to workshop)

**Caution! If you need to change any of the cables or their position, always unplug the 12V power cable before doing so. Otherwise, the electronic components might get damaged!**

We now need to flash the firmware for:

1. The ESP32 DEV-based UC2 standalone board
2. The LED matrix

These steps are described [here](https://openuc2.github.io/docs/Toolboxes/DiscoveryFluorescence/LED_Fluoresence_microscope/#22-flashing-the-esp32-firmware).



### 3) Testing the Electronics (optional)

With the electronics connected to **your laptop**, you can test the electronics from [this page](https://youseetoo.github.io/indexWebSerialTest.html) (note you should use Chrome or Edge):
- Laser 2 for Blue LED
- Motor control, Z stage

### 4) Assembling the Microscope

We can now assemble the microscope! These steps are laid out [here](https://openuc2.github.io/docs/Toolboxes/DiscoveryFluorescence/LED_Fluoresence_microscope/#step-1-assemble-the-microscope).

### 5) Using ImSwitch for remote control

Let's try to control the microscope remotely using ImSwitch. You can connect to the Raspberry Pi by first joining the network `openuc2-epfl-X` with password `copepode`. Then, open a browser and go to [https://192.168.4.1:8001/imswitch/index.html](https://192.168.4.1:8001/imswitch/index.html).

---

## Build your deconvolution algorithm with Pyxu

TODO

---
## Build your deep-learning analysis pipeline with deepImageJ & SAMJ

See here: https://github.com/deepimagej/Workshop-materials/tree/main/OpenMicroscopyEPFL-2025