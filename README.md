# Keegzcore
Universal arcade-input controller for accessible gaming and rehab.
Built by KeegzCade (YouTube).

## Status
- V1 (RP2350A): Keegzcade Universal Controller V1 schematic (KiCad) only, rev 1.0. Never fabricated, since V2
  changed too much. The first draft was prototyped on a Pico.
  ## Parts used (V1)
    **Core**
    U1: RP2350A microcontroller
    U4: W25Q128JVS 128Mbit QSPI flash
    U2: MCP1117-3.3 LDO regulator (SOT-223)
    Y1: 12 MHz crystal (15 pF load caps, 1k series resistor)
    L1: 3.3 uH inductor (RP2350 on-chip regulator)

    **Connectors**
    J1: USB-C receptacle (USB 2.0, 16-pin)
    J7: 2x11 2.54mm female header (GPIO0-21)
    J8: 1x6 GameCube controller connector
    J6: 1x5 2.54mm header (SWD debug)
    J2-J5: 3-pin protected receptacles, 4 analog inputs (ADC0-3)

    **Protection and power**
    D1, D2: PESD3V3U1UL ESD protection diodes on USB data lines
    27 ohm series resistors on USB D+/D-
    5.1k resistors on USB-C CC lines
    Decoupling caps (10uF, 4.7uF, 100nF) and 0.1uF filter cap

    **Controls and outputs**
    SW1, SW2: Omron B3FS buttons (BOOT and RUN/reset)
    D3: WS2812B addressable RGB LED
    BZ1: buzzer, driven by Q1 (NPN transistor)
  
- V2 (RP2350B): in progress, with more power, more connections and
  more capabilities
- First draft prototyped on a Pico
- Arch Linux running (fast)
- Started own small package set for Keegz OS (GRUB, Firefox, basics)

## Doing
- Keegz OS: input layer for keegzcore
  - Pre-inputted profiles
  - Talks to the Keegz browser layer (browser remapper)

## Next
- Commit packages.txt (`pacman -Qqe > packages.txt`)
- Add the KiCad files to hardware/
- Add the Pico prototype code to firmware/
- V2: RP2350B, 8 pots

## Ideas / notes
- Goal: replace controllers, MIDI pads and other devices with one rig
- Channel: KeegzCade (YouTube)

## License
GPL-3.0 (firmware), CERN-OHL-S (hardware)
