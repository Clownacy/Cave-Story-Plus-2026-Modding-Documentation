# `face_flipping_enabled`

Selects whether dialogue box portraits should be horizontally flipped in
accordance with TSC scripting.

| Value          | Description                       |
|----------------|-----------------------------------|
| `true`         | Portraits can face left or right. |
| `false`        | Portraits can only face left.     |


# `lighting_enabled`

Enables the lighting system which was introduced in the Switch version of
Cave Story+.

| Value          | Description       |
|----------------|-------------------|
| `true`         | Enable lighting.  |
| `false`        | Disable lighting. |


# `physical_water_enabled`

Enables the phyiscal water system which was introduced in the Switch version of
Cave Story+.

| Value          | Description             |
|----------------|-------------------------|
| `true`         | Enable physical water.  |
| `false`        | Disable physical water. |


# `pixel_alignment_shift`

Aliases the positioning of sprites, so that lower-resolution sprites always
have their pixels correctly aligned to a grid.

| Value          | Description                                      |
|----------------|--------------------------------------------------|
| `0`            | 1x1 alignment. Ideal for 4x resolution graphics. |
| `1`            | 2x2 alignment. Ideal for 2x resolution graphics. |
| `2`            | 4x4 alignment. Ideal for 1x resolution graphics. |


# `player_character`

Chooses the character which the player will appear as.

| Value            | Description        |
|------------------|--------------------|
| `"default"`      | Quote.             |
| `"quote"`        | Quote.             |
| `"curly"`        | Curly Brace.       |
| `"king"`         | King.              |
| `"sue"`          | Sue Sakamoto.      |
| `"booster"`      | Professor Booster. |
| `"toroko"`       | Toroko.            |
| `"killer robot"` | Killer Robot.      |
| `"curly clone"`  | Curly Brace Clone. |
