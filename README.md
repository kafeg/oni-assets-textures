# oni-assets-textures

Planet, moon and sky textures for [ONI](https://github.com/kafeg/oni), consumed as a Git
submodule at `public/assets/textures/`. Stored with Git LFS.

The build pipeline converts these into GPU-compressed KTX2 (`npm run build:planet-textures`
in the main repository) — the sources here are the originals.

## Licensing

**There is no blanket license on this repository** — see [ATTRIBUTION.md](ATTRIBUTION.md)
for the per-file record. In short:

- the planet, moon and sky maps are **Solar System Scope, CC BY 4.0** (commercial use
  allowed, attribution required — it is in the game's credits panel);
- the Pluto map and the lunar height/normal maps are **derived from public-domain NASA/USGS
  mission data** by scripts in the main repository;
- the Saturn and Uranus ring strips are **generated from published ring geometry**, with no
  source imagery at all.

The last two groups are original work under the main repository's license. Everything here
is cleared for commercial use.
