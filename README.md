# Model M Type C
This is a project with the simple goal of recreating the old IBM Model M keyboard controller with modern technologies in mind.

![Board Render](images/render.png)

## Motivation
Although the IBM Model M is perhaps the most well-known and popular of old keyboards, it isn't equipped with some modern ameneties we have grown used to enjoying. Key features that the Model M lacks are Windows and Media keys(or, broader, firmware-level repogramability), as well as a hotswappable connection with a modern interface. This controller is designed to bring 21st century features to a 20th century keyboard.

## Goals
- Native USB C
- Hotswappable
- Fully configurable with QMK compatibility
- Less power draw
- Complete reversability

## Usage
1. Print the board either using a cheap foreign service such as [JLCPBC](https://jlcpcb.com/ "JLCPBC") for around $6 + shipping, or a domestic service such as [OSH Park](https://oshpark.com/ "OSH Park") for around $35.
2. Order the components- [part list](https://www.digikey.com/short/p00t8f "part list") from Digikey. USB C port needs to be bought elsewhere, I recommend [here](https://keeb.io/products/usb-c-port-12-pin-hro-type-c-31-m-12 "here").  $15 total for components. If your LEDs connect via a ribbon, get [this](https://www.digikey.com/short/p012jt "this") instead of the JST 4 pin connector.
3. Put it together. It's possible to solder these SMD components manually with a soldering iron, but if you are able to find a hot air gun or a reflow oven, it'll be significantly easier. Reference the visual BOM to see what goes where.
4. Install firmware.

## Firmware
This board is fully compatible with QMK. Use [this fork](https://github.com/ashpil/qmk_firmware/tree/master/keyboards/ashpil/modelm_usbc "this fork") of QMK with configured ashpil/modelm_usbc keyboard for this controller.

## TODO
Create 3D print to allow for fully-native appearance and detachable cable.