# Attribution & licensing

This repository holds planet, moon and sky textures used by
[ONI](https://github.com/kafeg/oni). **None of it is original work of the ONI maintainer**,
so it is *not* covered by the ONI license. Each file keeps the terms of its source.

Files were renamed when they were brought in, which is why the names here do not match the
upstream names.

## Solar System Scope — CC BY 4.0

Source: <https://www.solarsystemscope.com/textures/>
License: [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) —
use, adaptation and redistribution allowed, **including commercially**, provided the source
is credited.

| File | Upstream |
|---|---|
| `earth_daymap_8k.jpg` | 8k Earth daymap |
| `earth_nightmap_8k.jpg` | 8k Earth nightmap |
| `earth_clouds_8k.jpg` | 8k Earth clouds |
| `earth_normal_8k.jpg` | 8k Earth normal map |
| `earth_specular_2k.jpg` | 2k Earth specular map |
| `mercury_8k.jpg` | 8k Mercury |
| `venus_8k.jpg` | 8k Venus surface |
| `moon_8k.jpg` | 8k Moon |
| `mars_8k.jpg` | 8k Mars |
| `jupiter_8k.jpg` | 8k Jupiter |
| `saturn_8k.jpg` | 8k Saturn |
| `uranus_2k.jpg` | 2k Uranus |
| `neptune_2k.jpg` | 2k Neptune |
| `sun_8k.jpg` | 8k Sun |
| `skybox_stars.jpg` | 2k Stars |
| `skybox_milky_way.jpg` | 2k Stars + Milky Way |

Required credit, reproduced in the ONI in-game credits panel:

> Planet, moon and sky textures © [Solar System Scope](https://www.solarsystemscope.com/textures/),
> licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

## ⚠️ Unverified — most likely JHT's Planetary Pixel Emporium

| File | Notes |
|---|---|
| `plutomap1k.jpg` | Filename and 1024×512 size match the upstream Pluto map exactly |
| `uranus_ring.jpg` | 1024×72 — matches the upstream Uranus ring strip |
| `saturnrings.png` | 1024×64 — matches the upstream Saturn ring strip |
| `moon_bump_2k.jpg` | Not part of the Solar System Scope set; a lunar bump map of this kind is |
| `moon_normal_2k.png` | Derived from `moon_bump_2k.jpg` by ONI's `scripts/generate-normal-map.mjs` — inherits whatever terms that file carries |

These appear to originate from JHT's Planetary Pixel Emporium,
© James Hastings-Trew (planetpixelemporium.com). **The terms could not be verified** — the
site did not resolve at the time of writing, so no license text could be retrieved and no
permission has been obtained.

**Status: blocked for commercial use.** Before ONI ships commercially these files must
either be cleared with the author or replaced. Public-domain replacements exist for all of
them — NASA/JHUAPL/SwRI New Horizons global maps for Pluto, NASA/USGS LRO data for the
lunar bump map, and the ring strips are simple 1D gradients that can be regenerated from
published ring photometry.

## Adding a texture here

Record the source, author and license in this file in the same commit. If the license is
unknown, do not add the file.
