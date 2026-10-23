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
- [smk-37-asio-drivers](https://github.com/amalahama/smk-37-asio-drivers) — Dedicated low-latency ASIO driver and control panel for the SMK-37 Pro on Windows 10/11, offered as an alternative to ASIO4ALL (written for the Pro, so check Elite compatibility).
- [smk37pro-acidsound-mod](https://github.com/acidsound/smk37pro-acidsound-mod) — Personal firmware-mod research project that loads arbitrary DX7 drum voices into the internal Ch10 drum synth; it analyzes the official USB OTA path, carries a brick risk, and was verified on a Pro (its GitHub Pages site was not yet live when checked).
- **Snoop37** — Alternative firmware for the SMK-37 Pro that turns it into a standalone four-track groovebox (three synth tracks and a drum machine): a port of SLOOP 2.5, itself based on Felucca. Its browser hub lists the SMK-37 Pro, SMK-37 Elite, and MKE-P37 as supported keyboards, noting that an Elite running an older build reports itself as an SMK-37 Pro.
  - [Site](https://genkigenki.github.io/smk37/) — SMK-37 firmwares (Snoop37, Vector37) installable from the browser, with simulator and a path back to factory firmware.
  - [Code](https://github.com/genkigenki/Snoop37) — Source repository.
- [M-Flasher](https://github.com/jvitkauskas/m-flasher) — Back up, restore, and reinstall firmware on the SMK-37 Pro / Elite (and FM-1) over USB download mode, with an open bootloader option and a backup before every write.
- **Biosphere37** — Browser app (connect the keyboard over Web MIDI) that turns the SMK-37 into controls for a blacklight galaxy: the 37 keys play a synth and draw a neon route, the 16 pads fly to six sound worlds and switch effects, and the faders control drive, delay, and reverb. It runs on a computer, not on the keyboard.
  - [Site](https://sunyux.github.io/biosphere37/) — Hosted app.
  - [Code](https://github.com/sunyux/biosphere37) — Source repository.
- **SMK-37 Repair** — Small firmware for the SMK-37 Pro, Elite, and MKE-P37 that repairs M-VAVE's key mapping while keeping the keyboard's calibration, wheel values, and Bluetooth pairings; for the case where, back on M-VAVE's firmware, every key reads "C" and the synth is silent.
  - [Help](https://genkigenki.github.io/smk37/help.html) — Hub help page.
  - [Code](https://github.com/genkigenki/smk37-repair) — Source repository.
- **genkigenki's other SMK-37 ports** — The same author (Snoop37, Vector37, Erik37) also ships SMK-37 builds of FoMni ([FoMni37](https://github.com/genkigenki/FoMni37)), MAKU ([MAKU37](https://github.com/genkigenki/MAKU37)), X0X ([X0X37](https://github.com/genkigenki/X0X37)), Makkuro ([Makkuro37](https://github.com/genkigenki/Makkuro37)), and Rainbow ([RAINBOW37](https://github.com/genkigenki/RAINBOW37)), plus SMK-37 releases of AMB-1, Polly, ORBIT, and winampFM; all are installable from the [hub](https://genkigenki.github.io/smk37/).
- [Oscuro companion protocol](https://github.com/kartun83/oscuro-companion-protocol) — Prototype of a phone-to-keyboard USB file bridge in which the phone is the USB host and the keyboard the device, including a RAM firmware payload.
- [altstrument: SMK-37](https://altstrument.org/devices/m-vave-smk-37) — Third-party firmware directory page tracking versions of the SMK-37 builds (covering the Pro, Elite, and MKE-P37).
- **Tonitor (SMK-37 Pro)** — Separate SMK-37 Pro build of the Tonitor acousmatic firmware for electroacoustic experimentation and live ambient music (see the [FM-1 list](awesome-mvave-fm-1.md)).
  - [Site](https://nzimas.github.io/tonitor-smk37/) — Project page.
  - [Code](https://github.com/nzimas/tonitor-smk37) — Source repository.
- [Erik37](https://github.com/genkigenki/erik37) — Sampled concert-grand piano firmware (velocity layers, dampers, pedals, sympathetic resonance, four rooms) for the SMK-37 and FM-1, from the same hub.
- [Vector37](https://github.com/genkigenki/Vector37) — Unofficial firmware for the SMK-37 family (installable from the [same hub](https://genkigenki.github.io/smk37/), which lists the Elite as supported): an orbiting overtone synth where a sun and moon moving along a path blend four corners of overtone generators and filters, with pads and knobs as the planets.
- [NESynth](https://chancethemaker.github.io/NESynth-FM1-SMK/) — NES homebrew player and cartridge-firmware builder that targets both the FM-1 and the SMK-37 Pro / Elite (see the [FM-1 list](awesome-mvave-fm-1.md)).
- **SMK Lab** — ChanceTheMaker's parent site for independent SMK-37 Pro / Elite firmware, browser studios, and simulators (including NESynth, Doom, and GameDude Color).
  - [Site](https://chancethemaker.github.io/smklab/) — Projects hub.
  - [Code](https://github.com/ChanceTheMaker/smklab) — Source repository.
- [m-bootloader](https://github.com/jvitkauskas/m-bootloader) — Open-source clean-room bootloader for the SMK-37 Pro / Elite and FM-1, used by M-Flasher.
- [melodee-smk37](https://github.com/djStrombo/melodee-smk37) — Port of the Melodee dual-core multi-engine synthesizer firmware to the SMK-37 Pro and Elite.
- **Melodee SMK** — ChanceTheMaker's Melodee for the SMK-37 Pro and Elite: dual-core beta with a browser Studio, simulator, and public installer.
  - [Site](https://chancethemaker.github.io/melodee-smk/) — Installer, Studio, and simulator.
  - [Code](https://github.com/ChanceTheMaker/melodee-smk) — Source repository.
- **picovave** — PICO-8 (femto8) firmware for the SMK-37 Pro, with a browser simulator built from the same engine (Korean-language README).
  - [Site](https://acidsound.github.io/picovave/) — Simulator and project page.
  - [Code](https://github.com/acidsound/picovave) — Source repository.
- [Jellybean-37](https://github.com/edco/jellybean-37) — Open dual-target firmware and hardware simulator for the SMK-37 Pro, described by its author as a rough testbed for the MCUno-32 engine and optimizations.
- [Doom FM-1 / SMK](https://chancethemaker.github.io/doom-fm1-smk/) and [GameDude](https://chancethemaker.github.io/gamedude-fm1-smk/) — Doom-engine port and Game Boy emulator tooling that target both the FM-1 and the SMK-37 Pro / Elite (see the [FM-1 list](awesome-mvave-fm-1.md)).
- [fm1-to-smk37](https://github.com/genkigenki/fm1-to-smk37) — Guide to porting FM-1 custom firmware to the SMK-37 Pro: the keyboard shares the FM-1's JieLi AC791N chip, bootloader, update loader, and chip key, so only the board layer (key matrix, analog inputs, display, pad LEDs, flash map) differs.
- [zp12-smk37](https://github.com/djStrombo/zp12-smk37) — SMK-37 port of the ZP12 12-bit sampling drum firmware (see the [FM-1 list](awesome-mvave-fm-1.md)).
- [smk37_pro_midi_sysex](https://github.com/hartaberunfairer-web/smk37_pro_midi_sysex) — HTML page for monitoring the SMK-37 Pro's BLE MIDI and SysEx traffic. Unverified: the repository has no README yet.

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
