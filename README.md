# Voron V0.1 Tophat LED Mounts

![Assembled Tophat](Images/Assembly_2.jpg?raw=true)

This mod for the Voron V0.1 adds four (4) LED mounting bars to the tophat and is designed to be minimumally intrusive and simple to build. It supports up to thirty (30) LEDs, which is the maximum officially supported using the BigTreeTech SKR Mini E3 V2 5-volt breakout board.

## Table of Contents
- [Bill of Materials](#bill-of-materials)
- [Recommended Tools](#recommended-tools)
- [Printed Parts](#printed-parts)
- [Assembly Instructions](#assembly-instructions)
- [Klipper Configuration](#klipper-configuration)
- [Photos](#photos)

## Bill of Materials

The following parts are required (unless otherwise denoted) to complete the assembly:

| Part | Quantity | Link | Alternate Link | Notes |
| --- | :-: | --- | --- | --- |
| BigTreeTech DCDC5V Power Module | 1 | https://www.biqu.equipment/products/bigtreetech-dcdc5v-v1-0-power-module-5v-for-skr-mini-e3-v1-2-skr-mini-e3-v3-0-32bit-control-board-rgb-light | | Required to run up to 30 total LEDs, otherwise the SKR Mini only supports up to 8 LEDs. |
| WS2812B RGB IP65 5v LED Strip | 16.4 ft., 300 LEDs (OR) 3.2 f.t, 60 LEDs | https://amzn.to/3l4htHR | | Channels in mounting bars are designed to fit this exact 10mm-wide LED strip. Any LED strip you use should be 5 volts, 10mm wide, individually addressable, and approximately 16.5mm in length or less per LED diode. |
| 3-Pin 18 AWG PVC Copper Ribbon Wiring | 3+ ft. | https://amzn.to/3nSPr4d | | 3-pin ribbon wiring is easier to work with for this mod, but any wiring will work. The reviews for the linked part suggest this wiring may actually be 20 AWG, but that is probably preferred anyway. |
| 1/4" Diameter Heat Shrink Tubing | 7 | https://amzn.to/3HMqvTM | | Heat shrink tubing will protect the solder joints on the LED wiring pads (otherwise the pads may rip off during assembly). Cut 7 pieces to about 1/2" long each. |
| JST-XH 2.54mm 3-Pin Female Connector | 1 | https://amzn.to/30Vttoj | | A JST-XH or similar 2.54mm connector is required to plug the LED strips into the Neopixel pins on the SKR Mini E3 V2 board. |
| Molex Micro-Fit 3.0 3-Pin Male/Female Connectors | 1 each | https://amzn.to/3FLt3zN | | **Optional** Added in-line within the printer chamber to allow for quick disconnects when removing the tophat for maintenance. |
| M3x10 Button Head Cap Screws | 8 | https://amzn.to/3HGdOd0 | https://www.boltdepot.com/Product-Details.aspx?product=22819 | These will replace the 8x M3x6 screws used to bolt the tophat center clips to the tophat frame. |

## Recommended Tools

The following tools are recommended, but not required, in order to complete the assembly:

| Tool | Link | Notes |
| --- | --- | --- |
| 3D Printer with >= 200mm Bed | | The largest part is about 185mm long, and you are encouraged to use a brim which increases the length. ***No, the LED mounting bars will not fit on a Voron V0 bed.*** |
| Wire Strippers | https://amzn.to/3HNQ86u | For cutting and stripping wires between the LED strips. |
| Crimping Pliers | https://amzn.to/3cIcCry | For crimping JST-XH connector and other terminals. |
| Soldering Iron | https://amzn.to/3CNMZjv | You will need to solder 21 joints, plus maybe another 9 joints once you realize that once again you forgot to slide on the heat shrink tubing before soldering. |
| Tin Lead Rosin Core Solder Wire | https://amzn.to/30PILdR | |
| 2mm Hex Driver | | |

## Printed Parts

Each of the following parts should be printed in either ABS or ASA. You will need a 3D printer with a bed that is at least 200mm wide to print the LED mounting bars. ***No, the LED mounting bars will not fit on a Voron V0 bed.*** Print each of the LED mounting bars with supports under the center of each bar where it will mount to the tophat center clip.

| Part | Quantity | LED Angle | Supports Needed |
| --- | :-: | --- | --- |
| Front LED Bar | 1 | 15 degrees | Yes|
| Side LED Bar | 2 | 15 degrees | Yes |
| Back LED Bar | 1 | 5 degrees | Yes |
| End Clip | 8 | | No |

## Assembly Instructions

1. Print each of the [printed parts](#printed-parts).
2. Remove the existing M3x6 button head cap screws from the tophat center clips and install the front, back, and side LED mounting bars over the center clips using M3x10 button head cap screws. Each of the mounting bars is angled to better direct light toward the build plate. Ensure that the LED mounting bars are installed in the orientation that will direct light downward rather than upward.
3. Cut two (2) strips of seven (7) LEDs for the front and back and two (2) strips of eight (8) LEDs for the sides. I recommend leaving the full contact pad length on each side of a strip rather than cutting the contact pad in half. This means that for each two (2) strips of LEDs you cut, you will throw away the LED diode between them because it won't have any contact pads. This will give you the greatest amount of surface area to ensure your soldering joints are strong.
4. Gently insert a seven (7) LED strip and an eight (8) LED strip into adjacent mounting bars to ensure that they will fit and measure the amount of 3-pin wire you will need between them. You will need somewhere around 3.5" of wire at each corner. Remove the strips from the mounting bars.
5. Cut off only the portion of IP65 plastic protective covering the contact pads on each end of the LED strips, except that you should not cut off the covering on the last set of contacts on the last LED strip since it will not be used. I have found the best way to do this is to peel away the covering from the LED strip by hand just enough to fully expose the contact pads and cut the covering with wire strippers.
6. Solder all the LED strips together with a strand of the measured 3-pin wire between each of them. ***Be sure to add heat shrink tubing to your wires for each of your solder joints.***
7. Measure the length of wire needed to connect your first LED strip to the controller board and then cut and solder it to the first LED strip. If using an SKR Mini E2 V2, crimp and add the JST-XH connector at the other end.
8. Slide the heat shrink tubing over the solder joints on each LED strip and apply heat to shrink them. Do not overheat or they will split and fall off.
9. Install each LED strip into its appropriate mounting bar by firmly pressing until it catches. You should not need to use the adhesive backing. Firmly press the wiring on each end of the LED strip into the mounting bar wiring channels.
10. Install the end clips on the ends of each mounting bar. The snap-fit connections are a bit oversized to ensure they strongly hold the wiring in place, so you may need to press firmly and/or twist the clips to install them properly.
11. Install the BigTreeTech DCDC5V Power Module onto the SKR Mini E3 V2 controller board. Be sure to move the appropriate jumper on the SKR Mini to ensure it uses the power module rather than the on-board 5v controller for Neopixel power (this is what allows you to use up to 30 LEDs rather than only 8). Consult the power module documentation for details.
12. Connect the JST-XH connector to the Neopixel port on the SKR Mini E3 V2.
13. Following the directions below for setting up the LEDs in the Klipper `printer.cfg` configuration file.

## Klipper Configuration

Add the following to `printer.cfg` in Klipper if using RGB LEDs:

```
###################################
# Neopixels / LEDs
###################################
[neopixel my_neopixel]
pin: PA8
chain_count: 30
color_order: GRB
initial_RED: 0.02
initial_GREEN: 0
initial_BLUE: 0.05
```

The LEDs can be changed by sending the command `SET_LED LED=my_neopixel RED={x} GREEN={x} BLUE={x}`, where `{x}` is a decimal value between 0 and 1. Consult the [Klipper documentation](https://www.klipper3d.org/Config_Reference.html#neopixel) for more information and configuration options.

## Photos

![Wiring 1](Images/Wiring_1.jpg?raw=true)
![Wiring ](Images/Wiring_2.jpg?raw=true)
![Assembly 1](Images/Assembly_1.jpg?raw=true)
![Assembly 2](Images/Assembly_2.jpg?raw=true)
![Wiring 3](Images/Wiring_3.jpg?raw=true)
![Overview 1](Images/Overview_1.jpg?raw=true)
![Overview 2](Images/Overview_2.jpg?raw=true)
![Overview 3](Images/Overview_3.jpg?raw=true)
![Overview 4](Images/Overview_4.jpg?raw=true)
