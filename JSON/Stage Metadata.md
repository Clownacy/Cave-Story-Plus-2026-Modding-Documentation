# `parts`

Type: String

Name of the tileset to be used. Affects the selection of `X.pxa`, `X.pxw`, and
`PrtX.png` files (`SURF_PARTS` - see `SURF.md`).


# `map`

Type: String

Name of the map to be used. Affects the selection of `X.pxe`, `X.pxm`, and
`X.tsc` files.


# `bkType`

Type: Integer

Numerical ID of the type of background scrolling to use.

| Value | Description                                                            |
|-------|------------------------------------------------------------------------|
| `0`   | Tiled background, unmoving.                                            |
| `1`   | Tiled background, moves with camera slowly.                            |
| `2`   | Tiled background, moves with camera.                                   |
| `3`   | No background. Full-screen water effect instead.                       |
| `4`   | No background.                                                         |
| `5`   | Tiled background, rapidly scrolls horizontally.                        |
| `6`   | Complex parallax background. Intended for `bkMoon`.                    |
| `7`   | Complex parallax background. Intended for `bkFog`.                     |
| `8`   | Complex parallax background. Intended for `bkMoon`. Scrolls backwards. |


# `back`

Type: String

Name of the background image to be used. Affects the selection of `bkX.png`
files.


# `back_water`

Type: String

Name of the background image to be used. Affects the selection of `bkX.png`
files.

This background only appears underwater, when physical water is enabled (see
`Settings.md` for more information).


# `npc`

Type: String

Name of the NPC sprite-sheet to be used. Affects the selection of `NpcX.png`
files (`SURF_NPC_ENEMY` - see `SURF.md`).


# `boss`

Type: String

Name of the Boss sprite-sheet to be used. Affects the selection of `NpcX.png`
files (`SURF_NPC_BOSS` - see `SURF.md`).


# `boss_no`

Type: Integer

Numerical ID of the boss to load in this stage.

| Value | Description  |
|-------|--------------|
| `0`   | No boss.     |
| `1`   | Omega        |
| `2`   | Balfrog      |
| `3`   | Monster X    |
| `4`   | Core         |
| `5`   | Ironhead     |
| `6`   | Twin Dragons |
| `7`   | Undead Core  |
| `8`   | Heavy Press  |
| `9`   | Ballos       |


# `lighting`

Type: String

The type of lighting to use in this stage.

| Value        | Description                                                |
|--------------|------------------------------------------------------------|
| `"disabled"` | No lighting; full-bright.                                  |
| `"normal"`   | Indoor lighting; floors, walls, and background can be lit. |
| `"outside"`  | Outdoor lighting; floors and walls can be lit.             |


# `name`

Type: String

The name of the stage. Will be shown in the minimap as well as briefly
on-screen when entering the stage.
