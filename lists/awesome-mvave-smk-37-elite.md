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

- **SMK37 OPEN (official)** — M-VAVE's own open firmware and web workbench for the SMK-37 Pro and Elite, with the matching binary SDK: eight tracks (DX7 FM, 303, 808, PSG, plucked string, and sample engines), 16–64-step sequences, arpeggiators, chords, parameter locks, effects, 16 project slots, a 128-preset DX7 library with SysEx import/export, USB/BLE MIDI input and DIN/USB/BLE output, and pad pressure as aftertouch. The workbench handles firmware updates, browser playback, and project, sample, and DX7 voice management. Licensed "Other" (see its LICENSE file).
  - [Workbench](https://open.m-vave.com/smk37-workbench) — Official browser workbench and development kit download.
  - [Code](https://github.com/m-vave/smk37_open) — Official repository (also hosts the SDK).
- **SMKSYNTH** — GPL-3.0 performance firmware for the SMK-37 Pro (v1.0.0; Portuguese and English manuals): marries OberVave's synthesis with the DRUM-X engine from JIANT and adds pad-centred performance features (parts, scenes, layers and splits, sequence recording, favorite sounds with one touch). The author tested it on a SMK-37 Pro; the installer accepts only a Pro on official V016 and refuses the Elite, the MKE-P37, the FM-1 and other firmwares. Browser simulator and backup/restore page on the site.
  - [Site](https://4t59m4f784-creator.github.io/SMKSYNTH/) — Installer, simulator and backup page.
  - [Code](https://github.com/4t59m4f784-creator/SMKSYNTH) — Source repository and releases.
- **Skiff** — Six-track groovebox firmware (fourteen synth and drum engines, 64-step sequencer, scenes, browser editor) with a dedicated SMK-37 Pro build since 1.4: the 16 pads become the step grid, the four faders a mixer, MIDI OUT with clock. Same installer picks the keyboard build; the Elite and MKE-P37 builds were reported as not yet tried on hardware.
  - [Site](https://illuminus5.github.io/skiff/) — Project page.
  - [Code](https://github.com/illuminus5/skiff) — Source repository, with SMK37.md install notes.
- **SMKTRON** — GPL-3.0 lo-fi Mellotron firmware for the SMK-37 Pro, adapted from FMEL-1: flute, choir, cello and violins with layering, chord pads, a sequencer, grain, tape wear, vibrato, Leslie, echo and reverb. Site with simulator and installer in Portuguese and English; first installation requires official SMK-37 Pro V016, and other models and firmware origins are rejected.
  - [Site](https://4t59m4f784-creator.github.io/SMKTRON/) — Project page, simulator and installer.
  - [Code](https://github.com/4t59m4f784-creator/SMKTRON) — Source repository.
- [smk37-base](https://github.com/fc79/smk37-base) — GPL-3.0 minimal SMK-37 firmware to build your own on: Dinghy for the SMK-37 only (Felucca/SLOOP platform and genkigenki's SMK-37 layer), with update path, USB rescue, USB MIDI/audio, keys, pads, encoders, faders, wheels, LEDs and screen each used once as an example. Installed and checked on one SMK-37 Pro only; Elite and MKE-P37 packages untried.
- [mdsmk](https://github.com/konsumer/mdsmk) — GPL-3.0 fork of Mutable Dreams (Kid Bunka) built by CI for both the FM-1 and the SMK-37; the web installer at mutant.cloud picks the right package for the connected device, with a rescue page to return to stock firmware.
- **ECHOFIELD (SMK-37)** — Granular sampler firmware port for the SMK-37 Pro / Elite: a few seconds of any sound become clouds, sparkles and tape loops, played from keys, pads, faders and wheels. Not tested on an SMK-37 yet (written from community hardware documentation, tested in simulation): back up your flash first. A fence in the flash driver keeps writes away from factory calibration, Bluetooth pairing and stock presets.
  - [Site](https://philip-bos.github.io/echofield-smk37/) — Companion app and flasher.
  - [Code](https://github.com/Philip-Bos/echofield-smk37) — Source repository and notes for testers.
- [smk37-aisling](https://github.com/stephencummins/smk37-aisling) — GPL-3.0 stage 1 port of the AISLING ambient drone firmware to the SMK-37 Elite (layout read from M-VAVE's V016 firmware; not the Pro or the MKE-P37). Passes its tests on a computer but has not run on an Elite, and the author offers no package until it has been installed, played and removed on one.
- [TLBX Animate (SMK-37 Pro)](https://github.com/mmi-studios/tlbx1-animate-smk37) — GPL-3.0 unofficial port of the Animate engine from the TLBX-1 audio toolbox: a four-slot vector wavetable synthesizer with a 289-wave bank, a ten-lane sequencer and a browser simulator; builds on Linux x86-64 or WSL and publishes no releases.
- **PERF-1 SMK (beta)** — GPL-3.0 beta test builds of PERF-1, the generative live-performance groovebox, on the SMK-37 Pro, with the SMK's controls, FOLLOWERS (drones on the chord) and CALL AND RESPONSE; not a release, so things may change or break and saved pieces may not carry over. M-VAVE's own firmware can be put back from the same page or with M-UPGRADE.
  - [Site](https://deamonslinky.github.io/PERF-1-SMK/) — Beta installer (Chrome or Edge).
  - [Code](https://github.com/deamonSLINKY/PERF-1-SMK) — Development tree plus the SMK board layer.
- [smk37-elite-firmware](https://github.com/TexasRADIO/smk37-elite-firmware) — GPL-3.0 open firmware (v1.0.0, SMK-37 Elite only: not for the FM-1, SMK-37 Pro or MKE) that turns the keyboard into a four-part performance instrument: Conductor (bar-aligned song and setup launches), Telegram (SH-101-style lead), Dillo (TB-303-style bass) and a synthesized 808, with a library of 1,056 band preset bars and imported acid phrases. A rollback `.fwsc` and checksums are in the [releases](https://github.com/TexasRADIO/smk37-elite-firmware/releases); the repository documents the permission for its acid-part data and its provenance.
- [m-apps](https://github.com/jvitkauskas/m-apps) — MIT kit and sample apps that run from RAM on the SMK-37 and FM-1 without changing the flash firmware; `hello`, `usbdisk` and the SD-card `picker` have run on an SMK-37. Early, no releases.
- **WORSHIP (worship-smk37)** — GPL-3.0 Felucca fork with the SMK-37 layer for church music (Portuguese documentation): an ambient pad by key, a 16-song setlist and keys-plus-lead routing; the GLOBE button opens the full Felucca synth. The author states it has been tested only in simulation and has not yet run on a real SMK-37; back up first.
  - [Site](https://jefersomusic-del.github.io/worship-smk37/) — Browser simulator.
  - [Code](https://github.com/jefersomusic-del/worship-smk37) — Source repository and `.fwsc` release.
- **Classic Tabby** — Performance-oriented fork of SMK37 OPEN for the SMK-37 Pro (Linux build), with a `.fwsc` and workbench HTML in its v01.0 release. The README is still M-VAVE's SMK37 OPEN text, so what differs from the official firmware is not documented; the licence file is not an SPDX-standard one.
  - [Site](https://seattleuser0.github.io/classic-tabby/) — Project page.
  - [Code](https://github.com/SeattleUser0/classic-tabby) — Source repository and release.
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
- [synth-rescue (Cardputer ADV)](https://github.com/jvitkauskas/cardputer-synth-rescue) — MIT v0.1.0 unbricker for the FM-1 and SMK-37 using only an M5Stack Cardputer ADV and a USB-C cable: it puts the unit in ROM download mode, backs up the whole 1 MiB flash to the SD card and installs m-bootloader plus a minimal open fm1-base firmware. Early release; it overwrites the whole flash, so keep the backup it makes.
- [M-Unbricker](https://jvitkauskas.github.io/m-unbricker/) — MIT rescue for a bricked FM-1 or SMK-37 using a second working unit and a USB-C cable, with no dongle and nothing installed on the working unit (step-by-step page for desktop Chrome/Edge, Android Chrome or iOS MIDIWeb). Tested on an FM-1 and an SMK-37 Pro, both ways. [Source](https://github.com/jvitkauskas/m-unbricker).
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
- **SLOOP Pro** — isod89's SLOOP groovebox firmware on the SMK-37 (GPL-3.0).
  - [Site](https://isod89.github.io/sloop-pro/) — Project page.
  - [Code](https://github.com/isod89/sloop-pro) — Source repository.
- **Clipper for the SMK-37 Pro** — Unofficial port of isod89's Clipper synth (23 engines, 407 factory sounds) to the SMK-37 Pro.
  - [Site](https://davidozz0.github.io/clipper-smk/) — Project page.
  - [Code](https://github.com/davidozz0/clipper-smk) — Source repository.
- **Clipper Pro** — isod89's own Clipper synth (23 engines, 407 sounds, four macros per sound, effects, arpeggiator, step sequencer, microtuning, MPE, USB audio and MIDI) on the SMK-37, with builds for Pro and Elite (and an MKE variant) and a browser editor; version 1.2, GPL-3.0, French quick-start guides included.
  - [Site](https://isod89.github.io/clipper-pro/) — Project page, browser installer and editor.
  - [Code](https://github.com/isod89/clipper-pro) — Source repository and `.fwsc` releases.
- **Impressionism** — Generative ambient firmware (Debussy/Ravel-style harmony) that also ships SMK-37, SMK-37 Elite and MKE builds; see the FM-1 list for details.
  - [Site](https://darrenjaworski.github.io/fm-1-impressionism/) — Project page with browser emulator.
  - [Code](https://github.com/darrenjaworski/fm-1-impressionism) — Source repository and `.fwsc` releases.
- **Modular Compagnon** — Free Elite firmware by Bungle Society: sixteen Modular Town sounds, a DAW-following arpeggiator and a little on-screen companion (black cat, fox, robot or goldfish); one control, one role, no banks or submenus; documentation in French and English.
  - [Site](https://bunglesociety.github.io/modular-compagnon/) — Project page and installer.
  - [Code](https://github.com/bunglesociety/modular-compagnon) — Source repository and `.fwsc` release.
- **RemoteFM1** — GPL-3.0 firmware that makes the device a remote panel for firmwares running on the computer (keys, encoders and the MASTER pot out as MIDI, LEDs and screen driven back). The SMK-37 and SMK-37 Elite builds in the releases are untested on a unit; the FM-1 build was tested on 2026-10-28.
  - [Site](https://remotefm1.com/) — Project page.
  - [Code](https://github.com/quixotic7/RemoteFM1) — Source repository and releases.
- [Velvet EP90](https://github.com/THEGREATCJPark/smk37-velvet-ep90) — Eight original FM electric-piano sounds (90s R&B ballad bell attack) and a custom firmware for the SMK-37 Pro, with demo WAVs, SysEx files and full source; documentation in Korean. v0.1.0-alpha.1, not verified on real hardware by the author.
- **SMK-dee** — Dual-core polyphonic synthesizer and dynamic MIDI controller ported to the SMK-37 Pro and Elite.
  - [Site](https://djstrombo.github.io/SMK-dee/) — Project page.
  - [Code](https://github.com/djStrombo/SMK-dee) — Source repository.
- **SMK-zp12** — SMK-37 build of the ZP12 sampling drum firmware, with an installer.
  - [Site](https://djstrombo.github.io/SMK-zp12/) — Project page.
  - [Code](https://github.com/djStrombo/SMK-zp12) — Source repository.
- **NOTE RUSH 37** — Note-reading game for the SMK-37 (Elite, Pro, and MKE-P37), a Vector37 fork, playable in the browser and installable from the same page.
  - [Site](https://ueinegoms.github.io/noterush37/) — Browser version and installer.
  - [Code](https://github.com/ueinegoms/noterush37) — Source repository.
- **KeyLab** — Chinese-first, free, open-source, mobile-first music-theory and MIDI learning site (0.3.0 beta) with 64 lessons, real staff notation, and ear training; SMK-37 Pro and iPad/iPhone support is still being implemented.
  - [Site](https://dsimpson-man.github.io/keylab/) — Learning site.
  - [Code](https://github.com/Dsimpson-man/keylab) — Source repository.
- [smk37-pro-fl-port](https://github.com/kritonpc/smk37-pro-fl-port) — Runs the SMK-37 Elite V016 application on an SMK-37 Pro using Pro-compatible update packaging and an FL Studio controller profile; experimental, demonstrated on one Pro.
- [smk37-ableton-session](https://github.com/shalafidragon/smk37-ableton-session) — Ableton Live 12 Remote Script (v1.7) for the SMK-37 Pro on stock firmware: Session View navigation, clip launch/record/delete, transport, selected-track faders and RGB pad feedback. Developed with Codex (AI-assisted) and tested on one macOS setup and one keyboard (stock V15); Windows, Elite and Bluetooth untested. No licence declared.
- [umetate](https://github.com/AkirakoSaintJust/umetate) — Opinionated framework for designing, building, testing, and safely installing custom firmware for the FM-1 and SMK-37 (see the [FM-1 list](awesome-mvave-fm-1.md)).
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
- [SMK37-Pro-Firmware-Recovery](https://github.com/fabioribeiroengbr-cmd/SMK37-Pro-Firmware-Recovery) — Community write-up (Portuguese) of an attempt to recover an SMK-37 Pro after an interrupted firmware update, with a start-here guide and case notes. Experimental: the author states that a working recovery has not been proven.

## Community and Reviews

- [MOD WIGGLER thread](https://www.modwiggler.com/forum/viewtopic.php?t=294075) — Community discussion of the SMK-37 family's DX7 emulation, including the Elite variant.
- [Elektronauts thread](https://www.elektronauts.com/t/m-vave-smk-37-pro-affordable-dx7-emulator/234750) — Discussion of the SMK-37 Pro/Elite as an affordable DX7 emulator, sound quality, and workflow tips.
- [Heise: MIDI keyboard with DX7 emulation](https://www.heise.de/en/background/MIDI-keyboard-with-DX7-emulation-M-VAVE-SMK-37-Pro-tested-10503740.html) — In-depth hands-on test of the SMK-37 platform.
- [Equipboard overview](https://equipboard.com/items/m-vave-smk-37-elite) — Specs summary and where-to-buy listing.
- [The Firmware Hub: SMK-37 Pro](https://thefirmwarehub.com/smk37/) — Catalog page of community firmware for the SMK-37 Pro and Elite.
- [m-store](https://github.com/jvitkauskas/m-store) — MIT files behind the on-device store for the SMK-37 and FM-1: open-source firmwares mirrored from their authors' tagged GitHub releases with a signed catalogue per model.
- [SMK37 Firmware Drawer (Korean)](https://thegreatcjpark.github.io/SMK37-Firmware-Drawer/) — GPL-3.0 PWA catalogue that checks and installs the existing public SMK-37 and FM-1 packages (plus sloopDX experimental ports), keeps backups and offers a Windows download helper for +VA builds; Android USB installation is unverified ([source](https://github.com/THEGREATCJPark/SMK37-Firmware-Drawer)).
- [Synth Anatomy: Baud Girl SMK-37+VA](https://synthanatomy.com/2026/10/baud-girl-smk-37va-custom-firmware-for-the-m-vave-smk-37-pro-elite-and-variants.html) — Article on the virtual-analog and 8-bit groovebox firmware (beta) for the SMK-37 Pro, Elite and variants.
- [Synth Anatomy: Obervave](https://synthanatomy.com/2026/10/zvenson-obervave-your-m-vave-fm-1-and-smk-37-pro-elite-are-now-oberheim-like-polysynths.html) — Article on zvenson's Oberheim-style polysynth firmware (beta) for the FM-1 and SMK-37.
- [MATRIXSYNTH: Skiff 1.4 on the SMK-37 Pro](https://www.matrixsynth.com/2026/10/skiff-14-now-on-m-vave-smk-37-pro-plus.html) — Video of Skiff running on the keyboard.
- [Sonic State at Music China 2026](https://www.matrixsynth.com/2026/10/m-vave-fm-1-and-more-music-china-2026.html) — Video interview with M-VAVE about its open firmware and compact keyboards (via MATRIXSYNTH).
- [M-VAVE forum: SMK37 OPEN](https://forum.m-vave.com/topic/34) — Official forum thread for the eight-track SMK37 OPEN firmware and developer kit.

## Notes

- The SMK-37 Elite shares its DX7-style FM engine and JieLi hardware platform with the M-VAVE FM-1 and the SMK-37 Pro; some [Awesome M-VAVE FM-1](awesome-mvave-fm-1.md) SysEx tools and patch banks may be compatible, but always verify against the Elite's own SysEx documentation before importing.
- Always back up factory presets before updating firmware or importing third-party SysEx banks.

## Contributing

Pull requests are welcome. Include the tested firmware version, operating system, and a short description of the resource.
