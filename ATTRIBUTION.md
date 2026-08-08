# Attribution & licensing

Planet, moon and sky textures for [ONI](https://github.com/kafeg/oni). Files were renamed
when they were brought in, which is why the names here do not match the upstream ones.

Two groups, with different terms. **There is no blanket license on this repository** —
check the group a file belongs to.

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

## Derived from public-domain mission data — ONI original work

Built by scripts in the main repository from NASA/USGS products. NASA and USGS planetary
data are not subject to copyright. The derived files are original work of the ONI
maintainer under the [repository license](https://github.com/kafeg/oni/blob/master/LICENSE)
(PolyForm Noncommercial 1.0.0), and each is reproducible from its script.

| File | Built by | Source data |
|---|---|---|
| `plutomap1k.jpg` | `scripts/generate-pluto-texture.mjs` | [Pluto New Horizons Global Mosaic 300m (Jul 2017)](https://astrogeology.usgs.gov/search/map/pluto_newhorizons_global_mosaic_300m_jul2017) — USGS Astrogeology / NASA / JHUAPL / SwRI |
| `moon_bump_2k.jpg` | inline conversion, see below | [LRO LOLA gridded DEM, 16 pixels/degree](https://pds-geosciences.wustl.edu/lro/lro-l-lola-3-rdr-v1/lrolol_1xxx/data/lola_gdr/cylindrical/) — NASA/GSFC LOLA team |
| `moon_normal_2k.png` | `scripts/generate-normal-map.mjs` | derived from `moon_bump_2k.jpg` |

The lunar height map is the LOLA `ldem_16.img` raster (5760×2880, 16-bit signed, height =
DN × 0.5 m) rolled half a width — LOLA is centred on 180° longitude, every other map here
is centred on 0° — then normalised and downsampled to 2048×1024. Verified by correlating
the elevation against the `moon_8k.jpg` albedo: the maria are both dark and low, and the
correlation is +0.64 with the roll versus −0.42 without.

## Generated from published geometry — ONI original work

No source imagery at all: these are one-dimensional strips (colour and opacity against
orbital radius) computed from ring radii and optical depths in the literature. Original
work under the repository license.

| File | Built by | Structure |
|---|---|---|
| `saturnrings.png` | `scripts/generate-ring-textures.mjs` | C, B and A rings, the Cassini Division, and the Colombo/Maxwell/Huygens/Encke/Keeler gaps |
| `uranus_ring.png` | `scripts/generate-ring-textures.mjs` | rings 6, 5, 4, α, β, η, γ, δ, λ, ε plus the faint ζ sheet |

## Adding a texture here

Record the source, author and license in this file in the same commit. If the license is
unknown, do not add the file.
