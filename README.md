<div align="center">

# SkinHub

### Every CS2 skin. In your browser. Rendered for real.

**[skinhub.gg](https://skinhub.gg)** — a free, community-built 3D skin viewer for Counter-Strike 2.

</div>

---

## What is SkinHub?

SkinHub lets you inspect any CS2 weapon or knife finish in full 3D, straight from your browser — no game launch, no downloads, no queue for an inspect server.

Unlike screenshot galleries or flat texture previews, SkinHub **re-implements CS2's own weapon-finish shader**. Every skin is composited in real time on your GPU exactly the way the game does it: the same paint styles, the same wear erosion, the same seeded pattern placement. What you see on SkinHub is what you get in-game.

## Features

- 🔫 **2,100+ weapon and knife finishes** — every rifle, pistol, SMG, heavy weapon, and knife in the game
- 🎨 **All 9 official paint styles** — Solid Color, Hydrographic, Spray-Paint, Anodized, Anodized Multicolored, Anodized Airbrushed, Custom Paint Job, Patina, and Gunsmith, each transcribed from the game's shader
- 📉 **True float rendering** — drag the wear slider from Factory New to Battle-Scarred and watch the paint erode using the game's actual wear, grunge, and durability masks — not a brightness filter
- 🎲 **Real pattern seeds** — pattern placement is driven by a faithful port of the game's own random-number generator, so seed `661` on SkinHub is seed `661` in-game
- 🏷️ **Stickers** — place, drag, and rotate stickers in all five positions, projected onto the actual weapon geometry
- 🧿 **Charms** — attach and position keychains on your weapon
- 🖱️ **Full 3D inspection** — rotate, zoom, and examine every angle in high quality, with game-matched lighting

## Why it looks right

Most skin sites approximate. SkinHub's renderer is a line-by-line transcription of the Source 2 weapon-finish shader, and every finish in the catalogue is verified against reference captures with an automated pixel-level test harness. When a skin has a pearlescent coat, a color-zone durability quirk, or a legacy CS:GO texture layout — it renders that way, because the game's rules are the renderer's rules.

## Roadmap

- 🧤 Gloves
- 🔢 StatTrak™ counters and name tags rendered on the model
- 🧿 Fully modeled 3D charms
- 📸 High-resolution screenshot export & shareable skin links
- 🔍 Inspect-link support — paste any `steam://` inspect link
- 🎲 Seed explorer for pattern-dependent skins (Case Hardened, Fade, Doppler, …)
- 👤 Sign in with Steam & showcase your own inventory *(exploring)*

## Open tooling

We keep the tooling that powers SkinHub open for the community:

| Repository | What it does |
|---|---|
| [`asset-export`](https://github.com/SkinHubgg/asset-export) | Pipeline for extracting weapon models, paint-kit recipes, and pattern textures from your own CS2 installation |
| [`npm-package`](https://github.com/SkinHubgg/npm-package) | Typed client for pulling skins, materials, and shader parameters from a defined URL |

Issues, bug reports (that skin that looks *slightly* off — we want to know), and ideas are welcome on the relevant repository.

## Contact

📧 [contact@skinhub.gg](mailto:contact@skinhub.gg)

---

<sub>SkinHub is a community project. It is not affiliated with, endorsed by, or sponsored by Valve Corporation. Counter-Strike, CS2, and all associated weapon finishes are the property of Valve Corporation. Asset extraction requires your own copy of the game.</sub>
