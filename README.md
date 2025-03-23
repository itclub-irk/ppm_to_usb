# ppm_to_usb

Firmware for ATMega32u4 based development boards (i.e. arduino pro micro) which converts 6 PPM channels to usb HID joystick inputs.

Connect PPM source (RC transmitter or RC reciever) as shown on the wiring diagram.
![Wiring diagram](/img/wiring_diagram.png)

For example, you can youse FlySky FS-i6 RC transmitter as PPM source. Just connect `GND` to `GND` and `PPM input` to `PPM` lines of trainer port. No additional settings are required.
![FlySky trainer port pinout](/img/flysky_trainer_port.jpg)

Compile and flash this firmware into devboard using PlatformIO or Arduino IDE.
After board reboots, check your device dispatcher for a new HID joystick device.

Dont forget to do axis calibration in your flight simulator.
