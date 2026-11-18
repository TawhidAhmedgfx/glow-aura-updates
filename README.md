# Aura Studio · update channel

This repository delivers updates for **Aura Studio** (formerly Glow Aura), a Photoshop plugin by Tawhid Ahmed with four tools: Glow Aura, Social Sizes, Background Remover (Auto Cut + Shadow Cut) and Glass.

- `version.json` holds the latest version, its download link and short release notes (English + Bangla).
- Every version's installer is kept in the `releases/` folder (`GlowAura-X.Y.Z.ccx`).
- `guide/Aura-Studio-Guide-Bangla.pdf` is the latest user guide (Bangla): first install, updates and every tool.
- From 2.8.0, `live/bundle-X.Y.Z.json` holds the live update that applies inside Photoshop (checked against the sha256 in `version.json`). From 3.6.0, the code inside the bundle (and the `.ccx`) ships obfuscated.

Aura Studio checks `version.json` when the panel opens. When a newer version is out, it shows **Update available** with an **Update now** button that downloads that `.ccx` and opens the installer.

To publish an update: add `releases/GlowAura-X.Y.Z.ccx`, then set `version` and `url` in `version.json` to that file.
