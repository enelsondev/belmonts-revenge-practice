# Alpha17 controls

## Pause and menu

| Input | Action |
|---|---|
| Start during gameplay | Normal pause |
| Up + Select while paused | Open PRACTICE |
| Up / Down | Navigate lists; adjust values on attribute pages |
| A | Open/confirm the selected item |
| B | Back one level; from the root, close the menu |
| Start or Select in the menu | Close the menu; game remains paused |
| RETURN at root | Close the menu; game remains paused |
| Release, then press Start | Resume gameplay |

Root order: **PRESETS → PLAYER → RULES → RETURN**.

## Presets

PRESETS → BOSSES selects one of the seven stage setups. The first six begin at
the boss-approach stretch; Final starts at its normal stage initialization.
PRESETS → SPEEDRUN TECH offers Cloud TAS Jump, Drac 1 Jump and Drac 2 Jump.

Each initializes its curated scenario with full health, 99 hearts, full whip,
and the selected rules' default weapon. Selecting a preset replaces your current
scenario. Normal deaths use the original respawn path without exhausting lives.
The visible REST number is not a remaining-retry limit.

## Player controls

- HEALTH: change Christopher's current health.
- HEARTS: change current ammunition/hearts.
- EQUIP → WHIP: Leather, Chain or Fire.
- EQUIP → WEAPON: None, Axe, Water or Cross. Up/Down cycles these values.
- EQUIP → DEBUG: toggle X/Y information, including fractional position.

These edits retain your room, location and encounter. Equipment editing can show
BUSY during an attack or while a projectile is active; close/resume and wait for
it to finish. Throw subweapons with the game's normal **Up+B** input.

## Weapon rules

- **US AXE** (default): original weapon1 pickups grant Axe.
- **JP CROSS**: the same pickup locations grant Cross instead. Water is unchanged.

Choosing a rule converts the current Axe/Cross to its corresponding weapon;
None/Water stay selected. Presets follow this rule. Player Controls can still
select any weapon independently. This changes weapon rules, not castle layouts.
The rule is not battery-backed; a fresh boot starts with US rules.
