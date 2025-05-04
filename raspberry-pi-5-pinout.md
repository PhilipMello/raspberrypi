# Raspberry Pi 5 Pinout

![Raspberry Pi 5 Pinout](https://raw.githubusercontent.com/PhilipMello/media/refs/heads/main/raspberrypi/raspberry-pi-5-pinout-01.webp)

In this diagram, we cover the following headers:

- **J8 GPIO Header**: This is the default 40-pin GPIO header.
- **J14 PoE**: Power over Ethernet (PoE) connection.
- **J2 Power Switch**: While not officially confirmed, it may be related to the Real-Time Clock (RTC) battery.
- **J7 Composite Video**: Composite video output (no longer on an audio jack).
- **J17 Fan Header**: This header allows for PWM control and provides feedback for the fan's speed.

The RP1 GPIO bank (IO_BANK0) supports the following functions:

- 5 UART interfaces
- 6 SPI interfaces
- 4 I2C interfaces
- 2 I2S interfaces (including Clock Producer and Clock Consumer instances)
- Registered IO (RIO) interface
- 24-bit DPI output
- 4-channel PWM output
- Stereo PWM audio output (AUDIO_OUT)
- General-purpose clock input and output (GPCLK)
- eMMC/SDIO bus with a 4-bit interface
- Interrupt generation from pin level or edge transitions

The functional blocks and their locations on the GPIO pins have been designed to match user-facing functions on the 40-pin header of a Raspberry Pi 4 Model B.
