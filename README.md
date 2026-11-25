# keegzcore
Universal arcade-input controller for accessible gaming and rehab.
Built by KeegzCade (YouTube).

# PROGRESS

Last updated: 2026-11-25

## Done
- Keegzcade Universal Controller V1 schematic (KiCad): RP2350A, USB-C, 24 digital + 4 analog inputs, MIDI/HID, GameCube connector, RGB LED, buzzer
- First draft prototyped on a Pico
- Arch Linux running (fast)
- Started own small package set for Keegz OS (GRUB, Firefox, basics)

## Doing
- Keegz OS: input layer for keegzcore
  - Pre-inputted profiles
  - Talks to the Keegz browser layer (browser remapper)
- Studying the ArcoLinux package list on DistroWatch for ideas

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
