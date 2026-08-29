# HP NVS 510 — UEFI GOP 0x10038 Mod

Modified VBIOS for an **HP NVIDIA NVS 510 2GB (GK107)** with an updated NVIDIA UEFI GOP.

## Card identification

- GPU: NVIDIA GK107
- Card: NVS 510 2GB
- PCI Device ID: `10DE-0FFD`
- HP Subsystem ID: `103C-0967`
- Original VBIOS: `80.07.43.00.0D`
- Original UEFI GOP: `0x1000B`
- Updated UEFI GOP: `0x10038` (GK1xx, x64)

## What was changed

Only the UEFI GOP portion was updated using GOP_Updater.

Original VBIOS version remains `80.07.43.00.0D`.

## Tested configuration

- Motherboard: **ASRock Z370 Gaming K6**
- OS: **Windows 11**
- CSM: **Disabled**
- Display output: NVS 510
- Result: motherboard UEFI/BIOS logo and pre-OS display output work correctly with CSM disabled.

Before the GOP update, the same card only showed pre-OS video when CSM was enabled with Legacy Video OpROM.

## Files

- `NVS510_HP_80.07.43.00.0D_GOP_0x10038.rom` — modified working ROM with GOP `0x10038`
- `original/NVS510_HP_80.07.43.00.0D_original.rom` — original ROM dumped from the card before modification

## Important

This is an **unofficial modified VBIOS** and is not an HP/NVIDIA factory BIOS.

The modified ROM was tested on an HP NVS 510 with subsystem `103C-0967`. Compatibility with other NVS 510 revisions/OEM variants is not guaranteed.

**Keep a backup of your original VBIOS before flashing any modified ROM.**

## SHA-256

Modified:
`7023b8e52239f10d846225cd56b0d4be31d38ce4281c8d309eba83f58188afbe`

Original:
`47ff85f8e782894d1e9ca145031487e2e4d978edea50f90caa47efe86cd93723`
