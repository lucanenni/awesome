# Awesome M-VAVE FM-1

> A curated list of official and community resources for the M-VAVE FM-1 pocket FM synthesizer.

## Contents

- [Official](#official)
- [Custom Firmware](#custom-firmware)
- [Unofficial Editors and Librarians](#unofficial-editors-and-librarians)
- [Preset Packs](#preset-packs)
- [Reverse Engineering](#reverse-engineering)
- [Community and Reviews](#community-and-reviews)

## Official

- [M-VAVE](https://www.m-vave.com/) — Official manufacturer site and product ecosystem.
- [M-VAVE FM-1 product page](https://www.m-vave.com/product?id=fm-1) — Official specifications: six-operator FM engine, 32 algorithms, 128 presets, arpeggiator, 16-step sequencer, triple MIDI.
- [M-VAVE Downloads](https://www.m-vave.com/download) — Official firmware (M-UPGRADE installer), PC/mobile software, and documentation.

## Custom Firmware

- [Groove OS](https://www.groove-os.com/) — Commercial ($29) custom firmware that turns the FM-1 into an 8-track groovebox: FM plus a new virtual-analog engine, 64-step sequencer with per-step sound changes (p-locks), independent track lengths, up to 20 voices, and a stage view for live play. Installs from Chrome/Edge over USB in about 2 minutes and the original firmware can be restored at any time.
  - [Manual](https://www.groove-os.com/manual) — Official Groove OS manual.
  - [Learn](https://www.groove-os.com/learn) — Nine-chapter guide to building a beat from scratch.
  - [Synth Anatomy coverage](https://synthanatomy.com/2026/10/groove-os-turns-the-m-vave-fm-1-into-an-8-track-groovebox.html) — News article on the release.
- [Felucca](https://github.com/hugelton/Felucca) — Hügelton Instruments' custom firmware that turns the FM-1 into a multi-engine synth: nine engines, four tracks with three synth parts each, a 64-step sequencer per track, and a web editor for every parameter, step grid, mixer, and preset library. ([Synth Anatomy coverage](https://synthanatomy.com/2026/10/hugelton-instruments-felucca-custom-m-vave-fm-1-firmware-turns-it-into-a-multi-engine-synth.html), [MATRIXSYNTH](https://www.matrixsynth.com/2026/10/fm-1-custom-firmware-felucca.html))
- [SLOOP](https://synthanatomy.com/2026/10/3dsam-sloop-custom-firmware-turns-m-vave-fm-1-into-a-4-track-groovebox.html) — 3dSam's free, open-source custom firmware that turns the FM-1 into a 4-track groovebox (Synth Anatomy coverage).
- [FM-1+VA](https://baudgirl.com/work/FM-1+VA) — Custom firmware focused on live performance and quality-of-life features, adding a Virtual Analog engine (BLEP oscillators, Super/Drift, ZDF filter), an editable sequencer with step move/copy, and corrected DX7 patch playback (fixed operator detune, LFO speed, algorithm 4/6 feedback, and velocity-0 note-on handling). Open-source firmware, a preset/pattern manager, and a browser FM/VA editor are listed as coming soon.

## Unofficial Editors and Librarians

- **FM1 Editor & Librarian** — Browser-based voice editor and patch librarian: edits all standard DX7 parameters plus the FM-1's effects chain, manages up to 10 custom banks alongside a catalog of 65 DX7 banks, and transfers patches or full banks over MIDI SysEx. No install required (Web MIDI, Chrome/Edge/Opera/Firefox).
  - [Site](https://fm1-editor.com/) — Live editor and librarian.
  - [Code](https://github.com/benny-sparra/fm1-dx7-patch-importer) — Source repository.
- [DXcompanion](https://dxcompanion.uk/) — Web MIDI editor and librarian for Yamaha DX-family synths, including the FM-1; supports live editing over Web MIDI or offline work with bundled factory libraries. Can send patches to the FM-1 but not read them back.
- [OpenPatches](https://openpatch.es/) — Web utility that matches an uploaded WAV recording to the closest DX7 patch via spectral analysis, plus live auditioning, sequencing, mutating, and exporting patch sets as `.syx` files for the FM-1.
- [FM1 Controller](https://www.zalmanim.com/2026/09/21/fm1-controller-vst3-mvave-fm-1-editor/) — Free Windows VST3 plug-in/standalone editor exposing all 155 DX7 parameters on one screen, with patch storage in the DAW project and a bundled library of 46,777 deduplicated DX7 patches. Requires the hardware connected via MIDI.

## Preset Packs

- [fm1-factory-presets](https://github.com/KingParamount/fm1-factory-presets) — FM-1 factory presets recovered as four standard DX7 bank dumps (piano/organ, guitar/bass, brass/woodwind, percussion/effects), with SysEx protocol notes, an FM synthesis tutorial PDF, and Python decoding tools.
- [DXcompanion.uk patch catalog](https://dxcompanion.uk/) — Four curated DX7 banks (best-of, drums/percussion, orchestral, extras/SFX) built from FM staples, DOS, and Sega Genesis game sounds; loadable via SysEx.
- [Digital X7](https://squaresawsound.gumroad.com/l/digital-x7) — Commercial DX7-compatible patch bank usable on the FM-1 via SysEx import.
- [Engedal's Yamaha DX7 presets](https://engedal.gumroad.com/l/cFMYB) — Commercial DX7 patch collection compatible with FM-1 SysEx import.

## Reverse Engineering

- [fm1-custom-fw](https://github.com/aroum/fm1-custom-fw) — Reverse-engineering research on the FM-1's JieLi AC791N processor, bootloader, memory map, and SysEx frame layout, with a SysEx scanner and an experimental (untested on hardware) MIDI SysEx firmware flasher script.
- [KVR Audio FM-1 thread](https://www.kvraudio.com/forum/viewtopic.php?t=632127) — Long-running community thread tracking firmware updates, SysEx editing support, and third-party tools.
- [Firmware update guide (Medium)](https://medium.com/@shelvindatt02/how-to-update-the-firmware-on-your-m-vave-fm-1-synthesizer-7bc4ea2c3bd5) — Step-by-step walkthrough of the M-UPGRADE SysEx firmware update process.
- [FM-1 firmware tracker (fwradar.com)](https://fwradar.com/p/m-vave-fm-1) — Firmware version history and changelog tracking for the FM-1.

## Community and Reviews

- [Synth Anatomy review](https://synthanatomy.com/2026/07/m-vave-fm-1-review-low-budget-pocket-fm-ynthesizer-with-iconic-sounds.html) — Hands-on review of the budget pocket FM synth.
- [Synth Anatomy: V15 update](https://synthanatomy.com/2026/07/m-vave-fm-1-a-budget-friendly-dx-7-style-desktop-fm-polysynth.html) — Coverage of the V15 firmware update and new features.
- [Synth Anatomy: FM-1+VA](https://synthanatomy.com/2026/09/baud-girl-fm-1-va-custom-m-vave-fm-1-firmware.html) — Coverage of the Baud Girl FM-1+VA custom firmware.
- [Synth Anatomy: patch librarian](https://synthanatomy.com/2026/07/m-vave-fm-1-patch-librarian.html) — Coverage of the browser-based patch librarian simplifying DX7 sound transfer.
- [Synthtopia announcement](https://www.synthtopia.com/content/2026/07/13/m-vave-introduces-fm-1-fm-pocket-synthesizer/) — Introduction of the FM-1 pocket synthesizer.
- [MATRIXSYNTH announcement](https://www.matrixsynth.com/2026/06/new-mvave-fm1-mini-fm-synthesizr.html) — Initial coverage of the FM-1.
- [MATRIXSYNTH: V15 firmware](https://www.matrixsynth.com/2026/07/m-vave-fm-1-v15-firmware-update-new.html) — Coverage of the V15 firmware update.
- [Sonicstate reviews roundup](https://sonicstate.com/news/2026/07/10/m-vave-fm-1-reviews-/) — Aggregated early reviews and impressions.
- [rackears.io buyer's guide](https://www.rackears.io/products/m-vave-fm-1) — Specs, pricing context, and video demos.
- [Tao of Mac notes](https://taoofmac.com/space/com/m-vave/fm-1) — Personal notes and links collected on the FM-1.
- [Gearspace thread](https://gearspace.com/threads/m-vave-fm-1.1465371/) — Community discussion covering sound quality, build, and tools.
- [Elektronauts thread](https://www.elektronauts.com/t/m-vave-fm-1/252170) — Community discussion and tips.
- [Firmware V09 overview video](https://www.youtube.com/watch?v=n-TShi-a5OA) — Video walkthrough of firmware V09 features and the upgrade process.
- [M-VAVE FM-1 review video](https://www.youtube.com/watch?v=eAMhxsnagx8) — Video review of the synth.

## Notes

- Always back up your 128 factory presets before installing custom firmware or bulk-importing SysEx banks.
- Custom firmware (e.g. Groove OS, Felucca, SLOOP, FM-1+VA) and reverse-engineered tools are unofficial and not supported by M-VAVE; read the relevant project's disclaimers before flashing.
- The FM-1's sound engine is Dexed-based, so most DX7 SysEx patches and editors work with minor caveats — check each tool's notes on send/receive support.

## Contributing

Pull requests are welcome. Include the tested firmware version, operating system, and a short description of the resource.
