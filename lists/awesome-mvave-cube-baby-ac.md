# Awesome M-VAVE Cube Baby AC

> A curated list of official and community resources for the M-VAVE (Cuvave) Cube Baby AC acoustic guitar multi-effects pedal.

## Contents

- [Official](#official)
- [Unofficial Editors](#unofficial-editors)
- [Reverse Engineering](#reverse-engineering)
- [Community and Reviews](#community-and-reviews)

## Official

- [M-VAVE](https://www.m-vave.com/) — Official manufacturer site and product ecosystem, headquartered in Zhuhai, China (brand also sold as Cuvave).
- [M-VAVE Cube Baby AC product page](https://www.m-vave.com/product?id=cube-baby-ac) — Official specifications: electro-acoustic multi-effects processor with 3 editable presets, 3-band EQ, compressor, feedback suppressor, chorus/tremolo, reverb/delay, a 9-slot IR cabinet section (8 classic IRs), Bluetooth music input, and a rechargeable ~6-hour battery.
- [Cube Baby AC manual (PDF)](https://manualf.oss-cn-hongkong.aliyuncs.com/manual/Combined-Effect-Pedals/CUBE-BABY-AC.pdf) — Official user manual, linked directly from the product page.
- [M-VAVE Downloads](https://www.m-vave.com/download) — Official CubeSuite PC software (Windows/Mac) and CubeSuite/SincoOTA mobile apps (iOS/Android) for preset editing and over-the-air firmware updates.

## Unofficial Editors

- **CubeControl** — Unofficial open desktop editor (Windows, Linux AppImage, Android APK) for the M-VAVE/Cuvave CUBE Baby with live A/B/C switching, setlists, and Cabinet 8 IR upload tools; the USB writer is experimental, so export a bank before risky operations. Targets the base CUBE Baby platform, so confirm Cube Baby AC compatibility before writing.
  - [Site](https://mrgarizack.github.io/cubecontrol-app/) — Project page and downloads.
  - [Code](https://github.com/MrGariZack/cubecontrol-app) — Application source; the hardware protocol lives in the companion [cubecontrol](https://github.com/MrGariZack/cubecontrol) core repository.

## Reverse Engineering

- [cuvave-midi](https://github.com/pferreir/cuvave-midi) — Early-stage Rust project reverse-engineering the SysEx MIDI protocol used by the Cuvave Cube Baby platform, documenting a memory map covering presets, USB loopback settings, IR cabinet slots, and RAM/ROM parameter storage; targets the base Cube Baby firmware family shared with the Cube Baby AC.

## Community and Reviews

- [Cuvave/M-Vave Cube Baby AC (Acoustic) para Violão – Review Completo](https://www.youtube.com/watch?v=ASpURJcq_9M) — Full Portuguese-language review by Julio Caliman (158K views) testing whether the pedal is worth it for acoustic guitar.
- [Cuvave/M-Vave Cube Baby AC: Teste de IR's Nylon e Aço!](https://www.youtube.com/watch?v=I5qLkAcvJkI) — Follow-up video by Julio Caliman testing several impulse responses on both nylon- and steel-string acoustic guitar.
- [CUVAVE CUBE BABY ACUSTICO – SEGREDOS REVELADOS!](https://www.youtube.com/watch?v=sw_TBoZ-Kqc) — In-depth Portuguese-language walkthrough by Nando Moraes (392K views) covering setup and tips to improve acoustic guitar tone.
- [Recensione del pedale processore multieffetto acustico M-Vave Cube Baby AC](https://www.youtube.com/watch?v=WHGDkPM1HZA) — Italian-language review by channel soYmartino, demonstrating the pedal in a real playing context.
- [Pedale multieffetto per chitarra acustica M-Vave Cube Baby AC – guida all'uso](https://www.youtube.com/watch?v=k9pIOwwgW4o) — Italian-language usage guide by channel Guitar Learner covering the pedal's menus and effects in detail.

## Notes

- This is a budget/niche acoustic pedal with no coverage found from major gear press (e.g. Premier Guitar, MusicRadar, GearNews); community coverage found is mostly Italian- and Portuguese-language YouTube content rather than English text reviews or forum threads.
- M-VAVE also sells/rebrands this pedal as "Cuvave"; product listings and videos use both names interchangeably.
- The Cube Baby AC is a distinct, acoustic-focused SKU from the standard (electric-guitar) Cube Baby and the Cube Baby Bass — check that any manual, firmware, or preset resource is specific to the AC model before using it.
- Always back up your presets before applying firmware updates via CubeSuite/SincoOTA.

## Contributing

Pull requests are welcome. Include the tested device, firmware version, operating system, and a short description of the resource.
