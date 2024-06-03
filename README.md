# Howto add USB data  support to the Miyoo Mini +

The Miyoo Mini + has a USB-C port but its only goal is to charge the battery. This hardware mod will let you use your USB-C port to plug any USB device to your console (joysticks, keyboard, mouse, bluetooth dongle etc.)

## 1. Connect the SoC's USB data pin to your USB-C port
As we can see in the datasheet, pins 111 and 112 are respectively DM_P2 and DP_P2 (second port's USB differential pair).

![SoC pins](https://github.com/1arthur1/MiyooMini-USB-Support/blob/master/images/SoC.png?raw=true)

Below, we can see a the footprint of the SoC on the PCB. This second port is not used, no track nor vias are visible.

![SoC footprint](https://github.com/1arthur1/MiyooMini-USB-Support/blob/master/images/SoC_PCB.png?raw=true)

Below an example of the result:

![SoC solder side](https://github.com/1arthur1/MiyooMini-USB-Support/blob/master/images/SoC_Connection.png?raw=true)
![USB-C solder side](https://github.com/1arthur1/MiyooMini-USB-Support/blob/master/images/USB_C_Connection.png?raw=true)

## Useful information
[SoC Datasheet](https://eaw.app/Downloads/SSD202D_Reference_v04.pdf)

[Adding UART tutorial](https://apuntes.eduardofilo.es/en/2022-08-08_mmiyoo_uart.html)

[HD pictures of the PCB](https://discord.com/channels/529983248114122762/1004510206098681968/1144256851307925575)
