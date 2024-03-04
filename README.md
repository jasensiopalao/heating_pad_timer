# Introduction

This project was started to replace the controller in a USB heating pad rated at a maximum of 10W but in practice delivering 7W.

The main motivation behind replacing the original controller was to provide a system that would not easily reset if the USB is unplugged, which caused the original device to switch off. Additionally the original controller had a maximum timeout of 1.5 hours, which was not enogh.

With the new controller the advantages are:
* Simple ON/OFF, no need to press multiple times to select duty cycles or different timeouts.
* Fixed timeout on 3.2 hours
* Timer does not reset even if USB is unplugged

# Design considerations

* Simple timer design using a capacitor and resistance to discharge
* Use of a MOSFET to efficently drive the heating pad.

# Schematics

![](schematics/heating_pad_protection.svg)

