# Awesome LIVTRA

> A curated list of official and community resources for the whole LIVTRA range: the NANOCORE and MOSAIC multi-effects pedals (sharing the ToneCommand and RESONA software), the VELRIX amp and cab pedal, the AETHER, CORVEN, and ZENITH effects pedals, the NEXFOOT, MidiLink, and FLUX controllers, the SKYTUNER tuner, and the WS15 and WS16 wireless in-ear systems.

## Contents

- [Official](#official)
- [Devices](#devices)
- [Unofficial Editors](#unofficial-editors)
- [Manuals](#manuals)
- [Community and Reviews](#community-and-reviews)
- [Videos](#videos)

## Official

- [LIVTRA downloads](https://livtramusic.com/downloads) — Official download center: ToneCommand Upgrader for Windows and macOS (version 1.3.2 added support for NANOCORE and MOSAIC firmware 1.12), firmware, manuals, and release notes for the whole range.
- [LIVTRA Music](https://livtramusic.com/) — Official LIVTRA site.
- [LIVTRA products](https://livtramusic.com/products) — Official product index.
- [LIVTRA news](https://livtramusic.com/news) — Official news: the VELRIX firmware and desktop apps added NAM A2 support (June 2026), and updates such as AETHER 1.06, CORVEN 1.05, VELRIX 1.05, and ZENITH 1.05 are announced here.
- [RESONA](https://livtramusic.com/resona) — Official tone-capture technology and desktop app that turns NAM A2 captures into LIVTRA's `.ead`/`.eadl` format for the MOSAIC and NANOCORE; LIVTRA says full RESONA is more accurate than the quick "Flash" import done by dragging an A2 file into ToneCommand (vendor claim).
- [ToneCommand for Android](https://play.google.com/store/apps/details?id=com.livtra.nanocore) — Android companion app for connecting to NANOCORE, editing presets, managing blocks, and importing/exporting bundles.

## Devices

Official product pages for every LIVTRA device.

**Multi-effects**

- [LIVTRA NANOCORE product page](https://livtramusic.com/products/nanocore/content-en.html) — Official product information covering effects, RESONA-ready captures, imports, software, and custom themes.
- [LIVTRA MOSAIC product page](https://livtramusic.com/products/mosaic/content-en.html) — Official page for the MOSAIC mobile multi-effects processor (three metal footswitches, NAM A2 and IR loader), the larger sibling of the NANOCORE that shares its editing software and firmware 1.10 updates.

**Amp & cab, delay, reverb, and modulation pedals**

- [LIVTRA VELRIX](https://livtramusic.com/products/velrix) — Amp and cab pedal: three-band preamp with gain and master, 9 preamps and 9 cabinets that can be freely combined, import of NAM neural amp models and third-party IRs (1024/2048 samples), a built-in FX loop, and a USB-C audio interface.
- [LIVTRA AETHER](https://livtramusic.com/products/aether) — Reverb pedal: nine stereo reverbs (Room, Plate, Hall, Concert Hall, Ambience, Cloud, Spring, Shimmer, Swell), pre-delay, a PARA parameter, infinite hold, DSP or pure-analog bypass, and a USB-C audio interface.
- [LIVTRA CORVEN](https://livtramusic.com/products/corven) — Delay pedal: nine stereo delays (Digital, Tape, BBD, Duck, Smear, Reverse, Ice, Lofi, Mod), Haas widening with ping-pong, tap tempo with freeze, DSP or analog bypass, and a USB-C audio interface.
- [LIVTRA ZENITH](https://livtramusic.com/products/zenith) — Modulation pedal: nine stereo algorithms (Chorus, Synth Chorus, Phaser, Flanger, Tremolo, Vibrato, Rotary, Uni-Vibe, Auto-Wah), two PARA knobs, tap tempo, pure-analog bypass, and a USB-C audio interface.

**Controllers and utilities**

- [LIVTRA NEXFOOT product page](https://livtramusic.com/products/nexfoot/content.html?embed=1&lang=en) — Official page for the dual-mode MIDI controller: four rotating footswitches (press to trigger, turn to adjust), MIDI and PEDAL (bank-based) modes, a color display, USB-C, Bluetooth, USB-A host and 3.5 mm TRS MIDI out, and an expression input; assignments can be edited on the unit or in ToneCommand.
- [LIVTRA MidiLink](https://livtramusic.com/products/midilink/content.html?embed=1&lang=en) — Wireless MIDI transmission system: 2.4 GHz adapters with bidirectional MIDI, under 3 ms latency, about 10 m unobstructed range, and 5-pin DIN, 3.5 mm TRS, and USB connections, with no charging needed.
- [LIVTRA FLUX](https://livtramusic.com/products/flux/content.html?embed=1&lang=en) — Hands-free page turner with two footswitches and seven control modes (page up/down, arrows, and more), Bluetooth and USB connection, and an independent dual-switch TRS output.
- [LIVTRA SKYTUNER product page](https://livtramusic.com/products/skytuner/content.html?embed=1&lang=en) — Official page for the guitar and bass tuner pedal: automatic single-note and polyphonic tuning, a 1.8-inch color display, MON continuous monitoring, true or buffered bypass, support for six- and seven-string guitars and four- and five-string basses (with Drop D, Drop A, and down tunings), and 9 V DC or USB power.

**Wireless in-ear monitoring**

- [LIVTRA WS15](https://livtramusic.com/products/ws15) — 2.4 GHz wireless IEM system with a charging dock, one-to-many stereo transmission, up to 32 hours of total battery life, and up to 30 m line-of-sight range.
- [LIVTRA WS16](https://livtramusic.com/products/ws16) — 5.8 GHz digital wireless IEM system: 24-bit/48 kHz stereo, six switchable channels, receiver charging in the transmitter, latency down to 8.9 ms, and up to 30 m line-of-sight range.

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
- [Livtra Aether Reverb (VGuitar Forums)](https://www.vguitarforums.com/smf/index.php?topic=39965.0) — Thread on the AETHER reverb and its infinite-hold feature.
- [LIVTRA NANOCORE (VGuitar Forums)](https://www.vguitarforums.com/smf/index.php?topic=39964.0) — Community thread on the NANOCORE.
- [Aether by Livtra (rockboard PedalPedia)](https://www.rockboard.de/en/pedalPedia/Livtra/Aether/8578186665/) and [Livtra Aether specs (Stompbox Garden)](https://www.stompboxgarden.com/gear/pedal/17841/livtra-aether) — Spec sheets for the AETHER.
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
- [Livtra Corven & Aether (Riffs & Rig)](https://www.youtube.com/watch?v=U2b30Jm7Lvk) — Demo of the CORVEN delay and AETHER reverb together; the same channel's [Brazilian-Portuguese version](https://www.youtube.com/watch?v=jrY1z46dU6g) covers the pair too.
- [Budget Livtra Audio stereo reverb pedal, first impressions (David Greer)](https://www.youtube.com/watch?v=IG6SBNEgHYc) and [Fuzz into held reverb demo (David Greer)](https://www.youtube.com/watch?v=QPW9XNaRmeA) — First impressions of the AETHER and a demo of its hold function.

## Notes

- Independent material is thin for the newer devices (NEXFOOT, SKYTUNER, CORVEN, ZENITH, FLUX, MidiLink, WS15, WS16): mostly official pages and a few forum threads and videos. For the NEXFOOT and SKYTUNER: apart from the skytuner-ui theme toolkit, no editors, firmware projects, or independent reviews were found, so the entries above are mostly the official pages and early forum threads.
- Always back up presets before updating firmware or importing third-party files.
- Verify exact model and firmware compatibility before using a preset or software package.
- Unofficial mirrors and community resources should be checked against the manufacturer’s documentation.

## Contributing

Pull requests are welcome. Include the tested device, firmware version, operating system, and a short description of the resource.
