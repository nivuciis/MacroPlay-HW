# MacroPlay

Open macro keyboard with 12 keys, an RGB LED under each key, a rotary encoder and a buzzer, built around an RP2040 devkit with 16 MB of flash. It runs CircuitPython and is configured through an HTML page stored on the keyboard itself, with no software to install.

MacroPlay is designed for three audiences: people who want ready-made shortcuts for the programs they use, programmers who want their own automations, and people with motor or visual disabilities who need an adaptable keyboard.

## What it does

| Feature | Purpose |
| --- | --- |
| Keyboard, mouse and media keys (USB HID) | Shortcuts, text snippets, volume, cursor control |
| HID gamepad | Controller for emulators and games |
| USB MIDI | Music controller: the 12 keys form one octave |
| USB serial | Communication with the configuration page and with scripts on the PC |
| 12 RGB LEDs | Per-key color, active profile and status |
| Buzzer (active) | Audio feedback through beep rhythm and duration |
| Encoder | Volume, zoom, timeline, profile switching |

## Repository layout

| Folder | Contents |
| --- | --- |
| [`hardware/`](hardware/) | Schematic, PCB, BoM and manufacturing files |
| [`firmware/`](firmware/) | `code.py`, `boot.py` and CircuitPython libraries |
| [`web/`](web/) | HTML configuration page |
| [`profiles/`](profiles/) | Ready-made JSON profiles for programs and games |
| [`3d/`](3d/) | Case, accessibility keyguard and tactile keycaps |
| [`docs/`](docs/) | Project website (GitHub Pages) and test reports |

## Getting started

1. Install CircuitPython on the board (hold BOOT, plug in the USB cable and drag the `.uf2` file onto the `RPI-RP2` drive).
2. Download the latest version from **Releases** and copy the contents of `firmware/` and `web/` to the `CIRCUITPY` drive.
3. Open the configuration page on the drive and pick a profile or configure each key.

## Roadmap

Development is split into four phases, each with a milestone and its issues:

1. **Platform foundation:** JSON profile format, simple and advanced modes, Brazilian ABNT2 layout, competitive mode.
2. **Ready-made profiles:** Altium, Blender, Fusion 360, games, meetings, OBS and games on the keyboard itself.
3. **Accessibility and music:** sticky keys, tremor filter, NVDA integration, MIDI.
4. **Browser, AI and community:** in-browser emulator, AI configurator and profile gallery.

Follow the progress in the **Milestones** tab and on the **Projects** board.

## Contributing

Ideas, new profiles and test results are welcome. Open an issue using one of the templates (**Idea** or **Test result**). New profiles go in as pull requests to the `profiles/` folder.

In online games, profiles follow the **one key, one action** rule. Profiles with automatic sequences or repetition are not accepted for competitive games, because they can lead to bans.

## Licenses

- Hardware (`hardware/`, `3d/`): [CERN-OHL-S v2](LICENSE-HARDWARE)
- Firmware, web page, profiles and documentation: [MIT](LICENSE)
