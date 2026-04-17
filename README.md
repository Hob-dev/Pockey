# Pockey

A lighter / stripped-down split keyboard PCB. (Formerly named "OrthusLight" — renamed to Pockey.)

## Status

**Functionally complete** — just a few finishing touches remaining before release.

## ⚠️ Schematic recovery note

The `Pockey.kicad_sch` (originally `OrthusLight.kicad_sch`) and `LeftMatrix.kicad_sch` files were **missing** from the working directory — they were lost sometime after January 2025 and the three most recent backups (dated 2026-04-16) no longer contained them either.

They have been **restored from** `KiCad/backups/Pockey-2025-01-22_173850.zip` — the last backup that still contained the real schematic files. The restored schematic is dated **2025-01-20 14:26** internally. If you did any schematic work between that date and when the file went missing, those changes are not recovered.

## Folder structure

```
Pockey/
├── KiCad/
│   ├── Pockey.kicad_pro / .kicad_pcb / .kicad_prl    Main project
│   ├── Pockey.kicad_sch                              (restored from backup)
│   ├── LeftMatrix.kicad_sch                          (restored from backup)
│   ├── fp-info-cache
│   ├── backups/           Kept 4 dated snapshots (including the one the schematic was recovered from)
│   └── Pockey-backups/    KiCad auto-backup folder (one zip, created on project reopen)
├── Renders/               Pockey_2025-Jan-21 3D CAD render
├── 3D/                    Pockey.step case model
├── Fabrication/           PockeyPCBOutlineV2.dxf, V3.dxf (PCB outline)
└── JLCPCB/                (empty — see "What's missing" below)
```

## What's missing / potentially missing

- **No gerbers / JLCPCB order files.** `JLCPCB/` is an empty placeholder.
- **No BOM / pick-and-place files.**
- **Very few renders** — only a single CAD export from Jan 2025. No WIP/product photos.
- **No STL files** for a printed case — only the `.step` source is included.
- **No sub-schematic for LeftMatrix's .kicad_pro** — only the sch file was recovered.
- **Original Mac-metadata `._*` AppleDouble files and three "bad" 2026-04-16 backup zips** that did not contain the real schematic were intentionally excluded when copying here.

## Original source

All files were copied from `Custom/Ergomania/OrthusLight/` and renamed from `OrthusLight*` → `Pockey*`. The original folder is still intact at that location under its original name.
