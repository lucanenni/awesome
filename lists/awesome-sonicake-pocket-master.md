# Awesome Sonicake Pocket Master

> A curated list of official and community resources for the Sonicake Pocket Master (QME-10).

## Contents

- [Official](#official)
- [Editor Software](#editor-software)
- [NAM and TONE3000](#nam-and-tone3000)
- [Community and Reviews](#community-and-reviews)
- [Demo and Tutorial Videos](#demo-and-tutorial-videos)

## Official

- [Pocket Master product page](https://www.sonicake.com/products/pocket-master) — Official QME-10 page: specs (24-bit/44.1kHz, 100+ effects, 20 amp models, 9 simultaneous blocks, 5 user IR slots, 50 factory + 50 user presets, 1000mAh battery), price, and box contents.
- [Pocket Master software & firmware downloads](https://www.sonicake.com/pages/pocket-master-software-firmware-download-qme-10) — Official download hub with current and historical firmware (latest V1.3.3), Sonicake Manager desktop software (Mac/Windows, "Support NAM A2"), SONICLINK mobile app links, the USB ASIO driver, user manuals, and a Windows 11 connection fix guide.
- [Sonicake Manager](https://www.sonicake.com/pages/pocket-master-software-firmware-download-qme-10) — Desktop manager (V1.5.2, Mac/Windows) already supports NAM A2 files; native A2 support on the device itself needs a firmware update that Sonicake has said is in progress (latest firmware: V1.3.3, which added USB MIDI control).
- [SONICLINK on the App Store](https://apps.apple.com/ug/app/soniclink/id6596747219) — Official iOS/iPad/Mac (Apple Silicon)/Vision Pro app for managing Pocket Master presets, effects parameters, IR import, and backups; also supports Smart Box, AMPCUBE, Amphonix II, and Pilot Whale.
- [SONICLINK on Google Play](https://play.google.com/store/apps/details?id=com.sonicake.soniclink&hl=en_US) — Official Android companion app for editing Pocket Master tones and managing presets/files over Bluetooth.
- [Sonicake QME-10 Pocket Master — Effects Database](https://www.effectsdatabase.com/model/sonicake/pocketmaster) — Independent spec-sheet entry listing the unit as a Bluetooth, IR-capable, USB-controlled amp simulator and headphone amplifier, with reference photos.

## Editor Software

- **Pocket Master Custom Firmware (CFW)** — Unofficial community firmware (CFW 0.9, beta, released 23 October 2026) that runs on top of the official V1.3.3 and installs through Sonicake Manager like any update; its web app is a CFW variant of SonicMaster. It adds two scenes (snapshots) per preset switchable from the pedal or by MIDI CC with spillover, a STOMP mode, MIDI tap tempo, six screen themes with brightness, 10 Clone (NAM) and 10 user IR slots that survive updates, 30-character names, and, from CFW 0.9, six new delays, five new reverbs, a real chorus in FX2, a lighter DSP that no longer freezes when overloaded, and a Global EQ with all seven models; TONE3000 tones can be loaded straight into the Clone and IR slots. A companion web app (installable, with a phone layout) backs up and restores the whole pedal, and a NAM converter and a full user manual are published. Going back to the stock V1.3.3 is documented and was tested (user IRs and Clones must be re-uploaded; presets are kept). The author flags it as beta and warns it is tested only on one unit, may brick other hardware revisions, and can void the warranty.
  - [Site](https://pocketmaster-cfw.guitar-training-generator.com/) — Project page with releases, install steps, and disclaimer.
  - [Manual](https://pocketmaster-cfw.guitar-training-generator.com/manual/) — User manual covering every feature.
  - [Web app](https://pocketmaster-cfw.guitar-training-generator.com/app/) — Companion app for backup, restore, and slot management.
  - [NAM converter](https://pocketmaster-cfw.guitar-training-generator.com/nam-converter/) — Converts `.nam` captures for the Clone slots.
  - [CFW 0.9 release notes](https://pocketmaster-cfw.guitar-training-generator.com/releases/0.9/RELEASE_NOTES.html) — What changed in the latest release.
- [PocketEdit](https://github.com/suckyble/PocketEdit) — Community-built, browser-based editor (HTML/JavaScript, no install) offering a visual signal-chain UI, real-time parameter editing, access to all 50 factory and 50 user presets, JSON preset export/import, and a tap-tempo calculator; connects via USB WebMIDI or Web Bluetooth. Live demo at [suckyble.github.io/PocketEdit](https://suckyble.github.io/PocketEdit/).
- [PocketMasterEdit](https://github.com/erfanrocker/PocketMasterEdit) — Fork of PocketEdit focused on Bluetooth-only real-time editing, with the same preset management and tap-tempo features plus added communication/debug logging; described by its author as built through reverse engineering the device's protocol.
- [pocket-master-mcp](https://github.com/voronkovd/pocket-master-mcp) — Unofficial MIT-licensed MCP server (also on [PyPI](https://pypi.org/project/pocket-master-mcp/)) that lets an AI assistant control a Pocket Master over USB MIDI, plus offline tools to build a firmware file with a translated UI (Russian built in); verified against firmware V1.3.3. Not affiliated with Sonicake.
- **SonicMaster** — Desktop and browser editor for the Pocket Master and Smart Box: preset management, per-effect editing, signal-chain reshaping, footswitch mapping, and NAM/IR importing, built on a hand-reverse-engineered BLE and USB-MIDI protocol (the author notes the code is almost entirely AI-written).
  - [Site](https://skyggedans.github.io/SonicMaster/) — Browser version and downloads.
  - [Code](https://github.com/Skyggedans/SonicMaster) — Source repository.
- [pocket-master-interoperability-guide](https://github.com/klotznick/pocket-master-interoperability-guide) — Independent, hardware-tested notes on the Pocket Master's MIDI command table, vendor editor protocol, and stored-preset format (tested on firmware V1.3.3), with a short getting-started exercise set.
- [pocket-master-tools](https://github.com/dantepeixoto/pocket-master-tools) — Portuguese-language web tools for `.nam` files on the Pocket Master, starting with a gain (dB) adjuster for captures that play too quietly.
- DIY MIDI controllers: [Sonicake-Smart-Box-Controller](https://github.com/DaveC3/Sonicake-Smart-Box-Controller) (ESP32 touchscreen BLE-MIDI controller for the Pocket Master and Smart Box), [Pocket Master + Raspberry Pi Pico 2 W](https://github.com/beankinghk/Sonicake-Pocket-Master-Raspberry-Pi-Pico-2-W), and [NARD_SPM_MidiFootSwitch](https://github.com/bonardalfin/NARD_SPM_MidiFootSwitch) (MIDI foot switch); the last two have no README, so their scope is unverified.
- [PocketMaster Studio](https://github.com/sadurni/PocketMasterStudio) — Single self-contained HTML app that generates, edits, and packages Pocket Master presets in the browser: 482 artist-inspired presets across 260 songs in three amp sets (modeled, NAM clone, mixed), with the PocketEdit editor embedded.
- [pocketmaster-presets](https://github.com/privatefound/pocketmaster-presets) — Free collection of Pocket Master presets inspired by well-known artists, with requests for new ones accepted.
- [Chocotone](https://solispensa.github.io/Chocotone/) — Open-source ESP32/ESP32-S3 MIDI controller configurable from the browser (BLE MIDI and USB MIDI) used with Pocket Master and similar pedals ([source](https://github.com/solispensa/Chocotone)); [PedalPlayground](https://github.com/fede2cr/PedalPlayground) is a CircuitPython Bluetooth controller for Smart Box and similar mini pedalboards.
- [Windows 11 firmware fix for Valeton / Hotone / Sonicake](https://cesardamien.github.io/hotone-family-firmware-fix/) — One-click fix for pedals not detected by the app or firmware updates stuck at 0% on Windows 11 ([source](https://github.com/cesardamien/hotone-family-firmware-fix)); see also Sonicake's [official guidance](https://www.sonicake.com/pages/stuck-updating-support).

## NAM and TONE3000

- [Best Budget NAM Compatible Gear Under $100/$200/$300 — TONE3000](https://www.tone3000.com/blog/best-budget-nam-compatible-gear-under-100-200-300) — Lists the Pocket Master among the most affordable NAM-capable units, noting it can run NAM tones with built-in effects and IR cab simulation via USB or headphones.
- [Sonicake Pocket Master Review: Best Starting Point for NAM Hardware? — tubesandcode.studio](https://tubesandcode.studio/posts/sonicake-pocketmaster-review-budget-nam-hardware) — In-depth review of the unit's 5 NAM + 5 IR slots, explains it uses a proprietary distillation/conversion process rather than native NAM processing, and notes firmware V1.7.2 of Sonicake Manager added NAM A2 model support; 4.5/5 verdict for practice/recording use, not professional touring.
- [Sonicake Pocket Master: NAM models, effects and acoustic guitar IR on the cheap — paniquejazz.com](https://www.paniquejazz.com/2026/02/27/sonicake-pocket-master-neural-amp-modeler-and-acoustic-guitar-impulse-response-on-the-cheap/) — Hands-on account of loading NAM amp captures and acoustic-guitar IRs (including from TONE3000); recommends software V1.1.1 over V1.3.3+ because loaded NAM/IR profiles play back too quietly on the newer version, and covers running the device on USB power for longer sets.
- [SONICAKE POCKET MASTER NAM trial — note.com (Japanese)](https://note.com/decopon110/n/n1ea01905ee08) — Review covering the SONICLINK app workflow for importing free TONE3000 NAM models, and notes that the onboard IR block is disabled while a NAM capture is loaded.
- [Sonicake NAM Captures discussion — The Gear Forum](https://thegearforum.com/threads/sonicake-nam-captures.7753/) — Thread tracking the rollout of NAM/Clone support from firmware V1.1.0, including an early stability issue that led to the firmware being pulled, and later confirmation that loading five NAM profiles works after updating.

## Community and Reviews

- [Sonicake Pocket Master — The Gear Forum](https://thegearforum.com/threads/sonicake-pocket-master.9254/) — General discussion thread covering build quality, headphone output, Bluetooth MIDI (working via switchers as of firmware 1.3.3), inconsistent amp-model quality, and the consensus that stock presets are weak out of the box.
- [Received my Sonicake Pocket Master today. VERY disappointed. — Squier-Talk](https://squier-talk.com/threads/received-my-sonicake-pocket-master-today-very-disappointed.211570/) — Critical user report describing harsh/metallic overdrive and distortion tones and excessive noise requiring a high noise-gate setting; a useful counterpoint to the more positive reviews below.
- [Sonicake Pocket Master Review — backingtracksverse.com](https://backingtracksverse.com/sonicake-pocket-master-review) — Review praising the built-in battery, Bluetooth app editing, and NAM/IR support, while noting only 5 IR slots (versus 20-50 on some competitors) and no XLR outputs; rated 4.2/5.
- [SONICAKE Pocket Master Review (2025) — Tone Authority](https://www.toneauthority.com/%F0%9F%8E%B8-sonicake-pocket-master-review-2025-tiny-pedal-huge-possibilities/) — Review focused on everyday usability: overdrive/distortion for classic rock and light metal, delay/reverb for ambient and indie tones, and headphone-based silent practice.

## Demo and Tutorial Videos

- [Sonicake Pocket Master Full Review & Demo](https://www.youtube.com/watch?v=pDynmUf70MQ) — Full walkthrough covering specs, software, connections, preset editing, and demos of effects, overdrive/distortion, amp models, delay, and reverb.
- [Sonicake Pocket Master QME-10 Tutorial](https://www.youtube.com/watch?v=fIeuMnW_6Cc) — Guided tour of setup, controls, connectivity options, and customizing settings on the device.
- [Sonicake Pocket Master for Beginners](https://www.youtube.com/watch?v=zv1zDyFmArc) — Beginner-oriented video on onboard features and MIDI integration.

## Notes

- Always back up presets before updating firmware or installing third-party editor software.
- NAM and IR slots share resources: on current firmware, loading a NAM capture disables the onboard IR block, and NAM/IR support can behave differently (including playback volume) across firmware and Sonicake Manager versions — check reviews above before updating.
- Community editors (PocketEdit, PocketMasterEdit) rely on a reverse-engineered protocol over USB WebMIDI or Web Bluetooth; they are not official Sonicake tools, so test on a spare preset slot first.
- Reported real-world experiences vary significantly, from very positive to very negative — read multiple reviews rather than relying on a single source before buying.

## Contributing

Pull requests are welcome. Include the tested device, firmware version, operating system, and a short description of the resource.
