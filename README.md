

# Atari ST/STe for SoCkit

This is a port to SoCkit from Mister port release of 20210224 ([commit](https://github.com/MiSTer-devel/AtariST_MiSTer/tree/13d78631f87202802149441d9781d407b74e46c8)).

Please find rbf binary inside output_files folder.

This core is working with MiSTer main and menu.rbf found in the [MiSTer_SoCkit](MiSTer_SoCkit) folder.

Copy rbf (and possibly MiSTer and menu.rbf) to the root of your SD card.

Following is original ReadMe from MiSTer.
-------------------------------------------------------------------------------------------

# Atari ST/STe for MiSTer (port of MiSTery)

Thanks to Gyorgy Szombathelyi for MiSTery core

Following is original ReadMe from MiST.
-------------------------------------------------------------------------------------------

# MiSTery - An Atari ST/STe core for the MiST board

## Features:

- Cycle accurate STe GLUE+MMU combo (re-created from the [original schematics](https://www.chzsoft.de/asic-web/))
- Cycle accurate [FX68K CPU core](https://github.com/ijor/fx68k)
- Cycle accurate Blitter offered by Jorge Cwik
- Mostly cycle accurate shifter based on [schematics made from reverse engineering](http://www.atari-forum.com/viewtopic.php?t=29658)
- MegaSTe 16 MHz CPU mode
- RAM size up to 14MB
- Support for all TOS versions
- 2 Floppy disc drives
- ACSI hard disc support
- Viking compatible hi-res monochrome card support
- [Real IKBD](https://github.com/harbaum/ikbd) with HD63701 MCU
- Real MIDI input/output using MiST's UART pins
- Serial/parallel port redirect to USB
- Gauntlet type 4 joystick interface support
- STe controller port support
- Optional scandoubled/YPbPr video output

## Usage:

Put the core.rbf and the TOS as tos.img to the SD-Card. TOS/hard disc/floppy images are selectable in the OSD (F12).
With F11, you can toggle between normal and STe joystick ports.

## Current issues/limitations:

- Some MFP imperfections
- Some bugs in ST mode
- No RAM cache for Mega STe
- Missing Ethernec support
- No RTC
- Only fake LMC1992
- PAL clock only (32.084 MHz)
- Since Jagpads have 21 buttons, not all are mapped to MiST controllers when using STe game ports
- No STe paddle handling (but it has 0 software support)

## Thanks to:

- Till Harbaum for the MiST board, original MiST core, new IKBD code
- Jorge Cwik for the FX68K CPU core, FX ST Blitter code and shifter decap
- Christian Zietz for recovering the schematics of the GSTMCU
