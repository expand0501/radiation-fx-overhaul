**Radiation FX Overhaul by Expand 2.1.1**

For S.T.A.L.K.E.R. Anomaly G.A.M.M.A. Author: Expand

Standalone: needs no other radiation mod.

**What it does**
1. Geiger ticks play only when you carry a geiger counter (anywhere in the inventory) whose battery has charge. Without one there are no clicks, even when irradiated (replaces "No geiger sound in my head").
   Radiation Geiger Sound Sources (MCM):
   - Play for internal radiation (default on): clicks for your own dose
   - Play for external radiation (default on): clicks while you stand in a radiation field
   - Only with geiger in detector slot (default off): the charged geiger must be in the detector slot (sound only)
   - DAR Dosimeter Enhanced integration (default on, used only if DAR is installed): overrides internal/external.
     Environment mode = environment clicks; contamination mode = body clicks; DAR self-scan mode = environment clicks (DAR plays body clicks during the self-scan).
     The DAR dosimeter mode is saved with the game and restored on load (one value in this mod's save data; harmless if the mod or DAR is removed later).
   Geiger clicks from other scripts (G.A.M.M.A.'s "Geiger panic while gaining rads" from Scrunkly's Collection, and Anti-lag's copy of it) count as external radiation clicks: they need a charged geiger counter, follow the detector slot setting, and play only with "Play for external radiation" on or in DAR's environment mode.
2. No radiation grain on screen (vanilla radiation effect and radioactive zone post-process).
   MCM "Film grain" (off by default): brings back the radiation film grain; its strength follows your own dose and the radiation around you. With Grain RGB & Psi Color Effects Remover installed the grain is invisible, because that mod blanks the effect.
3. The HUD radiation bar (SidHUD bar from G.A.M.M.A. Minimalist HUD) shows 0 without a charged geiger counter.
4. Inventory (UI Rework G.A.M.M.A. Style): the radiation icon still lights up and its tooltip still opens. MCM option for the dose line:
   - Always hidden: the dose is removed from the tooltip (the radiation removal rate of your gear stays)
   - Shown only with charged geiger (default): "???" without a charged geiger counter, the real mSv value with one
   Without UI Rework the inventory shows no dose at all, so nothing is changed there.
5. HUD radiation status icon, MCM option (Radiation FX Overhaul tab):
   - Hidden
   - Shown, mSv only with charged geiger (default): G_FLAT's "Msv Above Radiation Icon" (part of base G.A.M.M.A.) writes the dose above the icon only while you carry a charged geiger counter
   - Shown, never mSv
   - Only with charged geiger: no icon at all without a charged geiger counter; with one, the icon and the mSv value above it are shown
   - Only with charged geiger, no mSv: the icon appears only with a charged geiger counter, never with the mSv value

Not touched: Wearable Devices, the dosimeter self-scan from DAR Dosimeter Enhanced, item stats (smokes, drinks).

**Compatibility**
- Works with or without: DAR Dosimeter Enhanced, Grain RGB & Psi Color Effects Remover, G_FLAT's Msv Above Radiation Icon, G.A.M.M.A. Minimalist HUD, UI Rework G.A.M.M.A. Style.
- Replaces "Radiation_Overhaul - Silent Radiation" and "No geiger sound in my head" (both can be disabled). If Silent Radiation stays enabled, its ticks also require a charged geiger.
- Any MO2 position; file names are unique. No new game needed.

**Check**
After loading a save, the log (Anomaly\appdata\logs) shows lines starting with [zzz_rad_geiger_overhaul] saying what was patched.
