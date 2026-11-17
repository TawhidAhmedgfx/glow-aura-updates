# Glow Aura · update channel

This repository delivers updates for the **Glow Aura** Photoshop plugin by Tawhid Ahmed.

- `version.json` holds the latest version, its download link and short release notes (English + Bangla).
- Every version's installer is kept in the `releases/` folder (`GlowAura-X.Y.Z.ccx`).
- `guide/Glow-Aura-Guide-Bangla.pdf` is the latest user guide (Bangla): first install, updates and every button.
- From 2.8.0, `live/bundle-X.Y.Z.json` holds the live update that applies inside Photoshop (checked against the sha256 in `version.json`).

Glow Aura checks `version.json` when the panel opens. When a newer version is out, it shows **Update available** with an **Update now** button that downloads that `.ccx` and opens the installer.

To publish an update: add `releases/GlowAura-X.Y.Z.ccx`, then set `version` and `url` in `version.json` to that file.
