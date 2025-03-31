# ESP01LEDDriver: a board for attaching an ESP01 to an addressable LED strip

![ESP01LEDDriver PCB](/images/ESP01LEDDriver.png)

A [schematic](ESP01LEDDriver.pdf) is included here, along with the
[KiCAD](https://www.kicad.org) data files, whcih are in KiCAD 6 format.

## PCB design

The PCB is a trivial 2 layer board.

## Using

After coming across the
[ESP01](https://www.instructables.com/Getting-Started-With-the-ESP8266-ESP-01/)
I was very impressed. It seemed like an excellent solution to problems where a
very small controller board was needed, such as running
[WLED](https://kno.wled.ge) to control addressable LED strips. However the LED
strip attachment board I could find used an odd arrangement of receiving power
by attaching a USB-A plug directly to the board. I wanted to use a power lead of
some description, going to the controller board which then had the LED strip
screwed into it on terminals. As I was ordering some other boards, I thought I
would knock up this board and order it at the same time.

Power can be supplied via 5V on the barell plug, or 5V via a USB-B connector.
The [FTDI
FT231XS](https://ftdichip.com/wp-content/uploads/2021/10/DS_FT231X.pdf) is
optional: if included on the board then it is possible to program the ESP01
in-place via the USB connection. Otherwise it must either be programmed using a
dedicated board, or programmed when attached to this board but via a USB TTL (in
3.3V mode!) UART attached to the four header pins.

In either case, the PROGRAM button can be used to bring up the ESP01 in
programming mode.

## TODO

When time allows I will CAD-up a small printable case for enclosing this board.
