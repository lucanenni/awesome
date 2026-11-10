# Awesome M-VAVE Other Products

> A curated list of community resources for smaller M-VAVE (Cuvave) products that do not have a list of their own: Tank-B, Pocket AMP, IR Box, SMC-PAD and MK-300.

## Contents

- [Official](#official)
- [Tank-B](#tank-b)
- [Pocket AMP](#pocket-amp)
- [IR Box](#ir-box)
- [SMC-PAD](#smc-pad)
- [MK-300](#mk-300)
- [Notes](#notes)
- [Contributing](#contributing)

## Official

- [M-VAVE Product Ecosystem](https://www.m-vave.com/products) — Official product overview for the whole range.
- [M-VAVE Downloads](https://www.m-vave.com/download) — Official firmware, the M-EFCS editor (PC and mobile; it supports TANK-G, TANK-B, BLACKBOX, STATION-G, STATION-B, Tank Mini, Pocket AMP, SP100, MK300 and MK20) and the updaters.
- [M-VAVE app downloads](https://www.m-vave.com/appdownload) — Official mobile app downloads.
- [Effects Description (PDF)](https://manualf.oss-cn-hongkong.aliyuncs.com/manual/Combined-Effect-Pedals/Effects-Description.pdf) — Official description of the effects of the combined-effect pedals.
- [M-VAVE × TONE3000](https://www.m-vave.com/tone3000) — Official page on the TONE3000 (NAM) collaboration.
- [M-VAVE forum](https://forum.m-vave.com/) — Official forum, including firmware update summaries.

## Tank-B

- [tank_profile_pack](https://github.com/magicBorscht/tank_profile_pack) — Pack of bass amp profiles (`.am2Data`) made for the Tank-B, with EQ and volume adjusted; no licence declared.

## Pocket AMP

- [Pocket AMP Upgrader](https://vitoramaral10.github.io/pocket-amp-upgrader/) — GPL-3.0 app (beta, Windows, macOS and Linux) that sends the official V1.05 `.fwsc` to the Pocket AMP and its clones (such as the Coolmusic PIXIE1) over USB-MIDI, because M-VAVE's own updater runs only on Windows ([source](https://github.com/vitoramaral10/pocket-amp-upgrader)).

## IR Box

- [mvave-irbox-tools](https://github.com/marco-jardim/mvave-irbox-tools) — MIT unofficial editor and toolkit over USB-MIDI: edit presets, upload impulse responses, adjust EQ and volume, back up and restore all 32 slots; the protocol is verified on firmware `IR-BOX_010`.

## SMC-PAD

- [M-Vave for Home Assistant](https://github.com/SDR3078/mvave-home-assistant) — MIT integration (v0.2.0) that turns the SMC-PAD into a house control surface over Bluetooth LE, with sixteen lit pads and eight encoders.
- [mvave-smc-pad-ableton](https://github.com/SDR3078/mvave-smc-pad-ableton) — Ableton Live Remote Scripts for the SMC-PAD (clip launcher and a step sequencer) with a measured MIDI reference, since the manufacturer publishes none; no licence declared.

## MK-300

- [mk300ctl](https://github.com/rafaelsupport/mk300ctl) — Portuguese-language open-source Linux control tool over Bluetooth LE, an alternative to M-EFCS; experimental, reverse-engineered, use at your own risk; no licence declared.

## Notes

- These products share the M-EFCS editor; resources for other models are not interchangeable.
- Community tools write over reverse-engineered protocols: back up first.

## Contributing

Pull requests are welcome. Include the tested device, firmware version, operating system, and a short description of the resource.
