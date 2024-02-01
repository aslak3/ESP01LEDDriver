# ESP01LEDDriver: a board for attaching an ESP01 to an addressable LED strip

![ESP01LEDDriver PCB](/images/ESP01LEDDriver.png)

A [schematic](ESP01LEDDriver.pdf) is included here, along with the [KiCAD](https://www.kicad.org)
data files, whcih are in KiCAD 6 format.

## PCB design

The PCB is a trivial 2 layer board. 

## Using

After coming across the
[ESP01](https://www.instructables.com/Getting-Started-With-the-ESP8266-ESP-01/)
I was very impressed. It seemed like an excellent solution to problems where
a very small controller board was needed, such as running
[WLED](https://kno.wled.ge) to control addressable LED strips. However the LED
strip attachment board I could find used an odd arrangement of receiving
power by attaching a USB-A plug directly to the board. I wanted to use
a power lead of some description, going to the controller board which then
had the LED strip screwed into it on terminals. As I was ordering some other
boards, I thought I would knock up this board and order it at the same time.

Power can be supplied via 5V on the barell plug, or 5V via a USB-B connector.

Attach an ESP01(S) board to the header. The PROGRAM button can be used to
bring up the ESP01 in programming mode, with the UART pins provided on
another header for connecting a USB UART. Ensure the USB UART is in 3.3V
mode!

## TODO

When time allows I will CAD-up a small printable case for enclosing this
board.
 