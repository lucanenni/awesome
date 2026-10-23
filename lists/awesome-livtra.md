# Awesome LIVTRA

> A curated list of official and community resources for LIVTRA devices: the NANOCORE and MOSAIC pocket multi-effects pedals (which share the ToneCommand and RESONA software and the same firmware line), the NEXFOOT dual-mode MIDI controller, and the SKYTUNER polyphonic tuner pedal; the VELRIX is mentioned where it overlaps.

## Contents

- [Official](#official)
- [Unofficial Editors](#unofficial-editors)
- [Manuals](#manuals)
- [Community and Reviews](#community-and-reviews)
- [Videos](#videos)

## Official

- [LIVTRA downloads](https://livtramusic.com/downloads) — Official firmware, ToneCommand software, manuals, and release notes for NANOCORE and other LIVTRA devices.
- [LIVTRA NANOCORE product page](https://livtramusic.com/products/nanocore/content-en.html) — Official product information covering effects, RESONA-ready captures, imports, software, and custom themes.
- [LIVTRA Music](https://livtramusic.com/) — Official LIVTRA site with product information for NANOCORE, MOSAIC, VELRIX, and related devices.
- [LIVTRA news](https://livtramusic.com/news) — Official news: the VELRIX firmware and LIVTRA desktop apps added NAM A2 support (June 2026), and ToneCommand Upgrader 1.2.6 added editing for the new NANOCORE/MOSAIC firmware 1.10 effects and parameters.
- [ToneCommand for Android](https://play.google.com/store/apps/details?id=com.livtra.nanocore) — Android companion app for connecting to NANOCORE, editing presets, managing blocks, and importing/exporting bundles.
- [LIVTRA MOSAIC product page](https://livtramusic.com/products/mosaic/content-en.html) — Official page for the MOSAIC mobile multi-effects processor (three metal footswitches, NAM A2 and IR loader), the larger sibling of the NANOCORE that shares its editing software and firmware 1.10 updates.
- [LIVTRA NEXFOOT product page](https://livtramusic.com/products/nexfoot/content.html?embed=1&lang=en) — Official page for the dual-mode MIDI controller: four rotating footswitches (press to trigger, turn to adjust), MIDI and PEDAL (bank-based) modes, a color display, USB-C, Bluetooth, USB-A host and 3.5 mm TRS MIDI out, and an expression input; assignments can be edited on the unit or in ToneCommand.
- [LIVTRA SKYTUNER product page](https://livtramusic.com/products/skytuner/content.html?embed=1&lang=en) — Official page for the guitar and bass tuner pedal: automatic single-note and polyphonic tuning, a 1.8-inch color display, MON continuous monitoring, true or buffered bypass, support for six- and seven-string guitars and four- and five-string basses (with Drop D, Drop A, and down tunings), and 9 V DC or USB power.
- [LIVTRA products](https://livtramusic.com/products) — Official product index for the whole range.
- [RESONA](https://livtramusic.com/resona) — Official tone-capture technology and desktop app that turns NAM A2 captures into LIVTRA's `.ead`/`.eadl` format for the MOSAIC and NANOCORE; LIVTRA says full RESONA is more accurate than the quick "Flash" import done by dragging an A2 file into ToneCommand (vendor claim).

## Unofficial Editors

- **NanoCore Editor** — Unofficial online editor for NANOCORE, verified against real hardware with firmware 1.04 and later.
  - [Site](https://lucanenni.github.io/livtra-nanocore-editor/) — Hosted online editor.
  - [Code](https://github.com/lucanenni/livtra-nanocore-editor) — Source repository.
- [nanocore-controller](https://github.com/dvilelaf/nanocore-controller) — Unofficial local control for the NANOCORE: a command-line tool, Python library, and web editor over Bluetooth or USB MIDI, with lossless backup/restore and an audit log of every write; firmware updates are not implemented and the protocol was reverse-engineered from the official ToneCommand app. Writes to the pedal's flash, so keep a backup.
- [skytuner-ui](https://github.com/LIVTRA-Audio/skytuner-ui) — SkyTuner UI Toolkit 1.00: a Python toolkit and desktop app for building your own **SKYTUNER** theme (backgrounds, note fonts, meters, header and footer rows, startup animation), with previews and upload over USB and several examples; Windows is the tested platform and it expects the latest SKYTUNER firmware from ToneCommand. The `LIVTRA-Audio` GitHub organization was created on 23 October 2026, is unverified, and is not linked from livtramusic.com at the time of writing, so confirm its provenance before uploading anything to your tuner.
- [LivtraNanocore (Arduino MIDI controller)](https://github.com/Xander-Electronics/LivtraNanocore) — Arduino MIDI controller project for the NANOCORE. Unverified: the repository has no README yet.
- [JimCommanD](https://github.com/3rud1te/JimCommanD) — Independent, experimental (0.3.1) Intel-Mac controller for the **MOSAIC**: native CoreMIDI app with a simulator and local libraries, built because the inspected ToneCommand builds shipped only Apple Silicon binaries; NAM/IR uploads and firmware updates are unfinished. Its protocol research may also help with the NANOCORE.

## Manuals

- [NANOCORE user manual](https://ae-pic-a1.aliexpress-media.com/kf/Sf935a7af6cb64376869faa22e0bdc334i.pdf) — User manual mirror covering editing, saving tones, connections, and USB-C recording.

## Community and Reviews

- [LIVTRA MOSAIC (VGuitar Forums)](https://www.vguitarforums.com/smf/index.php?topic=40257.0) — Community thread with the firmware 1.10 release notes (new Gate release, Auto Gate sensitivity and release, Motion Wah on FX2, new MOD effects, click fixes) and notes on converting NAM A2 files through RESONA or ToneCommand; it also lists a 1.11 section that could not be confirmed on the official downloads page.
- [Livtra Velrix – new NAM / IR pedal (VGuitar Forums)](https://www.vguitarforums.com/smf/index.php?topic=39838.0) — Thread on the sibling VELRIX pedal that shares the software ecosystem.
- [LIVTRA NEXFOOT MIDI Controller 2-in-1 Dual Mode Pedal (VGuitar Forums)](https://www.vguitarforums.com/smf/index.php?topic=40241.0) — Community thread on the NEXFOOT.
- [LIVTRA SKYTUNER – Poly Tuner / Oscilloscope / Spectrum Analyser (VGuitar Forums)](https://www.vguitarforums.com/smf/index.php?topic=40242.0) — Community thread on the SKYTUNER; the poster reports that its manual describes spectrum analyzer and oscilloscope views (unverified, no review yet).
- [NexFoot by Livtra (rockboard PedalPedia)](https://www.rockboard.de/en/pedalPedia/Livtra/NexFoot/8754633219/) — Spec sheet for the NEXFOOT.
- [Livtra Mosaic specs (Stompbox Garden)](https://www.stompboxgarden.com/gear/pedal/17848/livtra-mosaic) — Spec sheet: headphone output, Bluetooth audio and MIDI, mobile and desktop editing, built-in battery.

## Videos

- [Free NANOCORE tones video](https://www.youtube.com/watch?v=f8z6Z2T2w28) — Video offering four free NANOCORE tones—clean, chorus, crunch, and solo—with download links in the description.
- [NANOCORE review and ToneCommand walkthrough](https://www.youtube.com/watch?v=hIfY65IPULc) — Portuguese review covering ToneCommand, EQ, audio separation, drum loops, capture downloads, themes, and firmware updates.
- [Pocket review Livtra Mosaic (Caverna Guitars)](https://www.youtube.com/watch?v=cVF9JxpcvfQ) — Hands-on pocket review of the MOSAIC.
- [A $60 Quad Cortex? Livtra Mosaic (Vito Astone Music)](https://www.youtube.com/watch?v=pR2kzWjjq5g) — Review and demo of the MOSAIC.
- [MOSAIC working-musician review (note.com)](https://note.com/arai_shoma/n/ne97b8dded8a4) — Written review of the MOSAIC finding its Stomp Mode smooth and usable live, with some reservations about the tuner.
- [Mosaic by Livtra (rockboard PedalPedia)](https://www.rockboard.de/en/pedalPedia/Livtra/Mosaic/8632704377/) — Spec sheet: three metal footswitches, color TFT display, wireless mobile and desktop editing.
- [Livtra Mosaic – Revisión y Test (Daniel Carreto)](https://www.youtube.com/watch?v=jcgCXHJnyzM) — Spanish-language review and test of the MOSAIC.
- [Livtra Mosaic – Tutorial de actualización de firmware (Daniel Carreto)](https://www.youtube.com/watch?v=IAzHk2ILXdU) — Spanish-language walkthrough of updating the MOSAIC firmware.

## Notes

- Little independent material exists yet for the NEXFOOT and SKYTUNER: apart from the skytuner-ui theme toolkit, no editors, firmware projects, or independent reviews were found, so the entries above are mostly the official pages and early forum threads.
- Always back up presets before updating firmware or importing third-party files.
- Verify exact model and firmware compatibility before using a preset or software package.
- Unofficial mirrors and community resources should be checked against the manufacturer’s documentation.

## Contributing

Pull requests are welcome. Include the tested device, firmware version, operating system, and a short description of the resource.
