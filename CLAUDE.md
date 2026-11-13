# Radiation FX Overhaul by Expand

Standalone radiation mod for G.A.M.M.A., meant for other players too (no dependency on Expand's modpack).
Shipped readme: `src/readme.md` (all features, MCM options, compatibility).

## Files
- `src/gamedata/scripts/zzz_rad_geiger_overhaul.script`: main logic (log tag `[zzz_rad_geiger_overhaul]`).
- `src/gamedata/scripts/zzz_rad_geiger_overhaul_mcm.script`: MCM menu (tab without author name; credit on the page).
- `src/gamedata/configs/mod_system_zzzz_rad_geiger_overhaul_postprocess.ltx`: removes radiation grain/noise.
- `src/gamedata/configs/text/{eng,rus}/ui_mcm_rad_geiger_overhaul.xml`: strings (rus = Windows-1251).

## Version
The version is part of the zip name ("Radiation FX Overhaul by Expand 2.1.0"). It appears in: `mod.json`,
`src/readme.md` title, header line of `zzz_rad_geiger_overhaul.script`.

## Decisions (keep)
- Replaces "Radiation_Overhaul - Silent Radiation" and "No geiger sound in my head".
  Must work with or without: Grain RGB & Psi Color Effects Remover, DAR Dosimeter Enhanced,
  G_FLAT's Msv Above Radiation Icon, G.A.M.M.A. Minimalist HUD, UI Rework G.A.M.M.A. Style.
- Geiger ticks only with a geiger counter with a charged battery anywhere in the inventory.
  MCM "Radiation Geiger Sound Sources": internal / external / only in detector slot. "Only in hand" was dropped.
- Optional DAR Dosimeter Enhanced integration (MCM toggle, no dependency); DAR mode saved in the mod's save data.
- No radiation grain (optional film grain in MCM, off by default).
- HUD rad bar shows 0 without a charged geiger. HUD icon has 5 modes; inventory tooltip dose: always hidden or
  "???" without a charged geiger.
- Not touched: Wearable Devices radiation displays, DAR self-scan, item stats (smokes/drinks).
- Campfire regen from Silent Radiation is intentionally gone (separate mod later, see ROADMAP.md).

## Check in game
After loading a save the log shows `[zzz_rad_geiger_overhaul]` lines saying what was patched.
