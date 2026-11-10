# Awesome M-VAVE Tank Mini

> A curated list of official and community resources for the M-VAVE Tank Mini, a compact rechargeable guitar/bass multi-effects pedal with 21 presets, USB audio and Bluetooth.

## Contents

- [Official](#official)
- [Unofficial Editors](#unofficial-editors)
- [Reverse Engineering](#reverse-engineering)
- [Community](#community)
- [Notes](#notes)
- [Contributing](#contributing)

## Official

- [M-VAVE Product Ecosystem](https://www.m-vave.com/products) — Official product overview for the whole range.
- [M-VAVE Downloads](https://www.m-vave.com/download) — Official firmware, the M-EFCS editor (PC and mobile; it supports TANK-G, TANK-B, BLACKBOX, STATION-G, STATION-B, Tank Mini, Pocket AMP, SP100, MK300 and MK20) and the updaters.
- [M-VAVE app downloads](https://www.m-vave.com/appdownload) — Official mobile app downloads.
- [Effects Description (PDF)](https://manualf.oss-cn-hongkong.aliyuncs.com/manual/Combined-Effect-Pedals/Effects-Description.pdf) — Official description of the effects of the combined-effect pedals.
- [M-VAVE × TONE3000](https://www.m-vave.com/tone3000) — Official page on the TONE3000 (NAM) collaboration.
- [M-VAVE forum](https://forum.m-vave.com/) — Official forum, including firmware update summaries.

## Unofficial Editors

- [OpenTank Mini](https://github.com/xxyurirangelxx/opentank-mini) — MIT open-source desktop and mobile editor (v0.1.4: Windows, Linux and Android builds) that replaces the vendor's M-EFCS; use at your own risk and back up first.
- [Tank Mini for Mac](https://github.com/pedroseibel/tank-mini-mac) — MIT native macOS editor (English and Portuguese): all 21 presets, a reorderable six-block chain and live following of the footswitches over USB.
- [TANK MINI for Linux](https://github.com/viniciusapl97/tankmini-linux) — MIT native Linux app (GTK4, Rust) with a CLI, using a protocol reverse-engineered from M-EFCS for Android and confirmed byte by byte on hardware.

## Reverse Engineering

- [mvave-tank-mini-protocol](https://github.com/xxyurirangelxx/mvave-tank-mini-protocol) — Portuguese-language specification of the USB-MIDI and BLE protocol, tested on firmware `TANK MINI_009`; the README is the whole repository.

## Community

- [Rockboard PedalPedia: M-VAVE Tank Mini](https://www.rockboard.de/en/pedalPedia/M-VAVE/Tank-Mini/8063182204) — Product page with a board configurator.

## Notes

- Seller listings often mix the Tank Mini (21 presets) with the Tank-G and Tank-B (36 presets); check the model before relying on a spec.
- Editors write to the pedal through a reverse-engineered protocol: keep a backup.

## Contributing

Pull requests are welcome. Include the tested device, firmware version, operating system, and a short description of the resource.
