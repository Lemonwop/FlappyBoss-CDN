# FlappyBoss-CDN

All of Flappy Boss's art, fonts and models. The game loads them from here through jsDelivr:

    https://cdn.jsdelivr.net/gh/Lemonwop/FlappyBoss-CDN@<commit>/<path>

(`<commit>` is pinned in the game's `src/shared/cdn.ts`, so a change here only shows up in the game once that is
updated. Pinned addresses never go stale in anyone's cache.) The game keeps its own copy in `public/` as a backup and
falls back to it if this is unreachable.

## What's where

| Folder | What |
| --- | --- |
| `badges/ birds/ buildings/ dishes/ forces/ fx/ items/ mobs/ npc/ props/ ships/ ui/` | Art the game draws |
| `fonts/` | The game's comic font |
| `models/` | The Bird Box 3D model |
| top level `*.png`, `*.jpg`, `*.webp` | Logos, frames and backgrounds |
| `island.png`, `islands/` | Island art. The game loads these from its own server, not from here: each one has to match the walking map files (`*.bin`) beside it, which stay with the code |
| `source/` | The original artwork the art was made from (not loaded by the game). The vector files the island maps are traced from are not kept here |

There are no sound files yet.

## v1 (the original Flappy Boss)

Everything from the first game, kept in `v1/`:

| Folder | What |
| --- | --- |
| `v1/assets/` | The original art, sorted by world, plus its fonts |
| `v1/music/` | All of its music and sound |
| `v1/birds/` `v1/eggs/` `v1/cosmetics/` | Every bird, egg and cosmetic picture from the game's database, named after the item |
| `v1/shop/` `v1/membership/` | The shop's and the membership bonuses' pictures |
| `v1/index.json` | Which file is which item |
