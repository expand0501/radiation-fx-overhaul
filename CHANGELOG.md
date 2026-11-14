# Changelog - Radiation FX Overhaul by Expand

Earlier builds were named RadiationGeigerOverhaul_GAMMA (1.3.1, 1.3.2, 1.3.3, 1.4.0).

- 1.5.0: first build under the name Radiation FX Overhaul by Expand.
- 1.7.0: (details not recorded)
- 2.0.0: state documented in the readme (geiger sound sources, DAR integration, HUD icon modes, tooltip modes, film grain option).
- 2.1.0: robustness fixes - 2D sound flag fallback, environment radiation read falls back to the engine value when arszi's value is not a number, MCM options re-applied 0.2 s after a change (stale MCM cache, e.g. DOGMA), HUD update wrapped in pcall, DAR mode from a previously loaded save no longer carried over.
- 2.1.1: robustness - wrapped HUD/tooltip/status-icon functions now return the original results; geiger tick skipped when there is no actor.
- 2.1.2: fix - the clicks a radiation field plays itself (engine HUD zone list) were not gated: they played in DAR player contamination mode, with "Play for external radiation" off and with "Only with geiger in detector slot". They now follow the same rules as the other environment clicks (wraps _G.CZone_Touch, like Nitpickers GeigerHush).
