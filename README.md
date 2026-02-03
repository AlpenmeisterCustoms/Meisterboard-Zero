# Meisterboard-Zero
a gaming controller focussed RP2040 micro breakout board

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

<img width="400" height="400" alt="meisterboard-zero" src="https://github.com/user-attachments/assets/cfa381f9-2c85-41a4-aca5-a8509badc839" />
<img width="400" height="400" alt="meisterboard-zero" src="https://github.com/user-attachments/assets/1b3efd9c-8270-4537-a673-c0b01cf654ad" />

## License

This design is licensed under the [OPEN COMMUNITY LICENSE](https://github.com/OpenCommunityLicence/OpenCommunityLicence). In short:  you can use, modify and build it for non-commercial use. You can use, modify and build it for internal commercial use. You may NOT modify, build and sell it without my permission. I will grant this permission without any costs, I just want to know who is building and selling it and make an official list here.
