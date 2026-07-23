# PRAGMATA Grace Mod

A small REFramework Lua mod for **PRAGMATA** that restores Diana's gradual Hacking Gauge auto-recovery ability.

The original game data contains the `HackingGaugeAutoRecovery` parameter with a recovery rate of `0.4`.  
This mod enables the corresponding passive ability at runtime.

## Features

- Restores gradual Hacking Gauge auto-recovery
- Uses the game's original passive/perk parameters
- Does not provide infinite Hacking Gauge
- Does not provide infinite hacking time
- Lightweight Lua script
- Designed for REFramework

## Installation

1. Install REFramework for PRAGMATA.
2. Download the latest release.
3. Copy the included `reframework` folder into the PRAGMATA game directory.
4. The final path should be:

   `PRAGMATA/reframework/autorun/pragmata_grace.lua`

5. Launch the game.

## Uninstallation

Delete:

`PRAGMATA/reframework/autorun/pragmata_grace.lua`

Then restart the game.

## Technical details

The mod uses the game's existing passive perk:

- Perk ID: `4281630528`
- Player parameter: `HackingGaugeAutoRecovery`
- Parameter hash: `4142741604`
- Original Rate: `0.4`

The ability is injected through the runtime perk system.

## Important

This is an unofficial fan-made modification and is not affiliated with or endorsed by CAPCOM.

No PRAGMATA game files are distributed in this repository.

## Requirements

- PRAGMATA
- REFramework

## Compatibility

Tested with the PRAGMATA version available in July 2026.

Future game updates may require changes to the script.

## License

MIT License
