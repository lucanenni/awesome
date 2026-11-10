# Awesome M-VAVE BlackBox

> A curated list of official and community resources for the M-VAVE (Sinco) BlackBox, sold as ANN BlackBox: a pocket multi-effects pedal and USB audio interface that OpenPocket supports alongside the Donner Pocket X.

## Contents

- [Official](#official)
- [Custom Firmware](#custom-firmware)
- [Unofficial Editors and Tools](#unofficial-editors-and-tools)
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

## Custom Firmware

- **OpenPocket** — GPL-3.0 open-source multi-effects firmware written from scratch for the Donner Pocket X and the M-VAVE BlackBox (JieLi AC791N): a 12-block chain of 78 models, NAM presets, a web installer and a web editor, with a `.fwsc` per version in the releases. The author calls it a proof of concept; the BlackBox build was still being tested.
  - [Site](https://isod89.github.io/openpocket/) — Installer and web editor.
  - [Code](https://github.com/isod89/openpocket) — Source repository and [releases](https://github.com/isod89/openpocket/releases).
- **Juice-Box** — GPL-3.0 replacement firmware (v0.17.0, English and Portuguese docs) that turns the ANN BlackBox into a Neural Amp Modeler A2 capture player: load `.nam` captures over USB, arrange them in banks and play live, with installer apps for macOS and Windows that can also restore the official firmware.
  - [Code](https://github.com/JPMViana/juicebox-nam-player) — Source repository and [releases](https://github.com/JPMViana/juicebox-nam-player/releases).
- [blackbox-nam-poc](https://github.com/seallegg/blackbox-nam-poc) — GPL-3.0 patches to the V20 firmware that run up to 18 NAM A2 lite captures natively, plus a `bbx` Python tool that backs up the pedal, builds the patched firmware and flashes it. A proof of concept that crashes, disables the factory amp models, carries brick risk and is announced as archived; partly written with AI help, as its README says.
- [ANNBLACKBOX Custom Firmware Installer](https://github.com/entitymar/annblackbox-custom-firmware-installer) — Windows tool that flashes custom `.fwsc` images or restores the factory V20 by patching a disposable copy of M-VAVE's own updater (which still does the transfer). Hardware-tested by its author on one unit with V20 only; the licence is not declared in a standard form.
- [mvave-blackbox-nam](https://github.com/tomanizer/mvave-blackbox-nam) — MIT research baseline for running NAM A2-Lite on the BlackBox with TONE3000 captures. By its own status note, no firmware has been built, installed or benchmarked yet.

## Unofficial Editors and Tools

- [BlackboxEdit](https://jvsobrinho.github.io/mvave-blackbox-edit/) — MIT browser preset editor over Web Bluetooth with real-time two-way communication ([source](https://github.com/jvsobrinho/mvave-blackbox-edit)). Beta: it writes to flash and its author takes no responsibility for bricked devices.
- [blackboxctl](https://github.com/mendong/blackboxctl) — macOS command-line tool, protocol notes and an example 12-preset bank for reading and writing the pedal over USB MIDI SysEx. Independent interoperability work.
- [mvave-blackbox-linux](https://github.com/Bulrok/mvave-blackbox-linux) — GPL-3.0 Linux tooling and protocol notes: the vendor's M-EFCS under Wine with a one-byte patch (the vendor binary is not included) and native control over USB-MIDI SysEx, with cab IR upload.
- [ESP32-S3 BlackBox MIDI controller](https://github.com/helgadb/ESP32-S3-M-VAVE-Blackbox-MIDI-Controller) — Portuguese-language ESP-IDF project for a DIY ESP32-S3 controller with battery monitoring for the BlackBox; no licence declared.

## Reverse Engineering

- [mvave-blackbox-reverse-engineering](https://github.com/jakino0/mvave-blackbox-reverse-engineering) — MIT documentation and read-only tooling for the ANN BlackBox: firmware, runtime layout, USB audio, BLE/M-EFCS protocol, OTA behaviour and DSP architecture.
- [mvave-blackbox-ble](https://github.com/jvsobrinho/mvave-blackbox-ble) — Notes on the BLE/GATT protocol (memory map, checksums) meant for third-party editors and hardware controllers; CC-BY-SA-4.0 documentation with GPL-3.0 code.

## Community

- [Rockboard PedalPedia: M-VAVE Blackbox](https://www.rockboard.de/en/pedalPedia/M-VAVE/Blackbox/487831603) — Product page that collects the manual, demo videos and reviews (Harmony Central, Reddit).

## Notes

- The pedal is sold under several names (BlackBox, ANN BlackBox, Annblack Box, Sinco). OpenPocket targets both the BlackBox and the Donner Pocket X; its README gives the details.
- Several resources replace the firmware or write to flash: back up first and keep the official V20 package as a fallback.
- A few projects here are AI-assisted or experimental; their entries say so.

## Contributing

Pull requests are welcome. Include the tested device, firmware version, operating system, and a short description of the resource.
