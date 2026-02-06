# Meisterboard-Zero
a gaming controller focussed RP2040 micro breakout board for the GP2040-CE firmware

<img width="400" height="400" alt="meisterboard-zero" src="https://github.com/user-attachments/assets/d9addb99-6070-4b7b-a13a-daf50d6e1c14" />
<img width="400" height="400" alt="meisterboard-zero" src="https://github.com/user-attachments/assets/20c26017-1fdb-43f6-93d4-e6d26236c3d3" />



## Introduction / goals
I was in need of a cost effective breakout board to use for rapid prototyping and iterating controller builds. The goal was to reduce PCB assembly service/time and have an easy to solder base/controller board available with all the necessary features present. That way one could quickly build on basic (locally produced) PCBs without the need to embed and assemble the whole RP2040 design.

*Picture disclaimer: They are showing a version without castellated holes on the USB-C and USB-A breakoff pieces. Also silkscreen adjustments were made.*

## Design considerations
The Waveshare Zero is a popular RP2040 based board to use as the central piece of GP2040-CE firmware based controller builds. While it is great because of its extremely small size and universal utility, it does not easily expose all available GPIOs and is not tailored for controller building. I therefore used its size as an (unattainable) goal/reference and added features I considered useful:
* All configurable GPIOs exposed via castellated holes for easy soldering. Optional holes for pin headers.
* Dedicated onboard bootsel, reset and webconfig button.
* Comes with a USB-A host breakout board, to be detached with wire cutters. 
* Modular design makes it possible to also detach the main USB-C port.
* Both USB-A and USB-C breakout boards can be either soldered to a PCB or connected via JST SH 2.0 wires. The main board has corresponding connectors in place.

<img width="400" height="400" alt="meisterboard-zero" src="https://github.com/user-attachments/assets/94d9ef30-2681-4ac7-ae23-ea711d4a513d" />
<img width="400" height="400" alt="meisterboard-zero" src="https://github.com/user-attachments/assets/c2f2d63e-6320-4312-8659-74c0d27542dc" />

## Advantages

* Smallest possible size, while all GPIOs are easily accessible.
* USB-C port easily and cheaply replaceable in case it ever fails from plugging and unplugging cables.
* Comes with a USB-A host breakout board.
* Modular design makes it useful for various controller builds, including flatbox style controllers, very small builds or those that need flexible placement of the USB-C and USB-A ports.
* Cheaper to produce and ship than having full size boards with embedded components, especially considering the current unpredictable global tariff regime.
* To make production cheaper, just do not populate some components, like the connectors or ports.
* Costs only 5-10€ incl. VAT and shipping built in a batch of 50 boards.

<img width="400" height="400" alt="meisterboard-zero" src="https://github.com/user-attachments/assets/cfa381f9-2c85-41a4-aca5-a8509badc839" />
<img width="400" height="400" alt="meisterboard-zero" src="https://github.com/user-attachments/assets/d4093e6c-8bef-4b90-bfe1-352fa782a909" />

## License

This design is licensed under the [OPEN COMMUNITY LICENSE](https://github.com/OpenCommunityLicence/OpenCommunityLicence). In short:  you can use, modify and build it for non-commercial use. You can use, modify and build it for internal commercial use. You must NOT modify, build and sell it without my permission. I will grant this permission without any costs, I just want to know who is building and selling it and make an official list here.  
Deviating from the OCL, you may build this board and use it as an internal component for your commercial product.

## Where to buy

List of recommended/known sellers:
* --

List of other sellers:
* --

## How to build

1. Choose your favorite fab. I recommend JLCPCB (very automated and streamlined process) or PCBWay (more involved but better guided process). Pricing for both is about the same for an order of 50 boards.
2. Upload the gerber files and go through ordering process. Make sure to check "castellated holes" and "confirm production files" in the JLC order form. 
3. Check if all components are in stock and placed correctly.

## How to use:
1. When the assembled boards arrive, use a wire cutter to remove the USB-A piece.
2. Solder all the pieces to your board and/or screw them in place and connect them with JST SH 2.0 connection wires if needed.
3. Connect to a PC via USB-C. Hold bootsel switch and push the reset switch. The board should get mounted as a drive. Copy the firmware to that drive to flash it.
4. Please refer to the [GP2040-CE project](https://gp2040-ce.info/) for further software documentation.

## Disclaimer:

Build and use at at your own risk. These files are provided as is. It is your own duty to make sure the boards work as you intend it. 
