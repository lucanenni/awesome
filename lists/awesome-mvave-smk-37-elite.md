# Awesome M-VAVE SMK-37 Elite

> A curated list of official and community resources for the M-VAVE SMK-37 Elite MIDI keyboard controller with built-in DX7-style FM synth engine.

## Contents

- [Official](#official)
- [Manuals](#manuals)
- [Documentation and Reverse Engineering](#documentation-and-reverse-engineering)
- [Community and Reviews](#community-and-reviews)

## Official

- [M-VAVE](https://www.m-vave.com/) — Official manufacturer site.
- [M-VAVE Products](https://www.m-vave.com/products) — Official product ecosystem listing, including the SMK-37 Elite in the MIDI series.
- [M-VAVE Downloads](https://www.m-vave.com/download) — Official firmware (M-Upgrade), MidiSuite device editor, Sinco Connector (Bluetooth MIDI), and mobile apps.

## Manuals

- [SMK-37 Elite user manual](https://manuals.plus/m/429b1ccce6a49ce721b72f2e4273ba886739413b86a651686edd4e25228c791b) — Full manual covering the 37-key controller, DX-7 style FM synth engine, pads, encoders, and DAW setup.
- [SMK-37 Elite manual (Manuals+)](https://manuals.plus/m-vave/smk-37-elite-37-key-velocity-sensitive-midi-keyboard-manual) — Alternative manual page covering setup, operation, and troubleshooting.
- [SMK-37 Elite manual (device.report)](https://device.report/manual/19067753) — Additional manual mirror.

## Documentation and Reverse Engineering

- [smk-37-pro-docs](https://github.com/jonathaslacerda/smk-37-pro-docs) — Community technical documentation covering firmware (`.fwsc` format, JieLi SoC extraction), hardware (DAC, battery charger, SoC datasheets), and SysEx implementation; explicitly notes the SMK-37 Elite, MKE-P37, and Donner Starrykey 37 Play as variants sharing the same platform with differing firmware binaries.
- [smk37-firmware-custom-mod](https://github.com/amalahama/smk37-firmware-custom-mod) — MIT-licensed custom firmware for the SMK-37 Pro (JieLi AC791N): v022 fixes BLE-MIDI pairing and note dropouts with the Woovebox 3.0 and improves DAW stability, with a Windows flasher and a dedicated low-latency ASIO driver ([v022 release](https://github.com/amalahama/smk37-firmware-custom-mod/releases/tag/v022)). Written and tested for the Pro, so check compatibility with the Elite before flashing.
- [SMK-37 Pro notes (Gist)](https://gist.github.com/probonopd/18b3ed65a69d0229eb630c47d7e316dc) — Independent technical notes on the device.
- [JieLi new firmware format](https://kagaimiq.github.io/jielie/datafmt/newfw.html) — Background documentation on the JieLi `.fwsc` firmware format referenced by the SMK-37 reverse-engineering docs.

## Community and Reviews

- [MOD WIGGLER thread](https://www.modwiggler.com/forum/viewtopic.php?t=294075) — Community discussion of the SMK-37 family's DX7 emulation, including the Elite variant.
- [Elektronauts thread](https://www.elektronauts.com/t/m-vave-smk-37-pro-affordable-dx7-emulator/234750) — Discussion of the SMK-37 Pro/Elite as an affordable DX7 emulator, sound quality, and workflow tips.
- [Heise: MIDI keyboard with DX7 emulation](https://www.heise.de/en/background/MIDI-keyboard-with-DX7-emulation-M-VAVE-SMK-37-Pro-tested-10503740.html) — In-depth hands-on test of the SMK-37 platform.
- [Equipboard overview](https://equipboard.com/items/m-vave-smk-37-elite) — Specs summary and where-to-buy listing.

## Notes

- The SMK-37 Elite shares its DX7-style FM engine and JieLi hardware platform with the M-VAVE FM-1 and the SMK-37 Pro; some [Awesome M-VAVE FM-1](awesome-mvave-fm-1.md) SysEx tools and patch banks may be compatible, but always verify against the Elite's own SysEx documentation before importing.
- Always back up factory presets before updating firmware or importing third-party SysEx banks.

## Contributing

Pull requests are welcome. Include the tested firmware version, operating system, and a short description of the resource.
