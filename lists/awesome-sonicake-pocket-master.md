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
- [SONICLINK on the App Store](https://apps.apple.com/ug/app/soniclink/id6596747219) — Official iOS/iPad/Mac (Apple Silicon)/Vision Pro app for managing Pocket Master presets, effects parameters, IR import, and backups; also supports Smart Box, AMPCUBE, Amphonix II, and Pilot Whale.
- [SONICLINK on Google Play](https://play.google.com/store/apps/details?id=com.sonicake.soniclink&hl=en_US) — Official Android companion app for editing Pocket Master tones and managing presets/files over Bluetooth.
- [Sonicake QME-10 Pocket Master — Effects Database](https://www.effectsdatabase.com/model/sonicake/pocketmaster) — Independent spec-sheet entry listing the unit as a Bluetooth, IR-capable, USB-controlled amp simulator and headphone amplifier, with reference photos.

## Editor Software

- [PocketEdit](https://github.com/suckyble/PocketEdit) — Community-built, browser-based editor (HTML/JavaScript, no install) offering a visual signal-chain UI, real-time parameter editing, access to all 50 factory and 50 user presets, JSON preset export/import, and a tap-tempo calculator; connects via USB WebMIDI or Web Bluetooth. Live demo at [suckyble.github.io/PocketEdit](https://suckyble.github.io/PocketEdit/).
- [PocketMasterEdit](https://github.com/erfanrocker/PocketMasterEdit) — Fork of PocketEdit focused on Bluetooth-only real-time editing, with the same preset management and tap-tempo features plus added communication/debug logging; described by its author as built through reverse engineering the device's protocol.

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
