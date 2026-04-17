# Meisterboard-Zero
a gaming controller focussed RP2040 micro breakout board for the GP2040-CE firmware

<img width="400" height="900" alt="meisterboard-zero front" src="https://github.com/user-attachments/assets/f311391f-1b10-4405-89c1-f342dad86785" />
<img width="400" height="400" alt="meisterboard-zero back" src="https://github.com/user-attachments/assets/b6fa2b68-b9fb-467c-9643-78f695e89ae9" />


## Introduction / goals
I was in need of a cost effective breakout board to use for rapid prototyping and to make iterating controller builds faster and more flexible. The goal was to reduce PCB assembly service costs and time and have a somewhat easy to solder breakout board available with all the necessary features present. That way one could quickly build on basic (even locally produced) PCBs without the need to embed and assemble the whole RP2040 design.

<img width="400" height="400" alt="meisterboard-zero vs waveshare zero" src="https://github.com/user-attachments/assets/346ca02b-1036-4476-95db-979c0776a11d" />
<img width="400" height="400" alt="meisterboard-zero vs waveshare zero size" src="https://github.com/user-attachments/assets/574aa9f5-1e4c-47ac-937f-6d52b6fcbcd1" />

## Design considerations
The Waveshare Zero is a popular RP2040 based board to use as the central piece of GP2040-CE firmware based controller builds. While it is great because of its extremely small size and universal utility, it does not expose all available GPIOs in an easily accessible way and is not tailored for controller building. I therefore used its size as a benchmark and reference to aim for and added features I considered essential or useful:
* All configurable GPIOs exposed via holes for pin headers and castellated holes for easier soldering.
* All essential components are only on the top side of the board; the whole bottom side can and in most cases should be left unpopulated (only optional connectors present) to make production even more affordable
* Dedicated onboard bootsel, reset and webconfig button.
* Comes with a USB-A host daughter board, to be detached with wire cutters. 
* Modular design makes it possible to also detach the main USB-C port.
* Both USB-A and USB-C daughter boards can be either soldered to a PCB or connected via JST SH 2.0 wires. The mother board has corresponding connectors in place.

<img width="400" height="400" alt="meisterboard-zero wired front" src="https://github.com/user-attachments/assets/0fd140d7-df9d-4137-9748-6dee1742daf3" />
<img width="400" height="400" alt="meisterboard-zero wired back" src="https://github.com/user-attachments/assets/a2f08034-a147-41db-9140-348a086c8b32" />

## Advantages

* Smallest possible size, while all GPIOs accessible via pins or castellated holes.
* USB-C port easily and cheaply replaceable in case it ever fails from plugging and unplugging cables.
* Comes with a detachable USB-A host daughter board.
* Modular design makes it useful for various controller builds, including flatbox style controllers, very small builds or those that need flexible placement of the USB-C and USB-A ports.
* Cheaper to produce and ship than having full size boards with embedded components, especially considering the current unpredictable global tariff regime.
* To make production more affordable, all essential components are placed on only one side. If you need to further cut costs, just don't populate the bottom side with the connectors.
* Costs only about 5-10€ incl. VAT and shipping built in a batch of 50 boards, depending on fab.

<img width="400" height="900" alt="meisterboard-zero with USB host front" src="https://github.com/user-attachments/assets/927df3fa-3640-468d-b14f-dad79b8ebe6d" />
<img width="400" height="900" alt="meisterboard-zero with USB host back" src="https://github.com/user-attachments/assets/d77f4d4c-0eac-4212-89e7-09342ec8c727" />


## License

This design is licensed under the [OPEN COMMUNITY LICENSE](https://github.com/OpenCommunityLicence/OpenCommunityLicence). In short:  you can use, modify and build it for non-commercial use. You can use, modify and build it for internal commercial use. You must NOT modify, build and sell it without my permission. I will grant this permission without any costs to whoever requests it, I just want to know who is building and selling it and make an official list here.  
Deviating from the Open Community License, you may build this board and use it as an internal component for your commercial product. In that case you do not need to formally request permission, but I would want to be informed ([contact via my website](https://alpenmeister.com/en)), so I can list the devices using it. 

## Where to buy

Devices using it:
* [Alpenmeister M](https://alpenmeister.com/en/products/meisterbox-m)

## How to build

1. Choose your favorite fab. I recommend JLCPCB (very automated and streamlined process) or PCBWay (more involved but better guided process). Pricing for both is about the same for an order of 50 boards.

3. Upload the gerber files and go through the ordering process. Make sure to check "castellated holes" and "confirm production files" in the JLC order form. 
4. Check if all components are in stock and placed correctly.

## How to use:
1. When the assembled boards arrive, use a wire cutter to remove the USB-A piece.
2. Solder all the pieces to your board and/or screw them in place and connect them with JST SH 2.0 connection wires if needed.
3. Connect to a PC via USB-C. Hold bootsel switch and push the reset switch. The board should get mounted as a drive. Copy [the firmware](https://github.com/AlpenmeisterCustoms/GP2040-CE/releases/) to that drive to flash it.
4. Please refer to the [GP2040-CE project](https://gp2040-ce.info/) for further software documentation.

## Disclaimer:

Build and use at at your own risk. These files are provided as is. It is your own duty to make sure the boards work as intended. 
