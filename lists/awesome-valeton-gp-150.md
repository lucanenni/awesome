# Awesome Valeton GP-150

> A curated list of official and community resources for Valeton GP-150.

## Contents

- [Official](#official)
- [Manuals](#manuals)
- [Unofficial Editors and Tools](#unofficial-editors-and-tools)
- [NAM and TONE3000](#nam-and-tone3000)
- [Preset Packs](#preset-packs)
- [Reverse Engineering](#reverse-engineering)
- [Mirrors](#mirrors)

## Official

- [Official downloads](https://www.valeton.net/download/) — Official Valeton download hub for firmware, software, manuals, and product files.
- [Valeton GP-150 product page](https://www.valeton.net/product/gp-150/) — Official product page with specifications, software, and firmware links.
- [Valeton Suite app](https://apps.apple.com/us/app/valeton-suite/id6739420888) — Official iOS companion app for tone editing, patch management, and updates over Bluetooth ([Android version](https://play.google.com/store/apps/details?id=com.sonicake.gp_5)). Recent releases add GP-150/GP-180 firmware V1.1.1 support and loading of converted NAM A2 files.
- [Windows 11 firmware update fix](https://www.sweetwater.com/sweetcare/articles/valeton-gp-series-firmware-update-fix-on-windows-11/) — SweetCare guide for firmware update problems on Windows 11 (see also the [official Valeton notice](https://www.valeton.net/win11-technical-notice/)).

## Manuals

- [GP-150 online manual](https://www.valeton.net/wpfd_file/gp-150_online-manual_en_firmware-v1-0-5-pdf/) — Online GP-150 manual with operating instructions, signal-chain information, and firmware-specific details.
- [GP-150 manual mirror](https://www.manualslib.com/manual/4387184/Valeton-Gp-150.html) — Mirror of the GP-150 manual, useful for browser reading and quick searches.

## Unofficial Editors and Tools

- **Valeton GP-150 Editor** — Browser-based preset editor and librarian over WebMIDI (Chrome/Edge, pedal on USB), with no vendor SDK or backend: reads every preset, edits blocks, models, and parameters live, renames and reorders presets and blocks, and browses SnapTone captures and IRs. A fork of the GP-5/GP-50 editor that adds GP-150 support (beta: read first and back up your presets before writing).
  - [Site](https://lucanenni.github.io/valeton-gp150-editor/) — Hosted editor, zero setup.
  - [Code](https://github.com/lucanenni/valeton-gp150-editor) — Source repository (MIT), forked from the [original GP-5/GP-50 project](https://github.com/drewmerc302/valeton-gp50), whose own hosted build is [valeton-gp50-woad.vercel.app](https://valeton-gp50-woad.vercel.app).
- [Valeton GP preset sorter](https://github.com/ciyi/Valeton-GP-Preset-Sorter) — Open-source utility for reordering GP preset files before importing them with Valeton software.
- [Custom firmware for GP-150 and GP-180](https://thegearforum.com/threads/custom-firmware-for-gp-150-and-gp-180.12050/) — Community discussion about unofficial custom firmware; unofficial and unsupported, so back up first.

## NAM and TONE3000

- [Use TONE3000 NAM Captures on Valeton GP Pedals](https://www.tone3000.com/blog/tone3000-valeton-nam-guide) — TONE3000 guide to converting and loading NAM captures on Valeton GP pedals via SnapTone and the companion software.
- [Valeton GP-150 and GP-180 put NAM support under $200 (Fader & Knob)](https://faderandknob.com/news/valeton-gp-150-gp-180-nam-support) — News coverage of the GP-150/GP-180 launch and their NAM support.

## Preset Packs

- [ToneGarage GP-150 presets](https://tonegarage.co.uk/valeton-gp150-180/) — Commercial preset collection for GP-150 and related Valeton processors.
- [Juca Nery free singing lead tone](https://jucaneryguitar.com/2026/07/27/free-singing-lead-tone-valeton-gp-150/) — Free GP-150 lead preset with a tutorial explaining the amp, delay, ambience, and sustain settings.
- [Guitar Tones Valeton patches and IRs](https://sites.google.com/view/guitartones) — Community/commercial library of Valeton patches, IRs, NAM files, and custom resources; verify GP-150 compatibility for each pack.
- [Andertons Valeton downloads](https://www.andertons.co.uk/andertons-valeton-downloads) — Free SnapTone downloads and patches created by Andertons performers; compatibility varies by Valeton model.

## Reverse Engineering

- [gp150-htfw](https://github.com/egorcipa8-debug/gp150-htfw) — MIT-licensed notes and tools on the Valeton HTFW firmware container (CRC-16/MODBUS region checksums, LZO1X payload packing), reverse-engineered from GP-150 images.
- [Valeton-GP180-Rev-Eng](https://github.com/majabojarska/Valeton-GP180-Rev-Eng) — GPL-3.0 notes, resources, and artifacts on reverse engineering the GP-180, which shares the platform family; useful background for the SysEx protocol.

## Mirrors

- [Valeton software mirror](https://valeton.web.id/software/) — Unofficial mirror of Valeton software downloads; use the official Valeton site whenever possible.
- [Valeton firmware mirror](https://valeton.web.id/firmware-valeton/) — Unofficial firmware index. Check model and version carefully before installing anything.

## Notes

- Always back up presets before updating firmware or importing third-party files.
- Verify exact model and firmware compatibility before using a preset or software package.
- Unofficial mirrors and community resources should be checked against the manufacturer’s documentation.

## Contributing

Pull requests are welcome. Include the tested device, firmware version, operating system, and a short description of the resource.
