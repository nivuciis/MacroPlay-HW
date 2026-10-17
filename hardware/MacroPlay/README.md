# MacroPlay

MacroPlay is a custom macro keyboard (macropad) designed for gamers, programmers, and productivity enthusiasts. Built around the Raspberry Pi Pico microcontroller, it features 16 mechanical keys with per-key RGB addressable LEDs for customizable lighting effects.

## Features

- **16 Mechanical Keys**: 4 profile keys for switching between different macro sets, and 12 macro keys for executing custom commands
- **Per-Key RGB LEDs**: Each key has its own addressable RGB LED for individual lighting control
- **Raspberry Pi Pico**: Powerful microcontroller with USB-C connectivity
- **Hot-Swappable Switches**: Easy to replace switches without soldering
- **Customizable Firmware**: Open-source firmware for programming macros and lighting effects
- **Compact Design**: Ergonomic layout suitable for desktop use

## Hardware Specifications

- **Microcontroller**: Raspberry Pi Pico (RP2040)
- **Keys**: 16 mechanical switches (Cherry MX compatible)
- **LEDs**: 16 WS2812B RGB LEDs (one per key)
- **Connectivity**: USB-C
- **Power**: 5V via USB
- **Dimensions**: [TBD] mm x [TBD] mm x [TBD] mm

## Key Layout

```
[Profile 1] [Profile 2] [Profile 3] [Profile 4]
[ Macro 1 ] [ Macro 2 ] [ Macro 3 ] [ Macro 4 ]
[ Macro 5 ] [ Macro 6 ] [ Macro 7 ] [ Macro 8 ]
[ Macro 9 ] [ Macro 10] [ Macro 11] [ Macro 12]
```

## Getting Started

### Prerequisites

- Raspberry Pi Pico
- 16 mechanical switches
- 16 WS2812B LEDs
- USB-C cable
- Soldering iron and tools

### Assembly

1. Solder the WS2812B LEDs to the PCB
2. Install the mechanical switches
3. Mount the Raspberry Pi Pico
4. Flash the firmware

### Firmware

The firmware is based on [CircuitPython/QMK/whatever is used]. Instructions for flashing and configuring macros will be added.

## Usage

- **Profile Keys**: Switch between different macro profiles
- **Macro Keys**: Execute programmed macros (keyboard shortcuts, text snippets, etc.)
- **RGB Lighting**: Customize lighting effects via software

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Project Structure

- `MacroPlay.SchDoc`: Main schematic
- `MacroPlay.PcbDoc`: PCB layout
- `MacroPlay.PcbLib`: PCB library
- `MacroPlay.SchLib`: Schematic library
- `BOM Project_Name.xltx`: Bill of Materials template
- `MacroPlay.OutJob`: Output job file
- `MacroPlay.BomDoc`: Bill of Materials document

## Images

Screenshots and photos of the macropad can be found in the `Images/` directory.
