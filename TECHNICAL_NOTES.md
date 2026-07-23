# Technical notes

These notes document only the identifiers needed by the mod. Game dumps and proprietary game files are intentionally not included.

## Identified parameter

- `app.PlayerParameterType.HackingGaugeAutoRecovery`
- Hash: `4142741604`
- Parameter class: `app.PeHackingGaugeAutoRecoveryParameter`
- Parameter table entry type: `app.PeDefault`
- Original `Rate`: `0.4`

## Identified perk

- Perk ID: `4281630528`
- The perk contains `HackingGaugeAutoRecovery` and does not contain `HealHackingGaugeRate`.

## Runtime path used

- `app.EnhanceManager`
- `get_CurrentEquipmentPerk()`
- `app.EquipmentPerk._PossessionPerkDict`
- `app.PossessionPerkUnit`
- `app.EquipmentPerk.addPassiveSkill(UInt32)`

The public script retries after save/load transitions because the current `EquipmentPerk` managed object may be recreated.
