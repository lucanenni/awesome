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
- [Official firmware V15 image](https://yms-file-store.oss-cn-hongkong.aliyuncs.com/software/firmware/FM-1.fwsc) and [release notes](https://yms-file-store.oss-cn-hongkong.aliyuncs.com/software/releaseNote/firmware/FM-1.txt) — Direct links to the current official `.fwsc` and the changelog for every firmware version (custom firmwares expect you to be on V15 first).
- [FM-1 MIDI control reference (EN)](https://yms-file-store.oss-cn-hongkong.aliyuncs.com/software/releaseNote/firmware/FM-1%20MIDI%20EN.docx) — Official MIDI CC map, with the effects on their own MIDI channel.
- [FM-1 user manual (PDF)](https://m.media-amazon.com/images/I/A1WOydif9HL.pdf) — Multi-language printed manual (also mirrored on [Manuals+](https://manuals.plus/ae/1005012499001058)).

## Custom Firmware

- [Groove OS](https://www.groove-os.com/) — Commercial ($29) custom firmware that turns the FM-1 into an 8-track groovebox: FM plus a new virtual-analog engine, 64-step sequencer with per-step sound changes (p-locks), independent track lengths, up to 20 voices, and a stage view for live play. Installs from Chrome/Edge over USB in about 2 minutes and the original firmware can be restored at any time.
  - [Manual](https://www.groove-os.com/manual) — Official Groove OS manual.
  - [Learn](https://www.groove-os.com/learn) — Nine-chapter guide to building a beat from scratch.
  - [Synth Anatomy coverage](https://synthanatomy.com/2026/10/groove-os-turns-the-m-vave-fm-1-into-an-8-track-groovebox.html) — News article on the release.
- [Felucca](https://github.com/hugelton/Felucca) — Hügelton Instruments' GPL-3.0 multi-engine synth firmware (v1.0, in field testing): thirteen engines, four tracks, a 64-step sequencer per track with chords/ties/slide/chance, song chaining, chord keys, arpeggiator, modulation matrix, effects, class-compliant USB MIDI plus a USB audio input. Installs from Chrome/Edge over USB via the [web installer](https://hugelton.github.io/Felucca/) (no extra hardware; "Return to official V15" restores the stock firmware) and comes with a [web editor](https://hugelton.github.io/Felucca/webapp/editor/). ([Synth Anatomy coverage](https://synthanatomy.com/2026/10/hugelton-instruments-felucca-custom-m-vave-fm-1-firmware-turns-it-into-a-multi-engine-synth.html), [MATRIXSYNTH](https://www.matrixsynth.com/2026/10/fm-1-custom-firmware-felucca.html))
- [SLOOP](https://github.com/isod89/sloop-fm1) — 3dSam's free, open-source (GPL-3.0) live groovebox firmware based on Felucca (v2.2, beta): four tracks (three synths plus a drum machine), nine synthesis engines, 68 sounds, 37 drum kits, three user sample slots, punch-in FX, ratchets, note repeat, one-key chords, live song sections A–D, and a web editor. Install from Chrome/Edge with the [web installer](https://isod89.github.io/sloop-fm1/) or the `.fwsc` files in the [releases](https://github.com/isod89/sloop-fm1/releases); recovery from a failed install needs [FM-1-transporter](https://github.com/kurogedelic/FM-1-transporter). ([Synth Anatomy coverage](https://synthanatomy.com/2026/10/3dsam-sloop-custom-firmware-turns-m-vave-fm-1-into-a-4-track-groovebox.html))
- [Melodee](https://github.com/keremimo/melodee) — GPL-3.0 fork of Felucca 1.0 (v0.10) with a DX7-accurate FM6 engine (Dexed-compatible, up to 16 voices, on-device operator pages, DX7 SysEx import), a TR-808 drum kit, USB audio in/out, eight pattern banks per track, improved step editing, and MIDI/panel refinements. Installs from Chrome/Edge via its [web installer](https://keremimo.github.io/melodee/) (with a [web editor](https://keremimo.github.io/melodee/webapp/editor/)); the original firmware can be restored. Projects saved by earlier Melodee versions are not imported.
- [X0X](https://github.com/charlesvestal/fm1-x0x) — Beta groovebox firmware (fork of Felucca) with a TR-909, a TR-808, two TB-303s with TB-3PO acid generators, and a breakbeat generator, plus 16 patterns, song mode, recorded knob moves, shared reverb/tape delay, and a master compressor. Try it in the [browser emulator](https://charlesvestal.github.io/fm1-x0x/emu/), read the [manual](https://charlesvestal.github.io/fm1-x0x/manual/), and install from Chrome/Edge via the [web installer](https://charlesvestal.github.io/fm1-x0x/install/); heavy patterns can still hit the CPU limit. ([Synth Anatomy coverage](https://synthanatomy.com/2026/10/charles-vestal-x0x-custom-firmware-turns-the-m-vave-fm-1-into-a-rebirth-like-groovebox.html))
- **OMNI (FoMni)** — Charles Vestal's GPL-3.0 chord-harp firmware inspired by the Omnichord: the 16 white keys strum, the 11 black keys pick chords (hold ENV for minor, LFO for 7th), with an organ-style bass, ten OM-84 rhythms with auto bass sync, Home/SEQ/FX pages, and MIDI out. Try it in the [browser emulator](https://charlesvestal.github.io/fm1-fomni/emu/) and install from Chrome/Edge via the [web installer](https://charlesvestal.github.io/fm1-fomni/install/); the stock firmware can be restored. ([Synth Anatomy coverage](https://synthanatomy.com/2026/10/charles-vestal-fomni-1-an-omnichord-custom-firmware-for-the-m-vave-fm-1.html))
  - [Site](https://charlesvestal.github.io/fm1-fomni/) — Project page.
  - [Code](https://github.com/charlesvestal/fm1-fomni) — Source repository and [releases](https://github.com/charlesvestal/fm1-fomni/releases).
- [Flowstate](https://github.com/zakariachowdhury/flowstate-fm1) — Beginner-oriented fork of SLOOP 2.1 (GPL-3.0) in which almost any key press sounds musical: smart keys, musical guardrails, four performance controls, and factory "worlds"; the repository holds the UI/experience spec, a progress log, and firmware sources, and is still under active development.
- [Lunar Modulator](https://github.com/ip2k/lunar-modulator) — Open firmware project for the FM-1 (JieLi AC791N) building a multi-engine instrument: five engines with 160+ models (built on Mutable Instruments code), four effects, and a planned step sequencer with parameter locks. Preview only: it runs as a [virtual FM-1 in the browser](https://ip2k.github.io/lunar-modulator/) but has never been installed on real hardware.
- **Hortator** — Drum-machine firmware by DEADACTIVE built on Felucca (GPL-3.0): eight drum tracks, a step sequencer, Grids, a pumping compressor, LFOs, resonators, and live effects, all on the FM-1's own keys, knobs, and screen.
  - [Site](https://deadactive.github.io/hortator/) — Play the real firmware in the browser (compiled to WebAssembly) on a 3D FM-1.
  - [Code](https://github.com/DeadActive/hortator) — Source repository.
- **Jangada** — Felucca fork with a dark, industrial, Brazilian accent: ten synth engines (including a Dexed-compatible 6-operator FM and a superwave analog with a ladder filter), four tracks, a modulation matrix, latched drones, ratchets, original drum kits, and live-oriented effects.
  - [Site](https://zednaked.github.io/jangada/) — Project page.
  - [Code](https://github.com/zednaked/jangada) — Source repository.
- **FiMba-1** — Physically modelled kalimba (thumb piano) firmware grown from FoMni: the 16 white keys are tines laid out like a real kalimba, the black keys play thumb-roll chords or performance moves. Playable in the browser (the firmware's own C code compiled to WebAssembly) without an FM-1.
  - [Site](https://jadamsowers.github.io/fm1-fimba/) — Browser version and project page.
  - [Code](https://github.com/jadamsowers/fm1-fimba) — Source repository.
- **SLOOP ALG-05** — Independent experimental fork of SLOOP 2.2 (Chinese-language documentation) with 16 synth engines including a 6-operator DX7, VA, plucked-string and additive engines, 93 factory voices, 37 drum kits, a live waveform on the edit pages, and a web installer and voice editor. Not released by SLOOP's author.
  - [Site](https://shaw-core.github.io/Sloop_ALG02/) — Web installer and editor.
  - [Code](https://github.com/shaw-core/Sloop_ALG02) — Source repository.
- [FM-1 B-Boy Edition](https://github.com/friendsmakenoise-prog/fm1-pocket-sampler) — Experimental sampler/groovebox firmware treating the FM-1 as a late-90s chop sampler: three sampler tracks with up to 24 chops each, linked-chop break slicing, and per-track mono/poly playback; beta, with the six-operator voice verified on hardware.
- **Bubba Box** — GPL-3.0 groovebox firmware for live play, with a web editor, manual, and a Spanish-language sampler guide.
  - [Site](https://erbubar23.github.io/bubba-box/) — Project page with installer, web editor, and manual.
  - [Code](https://github.com/Erbubar23/bubba-box) — Source repository.
- **FuMi-1** — Shigin-conductor firmware inspired by the Suiko ST-50 (a Felucca fork): the sixteen white keys play the ST-50's lower row, the black keys its upper row or koto ornaments, with adjustable key (本数), equal or just tuning, a koto plus twelve more 6-operator FM sounds, ring time, vibrato, trill, and a looper.
  - [Site](https://cartesive.github.io/fumi-1/) — Project page.
  - [Code](https://github.com/cartesive/fumi-1) — Source repository.
- [fm1-chord](https://github.com/math0ne/fm1-chord) — Clean-room chord-machine firmware built on Felucca: the left white keys are the scale degrees (I to vii) and play chords, and the right white keys are an Omnichord-style strum plate for the last chord played.
- **AMBII** — Development-preview firmware built on Melodee's synthesis and sequencing core, with a redesigned recording and editing interface. Not ready for device installation: there is no qualified release image yet.
  - [Site](https://milkboyg.github.io/Ambii/) — Project page and documentation.
  - [Code](https://github.com/MilkBoyG/Ambii) — Source repository.
- [Optimist](https://github.com/w0ts/optimist) — GPL-3.0 modular firmware platform derived from SLOOP (with parts of Felucca, Melodee, and X0X) for building your own FM-1 firmware; work in progress, running on a single real unit since 2026-10-09, so use at your own risk.
- **Dinghy** — The smallest FM-1 firmware to build your own on: a four-voice sine on the keys, with the update path, USB rescue, USB-MIDI, USB audio, controls, screen, and settings storage already done and documented.
  - [Site](https://fm1.designburgapps.com) — Project site.
  - [Code](https://github.com/zvenson/dinghy) — Source repository.
- [SLICE64-FM](https://jeymadcat-ops.github.io/SLICE64-FM-web/) — 4-track SID / FM / sampler tracker firmware (see its web editor in [Unofficial Editors and Librarians](#unofficial-editors-and-librarians)); the editor requires firmware s1.3 or later.
- [hardware-supersynth](https://github.com/OwenKirby/hardware-supersynth) — Custom FM-1 firmware based on the author's "supersynth" architecture. Unverified and currently unreachable: it had no README or description when first listed, and the repository now returns 404 (removed, private, or renamed).
- [FM-1+VA](https://baudgirl.com/work/FM-1+VA) — Custom firmware focused on live performance and quality-of-life features, adding a Virtual Analog engine (BLEP oscillators, Super/Drift, ZDF filter), an editable sequencer with step move/copy, and corrected DX7 patch playback (fixed operator detune, LFO speed, algorithm 4/6 feedback, and velocity-0 note-on handling). Open-source firmware, a preset/pattern manager, and a browser FM/VA editor are listed as coming soon.

## Unofficial Editors and Librarians

- **FM1 Editor & Librarian** — Browser-based voice editor and patch librarian: edits all standard DX7 parameters plus the FM-1's effects chain, manages up to 10 custom banks alongside a catalog of 65 DX7 banks, and transfers patches or full banks over MIDI SysEx. No install required (Web MIDI, Chrome/Edge/Opera/Firefox).
  - [Site](https://fm1-editor.com/) — Live editor and librarian.
  - [Code](https://github.com/benny-sparra/fm1-dx7-patch-importer) — Source repository (also covers backups of all banks, duplicate-patch search, operator-level editing, an effects-chain editor, and `.syx`/`.zip` export; it can also write patches to FM-1+VA).
- [DXcompanion](https://dxcompanion.uk/) — Web MIDI editor and librarian for Yamaha DX-family synths, including the FM-1; supports live editing over Web MIDI or offline work with bundled factory libraries. Can send patches to the FM-1 but not read them back.
- [OpenPatches](https://openpatch.es/) — Web utility that matches an uploaded WAV recording to the closest DX7 patch via spectral analysis, plus live auditioning, sequencing, mutating, and exporting patch sets as `.syx` files for the FM-1.
- [FM1 Controller](https://www.zalmanim.com/2026/09/21/fm1-controller-vst3-mvave-fm-1-editor/) — Free Windows VST3 plug-in/standalone editor exposing all 155 DX7 parameters on one screen, with patch storage in the DAW project and a bundled library of 46,777 deduplicated DX7 patches. Requires the hardware connected via MIDI.
- [SLOOP web emulator](https://sabliran.github.io/sloop-web-emu/) — Browser emulator of an FM-1 running SLOOP or Felucca, built by compiling the unmodified GPL-3.0 firmware sources to WebAssembly ([source](https://github.com/sabliran/sloop-web-emu)).
- **SLICE64-FM Editor** — Web editor for the SLICE64-FM firmware: patterns, song order, mixer, instruments, and samples sent to the FM-1 over Web MIDI SysEx (Chrome or Edge, firmware s1.3 or later).
  - [Site](https://jeymadcat-ops.github.io/SLICE64-FM-web/) — Hosted editor.
  - [Code](https://github.com/jeymadcat-ops/SLICE64-FM-web) — Source repository.
- **FM-1 Pulses** — Generative browser MIDI sequencer (clock, gate probability, sample-and-hold, LFO, quantizer, Deja Vu loop) that broadcasts MIDI live; on the FM-1+VA firmware it can also freeze 64-step phrases into the FM-1's patterns.
  - [Site](https://mene311.github.io/fm1-pulses/) — Hosted PWA.
  - [Code](https://github.com/mene311/fm1-pulses) — Source repository.
- [FM-1 Workbench](https://github.com/thegiantsnail/fm1-workbench-public) — Web workbench ([live](https://fm1-workbench.web.app)), Android app, MCP server, and VST3/CLAP controller plugin: DX7 voice library and editor with randomize/mutate/morph, a drum sequencer, a MIDI file player, and a built-in software FM-1 so every tab works without the hardware.
- [FM-1 Utility](https://fm1-utility.pages.dev/) — Dependency-light Web MIDI editor for the FM-1.
- [fm1-read-voice](https://github.com/czietz/fm1-read-voice) — Reads the current voice back from the FM-1 over USB MIDI, which the stock firmware does not otherwise offer.
- [fm1-bank-sender](https://github.com/leomaimoni/fm1-bank-sender) — Android APK that sends `.syx` sound banks to the FM-1 from a phone.
- [fm1_soundbank_app](https://github.com/pfkellogg/fm1-bonus-box/tree/main/fm1_soundbank_app) — Command-line tool to list, reorder, and send a 128-preset soundbank over USB MIDI.
- [Sloop Go](https://github.com/jahlib/sloop-fm1-go) — Native Android app (Kotlin, USB-MIDI) for editing the FM-1 while it runs the SLOOP firmware, based on SLOOP's web editor.
- [SloopStudio (sloop-ios-8trk)](https://github.com/smhulme/sloop-ios-8trk) — Native iOS/iPadOS 8-track workstation (Swift, CoreMIDI) that pairs with an FM-1 running SLOOP: tracks 1–4 are hardware, synchronized over CoreMIDI.
- **FM-1 Easy Guide** — Plain-words beginner's guide to the FM-1 written because the official manual is hard to read and predates the V15 sequencer changes: one-page lessons on every button, first sounds, loops, and beats, plus an interactive follow-along demo.
  - [Site](https://pingywon.github.io/fm1-easy-guide/) — Project page with the 31-page PDF guide and [interactive demo](https://fm1-demo.pingywon.workers.dev).
  - [Code](https://github.com/pingywon/fm1-easy-guide) — Source repository.
- [fm1-emulator](https://github.com/simonjohansson/fm1-emulator) — Rust desktop emulator that runs FM-1 firmware images (`.fwsc`, `.elf`, `.bin`) without a real device.
- [fm1-firmware-patcher](https://github.com/czietz/fm1-firmware-patcher) — Binary patches for the stock V15 firmware (e.g. Dexed-accurate detune); unofficial, so back up first.
- **fm-static** — Web page that installs a `.fwsc` firmware on an FM-1 whose MIDI port has a different name on your computer, where the usual updaters cannot find it.
  - [Site](https://seajaysec.github.io/fm-static/) — Hosted installer.
  - [Code](https://github.com/seajaysec/fm-static) — Source repository.
- [fm1-linux-update](https://github.com/fuleo/fm1-linux-update) — Updates the stock firmware from V14 to V15 from Linux over USB-MIDI SysEx, with verification (M-VAVE only ships Windows and macOS updaters); see also the [fm1-guide](https://fuleo.github.io/fm1-guide/) notes.
- AI-agent skills (Chinese-language, MIT): [Felucca Editor Skill](https://github.com/hunterxiong2026/fm1-felucca-editor-2026) and [SLOOP Editor Skill](https://github.com/hunterxiong2026/fm1-sloop-editor-2026) let an AI agent drive the FM-1 over direct SysEx (Windows) for multi-track arrangement and song playback.
- [Dexed](https://asb2m10.github.io/dexed/) — The open-source DX7 emulator and editor; the FM-1 accepts its single-parameter SysEx, so you can edit voices live.
- [FM-1 Bonus Box](https://github.com/pfkellogg/fm1-bonus-box) — ESP32-S3 companion box adding a sustain pedal, a rotary preset browser with a round TFT, a WiFi soundbank manager, and USB MIDI; its [fm1-sustain-footswitch](https://github.com/pfkellogg/fm1-sustain-footswitch) sibling is a simple Arduino board turning a TRS sustain pedal into MIDI CC64.
- [Virtual FM-1](https://github.com/jbschooley/Virtual-FM-1) — GPL-3.0 software FM-1: a standalone app and VST3/AU plugin (macOS, Windows, Linux) that plays the FM-1's FM engine, edits every sound setting, and runs its sequencer and arpeggiator, with two-way preset and pattern sync (single preset or the whole 128-preset library) over USB with the [FM-1+VA firmware](https://baudgirl.com/work/FM-1+VA). Instances can target stock, FM-1+VA, Felucca, or SLOOP (the last two run from their own source); it works as a standalone synth without the hardware.

## Preset Packs

- [fm1-factory-presets](https://github.com/KingParamount/fm1-factory-presets) — FM-1 factory presets recovered as four standard DX7 bank dumps (piano/organ, guitar/bass, brass/woodwind, percussion/effects), with SysEx protocol notes, an FM synthesis tutorial PDF, and Python decoding tools.
- [DXcompanion.uk patch catalog](https://dxcompanion.uk/) — Four curated DX7 banks (best-of, drums/percussion, orchestral, extras/SFX) built from FM staples, DOS, and Sega Genesis game sounds; loadable via SysEx.
- [Digital X7](https://squaresawsound.gumroad.com/l/digital-x7) — Commercial DX7-compatible patch bank usable on the FM-1 via SysEx import.
- [Engedal's Yamaha DX7 presets](https://engedal.gumroad.com/l/cFMYB) — Commercial DX7 patch collection compatible with FM-1 SysEx import.
- [This DX7 Cartridge Does Not Exist](https://www.thisdx7cartdoesnotexist.com/) — Neural-network-generated DX7 cartridges, fresh on every reload, that load straight into the FM-1.
- [Ambient & Dreams](https://natlifesounds.com/product/ambient-dreams-for-m-vave-fm-1-fm-synthesizers/) — Commercial soundbank by NatLife Sounds made for the FM-1.

## Reverse Engineering

- [fm1-custom-fw](https://github.com/aroum/fm1-custom-fw) — Reverse-engineering research on the FM-1 and the M-UPGRADE updater: JieLi AC791N hardware, teardown and case-opening notes with PCB photos, bootloader and memory map, the SysEx OTA frame layout, signature-verification findings, a SysEx scanner, and an experimental MIDI SysEx firmware flasher (untested on hardware). It also catalogs custom firmwares and JieLi tooling references.
- [FM-1-RE](https://github.com/AL-255/FM-1-RE) — Firmware reverse engineering and update-protocol research: architecture and boot-chain overview, V13/V14 disassembly and function databases, OTA protocol and loader analysis, Windows updater decompilation, Ghidra scripts, and a Linux USB-MIDI OTA client with offline tests. Confirms a Dexed/msfa-derived six-operator FM engine; the `main` branch intentionally contains no replacement firmware (that lives on the `with-custom-firmware` branch).
- [FM-1-transporter](https://github.com/kurogedelic/FM-1-transporter) — Recovery tool referenced by the SLOOP documentation for an FM-1 that no longer starts after a failed custom-firmware install.
- [fm1_flasher.py](https://github.com/aroum/fm1-custom-fw/blob/main/fm1_flasher.py) and [fm1_ota.py](https://github.com/AL-255/FM-1-RE/blob/main/tools/fm1_ota.py) — Standalone CLI flasher and preset uploader from fm1-custom-fw, and the Linux USB-MIDI update client with offline protocol tests from FM-1-RE.
- [USB_KEY dongle notes](https://github.com/ip2k/lunar-modulator/blob/main/docs/10-usb-key-dongle.md) — Lunar Modulator's write-up of the RP2040 dongle that forces the AC791N into download mode over USB-C.
- [fm1-nes](https://github.com/Keitark/fm1-nes) — Experimental resources, board-support code, and a worked example (an NES player) for developing custom firmware on the FM-1's JieLi WL82: source-only SDK integration, build setup, and [application-only updates](https://github.com/Keitark/fm1-nes/blob/main/APP_UPDATES.md) that preserve the stock bootloader; see the [getting started guide](https://github.com/Keitark/fm1-nes/blob/main/GETTING_STARTED.md).
- [fm1-mdx](https://github.com/Keitark/fm1-mdx) and [fm1-doom](https://github.com/Keitark/fm1-doom) — Experimental spin-offs of fm1-nes: an MDX/PDX karaoke player (host-tested, not yet accepted on the FM-1) and a Doom engine port in progress; neither has an installable firmware.
- [fm1-polyseq](https://github.com/NOVALENTI/fm1-polyseq) — Polyphonic 16-step sequencer and hardware abstraction layer in strict C99, written from scratch for the FM-1's pi32v2 core.
- [sloopy-sloop-32](https://github.com/smhgzll/sloopy-sloop-32) — GPL-3.0 proof of concept running SLOOP natively on an ESP32-S3 with a PCM5102A DAC, with a browser standing in for the front panel.
- [Felucca BUILDING.md](https://github.com/hugelton/Felucca/blob/main/BUILDING.md) — How to build a Felucca-family firmware from source.
- [MVAVE-M-UPGRADE-decompiled](https://github.com/entitymar/MVAVE-M-UPGRADE-decompiled) — Decompilation of the official updater application, for research.
- [jielie](https://kagaimiq.github.io/jielie/) — Reference site for the JieLi SoC family the FM-1's AC791N belongs to.
- [FM-1 MIDI Guide](https://m-vave-fm1-midi-guide.up.railway.app/) — Baud Girl's readable MIDI implementation: channels, effect CC map, SysEx, clock sync.
- [FM-1 SysEx protocol](https://github.com/KingParamount/fm1-factory-presets/blob/main/docs/protocol-and-provenance.md) and [OTA protocol docs](https://github.com/AL-255/FM-1-RE/blob/main/docs/io/11-ota-protocol.md) — Handshake, bank transfer, and 7-bit payload encoding, plus USB-MIDI update framing and memory layout.
- [fm1-banks](https://github.com/mene311/fm1-banks) — Themed DX7 bank collection (the 26 "mene311" banks bundled in the FM1 Editor & Librarian catalog).
- [ghidra-jieli](https://github.com/kagaimiq/ghidra-jieli), [jl-misctools](https://github.com/kagaimiq/jl-misctools), [jl-uboot-tool](https://github.com/kagaimiq/jl-uboot-tool) — JieLi toolchain used in the FM-1 reverse engineering: Ghidra processor support for pi32/pi32v2, firmware container utilities, and a UBOOT USB tool.
- [KVR Audio FM-1 thread](https://www.kvraudio.com/forum/viewtopic.php?t=632127) — Long-running community thread tracking firmware updates, SysEx editing support, and third-party tools.
- [Firmware update guide (Medium)](https://medium.com/@shelvindatt02/how-to-update-the-firmware-on-your-m-vave-fm-1-synthesizer-7bc4ea2c3bd5) — Step-by-step walkthrough of the M-UPGRADE SysEx firmware update process.
- [FM-1 firmware tracker (fwradar.com)](https://fwradar.com/p/m-vave-fm-1) — Firmware version history and changelog tracking for the FM-1.

## Community and Reviews

- [Synth Anatomy review](https://synthanatomy.com/2026/07/m-vave-fm-1-review-low-budget-pocket-fm-ynthesizer-with-iconic-sounds.html) — Hands-on review of the budget pocket FM synth.
- [Synth Anatomy: V15 update](https://synthanatomy.com/2026/07/m-vave-fm-1-a-budget-friendly-dx-7-style-desktop-fm-polysynth.html) — Coverage of the V15 firmware update and new features.
- [Synth Anatomy: FM-1+VA](https://synthanatomy.com/2026/09/baud-girl-fm-1-va-custom-m-vave-fm-1-firmware.html) — Coverage of the Baud Girl FM-1+VA custom firmware.
- [Sonicstate: free custom firmware](https://sonicstate.com/news/2026/09/29/free-custom-firmware-for-mvave-fm-1-/) — News coverage of the first free custom firmware for the FM-1.
- [Piano & Synth Magazine: FM-1+VA](https://pianoandsynth.com/m-vave-fm-1-custom-firmware-with-added-virtual-analog-drops/) — Coverage of the FM-1+VA custom firmware release.
- [Synth Anatomy: patch librarian](https://synthanatomy.com/2026/07/m-vave-fm-1-patch-librarian.html) — Coverage of the browser-based patch librarian simplifying DX7 sound transfer.
- [cicloid/awesome-fm-1](https://github.com/cicloid/awesome-fm-1) — Another curated FM-1 list with firmware, tools, and recovery notes.
- [Piano & Synth: custom firmware collection](https://pianoandsynth.com/m-vave-fm-1-custom-firmware-collection/) — Comparison table of the FM-1 custom firmwares.
- [Time To House: FM-1 article](https://timetohouse.com/en/articles/m-vave-fm-1-budget-dx7-fm-synth) — Launch article on the budget DX7-style synth.
- [Noizefield: SLOOP](https://www.noizefield.com/news/sloop-custom-firmware-turns-m-vave-fm-1-into-4-track-groovebox) — News coverage of the SLOOP groovebox firmware.
- [Synthtopia: alt firmware options](https://www.synthtopia.com/content/2026/10/04/alt-firmware-options-for-the-m-wave-fm-1-pocket-synthesizer/) — Roundup of the first alternative firmwares (Felucca, Baud Girl, Groove OS) with demo videos.
- [Drey Andersson: 7 custom firmwares ranked](https://dreyandersson.com/blog/m-vave-fm-1-custom-firmware/) — Comparison and ranking of the FM-1 custom firmwares, noting the scene's pace (dozens of forks within days).
- [Plugg Supply forum thread](https://plugg-supply.net/forum/gear-plugins/m-vave-fm-1-patch-librarian-free-browser-tool-for-dx-7-sound-transfer) — Discussion of the free browser patch librarian for DX7 sound transfer.
- [GitHub topic: m-vave](https://github.com/topics/m-vave) — Repositories tagged with the M-VAVE brand.
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
- [M-Vave FM-1 Review - The $70 Pocket DX-7 (Synth Anatomy)](https://www.youtube.com/watch?v=q3e2zH_-5I8) — Synth Anatomy's video review.
- [M-VAVE FM-1 Sound Import Tutorial (M-VAVE)](https://www.youtube.com/watch?v=zDfeGawNeJU) — Official tutorial on loading DX7 banks over SysEx.
- [Using MIDI CC's with the FM-1 (Maks Makes)](https://www.youtube.com/watch?v=vWRd1A8I3gc) — Working out the effect CC numbers before M-VAVE published them.
- [FM-1 as a Bluetooth MIDI controller (jesuzmario)](https://www.youtube.com/watch?v=Eu2BY2PxT5M) — Driving an iOS synth app over BLE MIDI.
- [Can M-VAVE FM-1 make a FULL SONG? (jesuzmario)](https://www.youtube.com/watch?v=a3yb4juRSuE) — No-talking demo tune using the factory sounds.
- [FM-1 VA full tutorial (NatLife Sounds)](https://www.youtube.com/watch?v=jfuoEBIUsEE) — Walkthrough of the Virtual Analog engine and new sequencer.
- [Felucca 0.9 and new presets (AutoHot, Russian)](https://www.youtube.com/watch?v=UzgbDjsFEpY) — Russian-language walkthrough and sound demo of Felucca 0.9.
- [Felucca first look (Stanley Gurvich)](https://www.youtube.com/watch?v=EzFknmhtKZk) — Multi-sequencer, nine engines, and scale mode.
- [Felucca 0.9-beta jam session (2403R / Case Woo)](https://www.youtube.com/watch?v=XEK4VhsYwCE) — Live performance on Felucca.

## Notes

- Always back up your 128 factory presets before installing custom firmware or bulk-importing SysEx banks.
- Custom firmware (e.g. Groove OS, Felucca, SLOOP, Melodee, X0X, Flowstate, FM-1+VA) and reverse-engineered tools are unofficial and not supported by M-VAVE; read the relevant project's disclaimers before flashing.
- The FM-1's sound engine is Dexed-based, so most DX7 SysEx patches and editors work with minor caveats — check each tool's notes on send/receive support.

## Contributing

Pull requests are welcome. Include the tested firmware version, operating system, and a short description of the resource.
