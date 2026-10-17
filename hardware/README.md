# MacroPlay hardware

MacroPlay is an open-source macro keyboard designed for automation and customization. It is aimed at creators, gamers and professionals who want to control their workflows with programmable keys and lighting effects.

## Main features

- 12 programmable keys (main keys)
- 4 profile keys to switch between macro sets
- Configurable rotary encoder
- Buzzer for audio feedback
- Addressable RGB LEDs on every key
- Open source: hardware and schematics are released for modification

## Philosophy

This project encourages modification and customization. You can adapt the hardware, swap the firmware, remap keys, create new LED effects and share your improvements.

## Contents

The Altium Designer project is in [`MacroPlay/`](MacroPlay/): schematics, PCB, libraries, BoM, the schematic PDF (`MacroPlay.pdf`), the 3D model of the board (`MacroPlay.step`) and the manufacturing outputs (Gerber, NC drill and ODB++) in `Project Outputs for MacroPlay/`.

## Firmware and software

The firmware runs CircuitPython on the RP2040. It lives in this same repository, in [`firmware/`](../firmware/), together with the configuration page in [`web/`](../web/) and the profiles in [`profiles/`](../profiles/).

## Contributing

Contributions are welcome: issues, pull requests, alternative designs, new firmware and tutorials. Document your changes and include tests when applicable.

## License

See the [Licenses](../README.md#licenses) section of the main README.
