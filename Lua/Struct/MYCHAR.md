# Description

A player character.

# Members

| Type    | Name            | Description                                                                                            |
|---------|-----------------|--------------------------------------------------------------------------------------------------------|
| Integer | `cond`          | Condition (see COND constants).                                                                        |
| Integer | `flag`          | Player's collision with the stage (see FLAG constants).                                                |
| Integer | `direct`        | Direction (see DIR constants).                                                                         |
| Integer | `strafe_direct` | Direction whilst strafing (see DIR constants).                                                         |
| Boolean | `up`            | Player is facing upwards.                                                                              |
| Boolean | `down`          | Player is facing downwards.                                                                            |
| Integer | `unit`          | Player's 'mode' (see UNIT constants).                                                                  |
| Integer | `equip`         | Bitfield of player's equipped items (see EQUIP constants).                                             |
| Integer | `x`             | X coordinate (measured in world units).                                                                |
| Integer | `y`             | Y coordinate (measured in world units).                                                                |
| Integer | `tgt_x`         | X coordinate for screen to follow (measured in world units).                                           |
| Integer | `tgt_y`         | Y coordinate for screen to follow (measured in world units).                                           |
| Integer | `index_x`       | X offset applied to `x` to create `tgt_x` (measured in world units).                                   |
| Integer | `index_y`       | Y offset applied to `y` to create `tgt_y` (measured in world units).                                   |
| Integer | `xm`            | X momentum (measured in world units).                                                                  |
| Integer | `ym`            | Y momentum (measured in world units).                                                                  |
| Integer | `ani_wait`      | Animation duration. Once expired, sprite will change.                                                  |
| Integer | `ani_no`        | Animation number. Controls player sprite.                                                              |
| RANGE   | `hit`           | Hitbox dimensions.                                                                                     |
| RANGE   | `view`          | Offsets to apply when drawing the player's sprite.                                                     |
| RECT    | `rect`          | Sprite rectangle of player.                                                                            |
| RECT    | `rect_arms`     | Sprite rectangle of player's weapon.                                                                   |
| Integer | `level`         | Level of the player's weapon.                                                                          |
| Integer | `exp_wait`      | Duration of EXP bar flashing.                                                                          |
| Integer | `exp_count`     | EXP that the player has just earned. Will be shown by a value-view.                                    |
| Integer | `shock`         | Duration of player's invulnerability after being hurt.                                                 |
| Integer | `rensha`        | Delay between player's shots of an automatic weapon.                                                   |
| Integer | `bubble`        | Counter that animates the bubble barrier.                                                              |
| Integer | `life`          | Player's current health.                                                                               |
| Integer | `star`          | How many Whimsical Stars are orbiting the player.                                                      |
| Integer | `max_life`      | Player's maximum health. The limit is 232.                                                             |
| Integer | `lifeBr`        | Player's current health, delayed. Gradually ticks-down after being hit.                                |
| Integer | `lifeBr_count`  | Counter that controls how slowly `lifeBr` is decremented.                                              |
| Integer | `air`           | How long the player has until drowning.                                                                |
| Integer | `air_get`       | How long the air counter should flash for.                                                             |
| Boolean | `sprash`        | "Splash". Whether the player is underwater or not.                                                     |
| Boolean | `ques`          | "Question". Whether or not the player is facing away and examining something.                          |
| Integer | `boost_sw`      | Booster mode: 0 = inactive, 1 = active (v0.8)/right (v2.0), 2 = up, 3 = down, 4 = left.                |
| Integer | `boost_cnt`     | Booster energy remaining.                                                                              |
| Integer | `muzzle`        | Duration of the weapon muzzle flash.                                                                   |
| Integer | `dust`          | Cooldown before player can create another sand/dust caret.                                             |
| Integer | `outside_cnt`   | Countdown until off-screen player is respawned.                                                        |
| Integer | `outside_x`     | X coordinate of the off-screen player indicator (measured in world units).                             |
| Integer | `outside_y`     | Y coordinate of the off-screen player indicator (measured in world units).                             |
| Integer | `add_flash`     | Counter that animates the EXP bar's flashing.                                                          |
