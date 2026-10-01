# Playshelf downloads

Copies of the third-party parts that [Playshelf](https://github.com/bookwright/Playshelf) downloads when you install an engine. Playshelf always tries the original source first and uses these copies only if it fails, for example because the original was deleted. Every file is pinned by SHA-256 in Playshelf's engine definitions, so a copy is only accepted if it is byte for byte the original.

Nothing here was changed. Each release holds the exact files Playshelf installs, their license, and for programs under the GPL the corresponding source code.

| Release | What | Original source | License |
|---|---|---|---|
| `mkxpz-m5kro-a4f4500` | MKXP-Z universal build for macOS (`Z-universal.zip`) | [m5kro/mkxp-z](https://github.com/m5kro/mkxp-z/releases/tag/launcher), a fork of [mkxp-z](https://github.com/mkxp-z/mkxp-z) | GPL-2.0-or-later; built with OpenSSL, so GPL-3.0 applies to the binary |
| `kawariki-m5kro-2025-01-18` | Kawariki compatibility scripts (`kawariki.zip`, Ruby source) | [m5kro/mkxp-z](https://github.com/m5kro/mkxp-z/releases/tag/launcher), extended from [Orochimarufan/Kawariki](https://github.com/Orochimarufan/Kawariki) | GPL-3.0 |
| `easyrpg-player-0.8.1.1` | EasyRPG Player 0.8.1.1 for macOS | [easyrpg.org](https://easyrpg.org/player/downloads/) | GPL-3.0 |
| `safety-scripts-2185abd` | Scripts that keep NW.js games from starting programs or going online | [m5kro/RPG-Maker-MacOS-Launcher](https://github.com/m5kro/RPG-Maker-MacOS-Launcher/tree/2185abd23119eead10278dc546800350ab1e46a4) | GPL-3.0 |
| `cheat-ui-1.0.3` | Cheat menu for RPG Maker MV/MZ, with the Vuetify and Material Design Icons styles it uses | [paramonos/RPG-Maker-MV-MZ-Cheat-UI-Plugin](https://github.com/paramonos/RPG-Maker-MV-MZ-Cheat-UI-Plugin/releases/tag/v1.0.3), [Vuetify 2.6.3](https://www.npmjs.com/package/vuetify/v/2.6.3), [@mdi/font 6.9.96](https://www.npmjs.com/package/@mdi/font/v/6.9.96) | MIT; icons and font Apache-2.0 |
| `fluidr3-gm-3.1` | FluidR3_GM MIDI soundfont by Frank Wen (Debian's `fluid-soundfont_3.1.orig.tar.gz`) | [Debian](https://packages.debian.org/source/stable/fluid-soundfont) | MIT |

## Source code

- **MKXP-Z:** The build's `Info.plist` names commit `a4f4500` of m5kro's fork; `mkxp-z-source-a4f4500.tar.gz` is that commit. m5kro committed a fix for Japanese file names on macOS (`8124670`) three minutes before uploading the build, so it may be part of it; it is included as `fix-japanese-filenames-8124670.patch`. The libraries mkxp-z bundles are fetched and built by its build files from their own sources.
- **EasyRPG Player:** `easyrpg-player-0.8.1.1-source.tar.gz` is the 0.8.1.1 tag of [EasyRPG/Player](https://github.com/EasyRPG/Player). It uses [liblcf](https://github.com/EasyRPG/liblcf) (MIT).
- **Kawariki, safety scripts, cheat menu, soundfont:** these are the source.

## Not here

- **RPG Maker RTPs.** They belong to Kadokawa, whose license doesn't allow passing them on. Playshelf downloads them from [rpgmakerweb.com](https://www.rpgmakerweb.com/run-time-package) only.
- **NW.js.** Playshelf downloads it from [nwjs.io](https://nwjs.io).

Each release lists the SHA-256 of its files.
