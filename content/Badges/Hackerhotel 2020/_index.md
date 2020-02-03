---
title: "Hackerhotel 2020"
nodateline: true
weight: 10
---

![badge](hackerhotel2020.gif)

## The project

Welcome to Hackerhotel 2020, where you may check-out any time you want but you may never leave...

...just kidding of course, but our Egyptian cat goddess badge will be watching over you both during and after the event.

This badge is a bit different from our other badges: it's a challenge badge. No apps, no Python, but instead a story for you to experience filled with puzzles and lore!

The Hackerhotel 2020 badge is a mixed reality escape room. Reminiscent of the classic 'text adventures' but with interactions in the real world, it will present you with many challenges to overcome in both the virtual and the real hotel. 

## Getting started

Did you just receive your badge at the event? Great! Plug in the batteries and you can start playing the minigames on the badge right away. There are four buttons on the front of the device using which you can control the games. Good luck figuring out how it works, as we're leaving that part as a little secret!

{{% notice warning %}}
Before plugigng in shitty addons please read the notes mentioned in the Errata section of this page!
{{% /notice %}}

## Playing the game

To play the "escape from Hackerhotel" challenge you need to connect your badge to a computer. You can do this by connecting a USB-serial converter with 3.3 volt signal levels to the GND, RX and TX pins of the shitty-addon (SAO) connector. The TX pin is the pin transmitting data to your computer, the RX pin is for sending data from your computer to the badge.

The badge will present you with a text entry prompt when you connect to it using a terminal emulator configured for 115200 baud, 8-bit data width, no pairity bit and 1 stop-bit (115200 8n1).

### Installing a terminal emulator
  - [On Linux](connecting-linux)
  - [On Windows 7, 8 and 10](connecting-windows)
  - [On Apple OS X](connecting-mac)

## Errata
Some mistakes were made both in the design and during assembly, which we couldn't fix in time for the event. The SAO (shitty add-on) connector has been placed on the bottom of the badge, while it was intended to be placed on the top side. This means that the pinout of the SAO connector is mirrored when compared to the SAO specifications. The pinout mentioned on the silkscreen of your badge does properly match the connector, so no worries there. Should you want to plug in a shitty-addon then you will have to replace the connector.

At the badge assembly, both during Hackerhotel 2020 and during future events where we attend we will be sure to take some extra SAO connectors with us, together with the necessary equipment for doing this small rework step.

Other mistakes are more visible, but less obvious: we've mirrored the pinout of the LEDs on this badge. To work around this issue we've removed the N-mosfets used to drive the LED-matrix and replaced them with bodgewires. To get the most light intensity out of your badge and to restore your badge to it's full potential you can flip the leds (they're symmetric), solder the N-mosfets back in place and re-flash the firmware to drive the LED-matrix the right way round. Doing this rework takes a lot of time (30 minutes or more), but we're glad to be of assistance should you want to attempt this.

You can find a manual for fully reworking your badge [here](rework-manual).








 