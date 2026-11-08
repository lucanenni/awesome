# Awesome M-VAVE Chocolate

> A curated list of official and community resources for the M-VAVE (Cuvave) Chocolate and Chocolate Plus wireless MIDI foot controllers.

## Contents

- [Official](#official)
- [Manuals](#manuals)
- [Unofficial Editors](#unofficial-editors)
- [Reverse Engineering](#reverse-engineering)
- [Community and Guides](#community-and-guides)

## Official

- [M-VAVE Chocolate product page](https://www.m-vave.com/product?id=chocolate) — Official page for the original Chocolate: a pocket-sized four-footswitch wireless MIDI controller (also marketed as a page turner) with a command-feedback display, USB-C charging, and up to 12 hours of use.
- [M-VAVE Chocolate Plus product page](https://www.m-vave.com/product?id=chocolate-plus) — Official page for the Chocolate Plus: Bluetooth 5.0 and USB, a built-in host interface for controlling effects units directly, an advanced custom mode with switchable banks, and a 300 mAh battery (2.5 h charge, up to 12 h of use).
- [M-VAVE Downloads](https://www.m-vave.com/download) — Official CubeSuite and MidiSuite editors, SincoOTA firmware updater, Sinco Connector (Windows BLE), and firmware for both models.
- [M-VAVE app downloads](https://www.m-vave.com/appdownload) — Official desktop and mobile software page.

## Manuals

- [Chocolate Plus user manual (ManualsLib)](https://www.manualslib.com/manual/4522584/M-Vave-Chocolate-Plus.html) — Panel layout, software acquisition, connection, and usage of the Chocolate Plus.
- [Chocolate Plus software instructions (Manuals+)](https://manuals.plus/m/18d70cfaf3529f260e31f644b97214bca665309586d3ba218d1cc2c127ddb028) — Guide to the MIDI editing interface (channel, type, and data fields for PC, CC, Note, and SysEx messages).
- [Chocolate Plus user manual (Manuals+)](https://manuals.plus/asin/B0F8VRKM6K) — Mirror of the Chocolate Plus manual.
- [Chocolate programmable MIDI controller manual (Manuals+)](https://manuals.plus/ae/1005003192985706) — Mirror of the instruction manual for the original Chocolate.
- [Chocolate Plus manual (Notice-Facile)](https://www.notice-facile.com/en/manual/1784538/m-vave+chocolate-plus) — English 10-page manual mirror.

## Unofficial Editors

- **Chocolate Plus custom firmware (dtnprt)** — Modded firmware for the Chocolate Plus (FootCtrlPlus), built by patching the original M-VAVE firmware 012 (checked by SHA-256, no binaries redistributed): shorter footswitch debounce and combo window, short taps no longer dropped, and a custom name/version reply. Flash with SincoOTA with the pedal not paired; at your own risk.
  - [Site](https://dtnprt.github.io/chocolate/firmware/) — Firmware page and build guide.
  - [Code](https://github.com/dtnprt/chocolate-plus-re) — Patch/build scripts, changelog and CubeSuite analysis notes.
- [ChocoEdit](https://github.com/jonpikereally/ChocoEdit) — MIT Morningstar-style macOS editor for the Chocolate Plus: read all settings over USB MIDI, edit Custom MIDI, Mix Key and Custom keyboard modes (up to 16 PC/CC/Note/SysEx messages per switch), write back with an automatic backup and read-back check, `.chocoplus` settings files, live MIDI monitor and a documented SysEx [protocol](https://github.com/jonpikereally/ChocoEdit/blob/main/PROTOCOL.md). Not made or supported by M-VAVE.
- [OpenChocolate](https://github.com/majabojarska/OpenChocolate) — Free, open-source web-based configuration tool for the Chocolate Plus (also known as FC2 / FootCtrl Plus) over Web MIDI SysEx, with no drivers or install: device discovery, configuration read-back, and per-mode views (Program Change banks, per-footswitch CC and latching, advanced custom modes). Runs locally from the repository; no hosted build is published.
- [zoom-ms-chocolate-midi](https://github.com/nilsjesper/zoom-ms-chocolate-midi) — Generates a CubeSuite preset (`.fcp`) so a Chocolate Plus can control an original Zoom MS-50G directly, toggling effects and the tuner and jumping between patches, with no computer in between (stock 3.10 firmware; MIDISTOMP firmware adds effects 4-6 and knob control).
- [katana-gen3-50-chocolate-plus](https://github.com/filhodomauro/katana-gen3-50-chocolate-plus) — Portuguese-language configuration for controlling a Boss Katana Gen 3 50 W amp from a Chocolate Plus.
- [bandbox-midi-bridge](https://github.com/lucanenni/bandbox-midi-bridge) — ESP32-S3 bridge that lets a Chocolate Plus (looper mode 4, plus an expression pedal on the TRS input) control a JBL BandBox Solo or Trio over BLE with no change to the pedal's firmware; see the JBL BandBox list for details.
- [PyFootCtrl](https://github.com/varlen/pyfootctrl) — Python companion app for the Chocolate that implements custom behaviours for the footswitch.
- [altstrument: Chocolate](https://altstrument.org/devices/m-vave-chocolate) — Third-party firmware and tools directory page for the device.
- [mvave-chocolate-tui](https://github.com/WilsonNet/mvave-chocolate-tui) — Terminal UI for configuring the Chocolate on Linux.
- [ChocolatePlus (Ableton)](https://github.com/zwass/ChocolatePlus) — Ableton Live 12 control surface script that lets a Chocolate Plus launch clips in Session View (button B is left unassigned); includes a CubeSuite "Advanced custom mode" preset.
- [TransportCC](https://github.com/cartfisk/TransportCC) — Ableton Live MIDI Remote Script that turns a Chocolate into a transport controller: play, rewind/forward by bar, record, undo, metronome and loop.
- [cq-bluetooth-controller](https://github.com/btafoya/cq-bluetooth-controller) — Raspberry Pi 3B wireless MIDI bridge that lets a Chocolate Plus control an Allen & Heath CQ-20B mixer, with install and read-only deployment scripts and extensive docs.
- [Chocolate Plus × REAPER Guitar Rig](https://github.com/Aditosom/ChocolatyPlus-Reaper-Guitar-Rig) — Windows guitar-rig appliance (FastAPI service driving REAPER via loopMIDI and OSC) to switch Neural DSP amps and presets from a Chocolate Plus and a tablet, with crossfade, tuner, stomp mode and looper; no licence declared.
- [TonexOneController](https://github.com/Builty/TonexOneController) — Apache-2.0 ESP32 controller for the IK Multimedia Tonex One, Tonex Pedal and Valeton GP5; in Bluetooth client mode it uses a Chocolate or Chocolate Plus to switch presets (4 buttons plus bank up/down).

## Reverse Engineering

- [mvave-chocolate-sysex](https://github.com/cbix/mvave-chocolate-sysex) — Early SysEx dumps and observations for the Chocolate, including messages that switch the controller's basic mode (for example to "Program change C") with `aseqsend`; notes that configuration only worked while the official app was connected and that SysEx over BLE MIDI did not.
- [OpenChocolate reverse-engineering notes](https://github.com/majabojarska/OpenChocolate/tree/main/reverse-engineering) — MIDI protocol specification, a protocol addendum with findings from the official apps, USBPcap captures, and a pcapng-to-SysEx extraction script.

## Community and Guides

- [Step-by-step tutorial: Chocolate as a cheap MIDI Bluetooth footswitch for Fractal (Fractal Audio Forum)](https://forum.fractalaudio.com/threads/step-by-step-tutorial-cheap-40-midi-bluetooth-trs-footswitch-for-fractal-m-vave-chocolate.186861/) — Walkthrough of using the Chocolate with a Fractal unit.
- [MIDI "Chocolate" controller with the MOD Dwarf (MOD Audio Forum)](https://forum.mod.audio/t/midi-chocolate-controller-with-the-mod-dwarf-an-introduction/7003) — Introduction to controlling a MOD Dwarf with the Chocolate.
- [M-Vave/Cuvave Chocolate and Chocolate Plus for MIDI control (V-Guitar Forums)](https://www.vguitarforums.com/smf/index.php?topic=38822.0) — Discussion of both models for MIDI control.
- [M-VAVE Chocolate Plus (V-Guitar Forums)](https://www.vguitarforums.com/smf/index.php?topic=37596.0) — Thread on the Chocolate Plus.
- [M-VAVE Chocolate BT Wireless MIDI Controller (Bome Forum)](https://forum.bome.com/t/m-vave-chocolate-bt-wireless-midi-controller-4-footswitch/6386) — Using the Chocolate with Bome MIDI Translator.
- [Raspberry Pi as MIDI host for a Bluetooth MIDI controller (Gist)](https://gist.github.com/pthrrr/7e6d40f720b1a1ebd9618dc95c08bc65) — Making a Bluetooth MIDI controller such as the Chocolate drive a USB MIDI device through a Raspberry Pi.

## Notes

- Always back up your configuration and use the official firmware updater (SincoOTA) when updating; the Chocolate and Chocolate Plus use different firmware (FootCtrl and FootCtrl Plus).
- Community editors target the Chocolate Plus; check model compatibility before writing to an original Chocolate.
- Some manual mirrors are text conversions of the original PDF; rely on the official download page for exact button mappings and current versions.

## Contributing

Pull requests are welcome. Include the tested device, firmware version, operating system, and a short description of the resource.
