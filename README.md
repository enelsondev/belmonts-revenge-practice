# Belmont's Revenge Practice ROM

A fan-made practice patch by **SiREJ** for **Castlevania II: Belmont's Revenge (US)**.

**[Download alpha17](https://github.com/enelsondev/belmonts-revenge-practice/releases/tag/alpha17)**

Download `BelmontsRevengePractice-alpha17.zip` from **Assets** and extract it.
You need your own matching US ROM. This project distributes an IPS patch, not
the original game or a playable ROM. No ROM downloads are provided.

## Quick start

1. Follow [PATCHING.md](PATCHING.md) to check your original US ROM and apply the patch.
2. Save the patched game as a new `.gb` file and cold-boot it in your emulator.
3. Press **Start** to pause, then hold **Up + Select** to open PRACTICE.
4. Use Up/Down and A to select; B goes back. Close the menu and press Start to resume.

[Complete controls](CONTROLS.md) | [Known issues](KNOWN_ISSUES.md) | [Changes](CHANGELOG.md)

## Features in alpha17

- In-game practice menu: **PRESETS, PLAYER, RULES, RETURN**.
- Boss-approach presets for Cloud, Crystal, Rock, Plant, Dracula 1 and Dracula 2;
  Final initializes at its normal stage entrance.
- Speedrun Tech checkpoints: **Cloud TAS Jump, Drac 1 Jump, Drac 2 Jump**.
- Independent health, hearts, whip and subweapon controls.
- **Axe, Holy Water and the Japanese Cross**, including Cross artwork.
- US Axe / JP Cross weapon-pickup rules; US castle layouts remain the base.
- Optional X/Y and fractional-coordinate display.
- Unlimited retries through the normal death/respawn path.

Presets start with full health, 99 hearts, full whip, and Axe under US rules or
Cross under JP rules. Independent Player controls do not relocate Christopher.
JP rules do **not** require a Japanese ROM from players.

Movement-speed options are experimental work and are **not included in alpha17**.

## Compatibility and reporting

Validated in **BGB 1.6.6** and playtested on stream. MiSTer/hardware compatibility
has not yet been verified. Older emulator save states can resume incompatible
code/data: use a fresh boot when changing builds, then create new states.

Found a bug? [Open an issue](https://github.com/enelsondev/belmonts-revenge-practice/issues/new/choose)
with the build, emulator/core, rules, preset/route, and steps. Do not attach ROMs
or emulator save states to public issues.

This repository contains public release materials only. Development is maintained
separately. See [credits and notices](CREDITS.md).
