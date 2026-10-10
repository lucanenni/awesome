# Awesome JBL BandBox

> A curated list of official and community resources for the JBL BandBox Solo and BandBox Trio portable guitar amp and Bluetooth speaker with Stem AI.

## Contents

- [Official](#official)
- [Unofficial Tools and Protocol Research](#unofficial-tools-and-protocol-research)
- [Community and Reviews](#community-and-reviews)

## Official

- [JBL BandBox Trio](https://www.jbl.com/BANDBOX-TRIO.html) — Official Trio product page.
- [JBL BandBox Solo & Trio](https://www.jblonlinestore.com/pages/bandbox-solo-trio-ai-amplifier) — JBL online store overview of both models.
- [BandBox Solo owner's manual (PDF)](https://www.jbl.com/on/demandware.static/-/Sites-masterCatalog_Harman/default/dwcf2248e5/pdfs/JBL%20BandBox%20Solo_OM_Global_SOP_EN_V7.pdf) — Official Solo manual: 60-second looper, Stem AI practice workflow, inputs and outputs, charging, and auto power-off.
- [BandBox Trio owner's manual (PDF)](https://www.jbl.com.mx/on/demandware.static/-/Sites-masterCatalog_Harman/default/dw5e85e201/pdfs/JBL_BandBox_Trio_OM_Global_EN_V5.pdf) — Official Trio manual.
- [BandBox Solo input/output guide](https://support.jbl.com/us/en/howto/bandbox-solo-input-output-guide-mnjc906jejc-us/000054291.html) — Official support guide to the Solo's connections.
- [JBL One on the App Store](https://apps.apple.com/us/app/jbl-one/id1610239857) and [on Google Play](https://play.google.com/store/apps/details?id=com.jbl.oneapp) — Official companion app for presets, effect chains, EQ, looper options, and Stem AI settings.
- [JBL BandBox announcement (Business Wire)](https://secure.businesswire.com/news/home/20260122156056/en/JBL-BandBox-a-Brand-New-AI-Powered-Amp-and-Speaker) — Press release introducing BandBox.

## Unofficial Tools and Protocol Research

- [BandBox Studio](https://github.com/opethlike/bandbox-studio) — Unofficial local macOS control panel and MCP server for the **Trio**: browser GUI and 21 MCP tools to manage presets, 44 amp and effect models, mixer levels, drums, metronome, tuner, and the looper over Bluetooth, without JBL One or a phone. Experimental and tested with a single Trio; also indexed on [Glama](https://glama.ai/mcp/servers/opethlike/bandbox-studio).
- [OpenJBL](https://github.com/NiceDayZc/openjbl) — Safe Bluetooth protocol, EQ, CLI, TUI, and GUI toolkit for JBL portable speakers (37 catalogued models, BLE GATT and Bluetooth Classic SPP, read-back verification of every write). It is not BandBox-specific, but BandBox Studio cites its protocol notes as background.
- [BandFOSS](https://github.com/vforvilela/bandfoss) — Open-source real-time stem separation and mixer for live system audio, in the style of BandBox's Stem AI; it does not control the hardware.

## Community and Reviews

- [Sound On Sound: JBL BandBox Trio](https://www.soundonsound.com/reviews/jbl-bandbox-trio) — Review noting, among other things, that there is no footswitch jack, so loops are controlled from the panel.
- [Guitar World: BandBox Trio review](https://www.guitarworld.com/gear/combo-amps/jbl-bandbox-trio-review) — Hands-on review of the Trio.
- [Guitar World: BandBox Solo review](https://www.guitarworld.com/gear/combo-amps/jbl-bandbox-solo-review) — Hands-on review of the Solo, including how the pitch shifter affects Bluetooth audio only.
- [Guitar World: BandBox launch](https://www.guitarworld.com/gear/amps/jbl-bandbox-stem-ai) — Launch coverage of the amp and Stem AI separation.
- [gearnews.com: BandBox Solo & Trio](https://www.gearnews.com/jbl-bandbox-solo-trio-guitar/) — Overview and impressions of both models.
- [TechRadar: Stem AI speakers](https://www.techradar.com/audio/wireless-bluetooth-speakers/jbls-new-portable-speakers-have-stem-ai-for-jamming-they-can-remove-any-instrument-or-vocal-from-songs-in-realtime-no-internet-required) — Coverage of on-device instrument and vocal separation without an internet connection.
- [Musician reviews: JBL BandBox Solo](https://www.musicngear.com/jbl-bandbox-solo/reviews) — Owner reviews, including a note that there is no effects loop.
- [The Acoustic Guitar Forum: BandBox Solo review thread](https://www.acousticguitarforum.com/forums/showthread.php?t=709923) — Owner impressions with amp settings and a tip about hiss at maximum master volume.
- [Jazz Guitar Forum: JBL Bandbox, Solo and Trio](https://www.jazzguitar.be/forum/guitar-amps-gizmos/106048-jbl-bandbox-solo-trio.html) — Forum thread on both models.

## Notes

- The Trio has no MIDI interface and no footswitch input, and JBL publishes no control protocol: everything beyond the JBL One app is reverse-engineered and can break with app or firmware updates.
- BandBox Studio targets the Trio on macOS only; there are no known third-party tools for the Solo.
- Download JBL One only from the official stores; unofficial mirrors of the app exist.

## Contributing

Pull requests are welcome. Include the tested model, firmware version, operating system, and a short description of the resource.
