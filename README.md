# H730/733 Duino

Arduino form factor and software compatible board with giant cortex-m7 at 550MHz.

![banner](docs/h730duino.png)

## Characteristics

 - CPU Cortex-M7 at 550MHz.
 - 128K/1MB of internal flash (depending of the MCU version).
 - 500KB of internal RAM.
 - 8MB of external QSPI PSRAM at 133MHz SDR.
 - 16/32/128MB of external QSPI Flash at 133MHz SDR.
 - 10/100Mb Ethernet.
 - USB 2.0 OTG Type-C with power switch control.
 - USB CMSIS-DAP Debugger.
 - uSD Card slot.
 - Arduino Due/Mega compatible pin headers (3.3V IO, 5V tolerant on some pins).
 - Arduino API compatible (via STM32Duino project).
 - Micropython support.
 - Protected power inputs with ideal diodes and DC-DC converter

![internal diagram](docs/internal-diagram.png)

## Capabilities and applications

Some interesting CPU capabilities are listed below:

 - Hard real time capable CPU with predictable execution using tightly coupled memory for instruction and data.
 - High speed and presition PWM suitable for motro control (BLDC, Stepper, DC).
 - High resolution timing measure in capture mode for some pins.
 - Arbitrary waveform generation in any GPIO using DMA without CPU intervention.
 - High speed DACs suitable to generate analog signals up to 18MHz.
 - High speed ADCs suitable to capture up to 5MSPS in any channel.
 - Internal RAM with multiple block paritions enabling multiple pheriperal access at same time without contention.
 - External high density RAM up to 8MB connected across 133MHz QSPI bus accesible in memory mapped mode or block device mode with on the fly encription/decription.
 - External high density FLASH up to 16MB connected across 133MHz QSPI bus accesible in memory mapped mode or block device mode with on the fly encription/decription.
 - Multiplexed parallel memory controller for LCD and TFT access
 - Parallel capture port at 200MHz

These capabilities enables multiple ineteresting applications:

 - High presition CNC and 3D printing.
 - Signal generator and data adqusition system
 - Human machine interface enabled terminal with USB, CAN and Ethernet support
 - High speed logic analyzer.
 - Programable instrumentation system.
 - Network laboratory instrument.

## Schematics

[Download in PDF format](docs/schematic.pdf)

![docs/h730duino.svg](docs/h730duino.svg)
![docs/h730duino.svg](docs/debugger-Debug.svg)
![docs/h730duino.svg](docs/ethernet-Ethernet.svg)
![docs/h730duino.svg](docs/USB-OTG-USB_OTG.svg)

## Licence

[MIT Licence](LICENCE.txt)
