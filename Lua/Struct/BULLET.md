# Description

A bullet. You know, that thing that comes out of a gun.

# Members

| Type    | Name           | Description                                                                                            |
|---------|----------------|--------------------------------------------------------------------------------------------------------|
| Integer | `flag`         | Bullet's collision with the stage (see FLAG constants).                                                |
| Integer | `code_bullet`  | Bullet ID (see BULLET constants).                                                                      |
| Integer | `bbits`        | Bullet traits (see BBITS constants).                                                                   |
| Integer | `cond`         | Condition (see COND constants).                                                                        |
| Integer | `x`            | X coordinate (measured in world units).                                                                |
| Integer | `y`            | Y coordinate (measured in world units).                                                                |
| Integer | `xm`           | X momentum (measured in world units).                                                                  |
| Integer | `ym`           | Y momentum (measured in world units).                                                                  |
| Integer | `tgt_x`        | Target X coordinate (measured in world units).                                                         |
| Integer | `tgt_y`        | Target Y coordinate (measured in world units).                                                         |
| Integer | `tgt_mc`       | ID of targeted player (0 for P1, 1 for P2).                                                            |
| Integer | `act_no`       | Action number. Controls bullet behaviour.                                                              |
| Integer | `act_wait`     | Action duration. Once expired, bullet changes behaviour.                                               |
| Integer | `ani_wait`     | Animation duration. Once expired, sprite will change.                                                  |
| Integer | `ani_no`       | Animation number. Controls bullet sprite.                                                              |
| Integer | `direct`       | Direction (see DIR constants).                                                                         |
| RECT    | `rect`         | Sprite rectangle.                                                                                      |
| Integer | `count1`       | Miscellaneous counter.                                                                                 |
| Integer | `count2`       | Miscellaneous counter.                                                                                 |
| Integer | `life_count`   | Timer until the bullet dissipates.                                                                     |
| Integer | `damage`       | Damage that the bullet inflicts.                                                                       |
| Integer | `life`         | How many things a bullet can pierce before dissipating.                                                |
| Integer | `light_offset` | Offset of the bullet's light, along the direction that the bullet is facing (measured in world units). |
| Integer | `enemyXL`      | Hitbox X radius for enemy collision (measured in world units).                                         |
| Integer | `enemyYL`      | Hitbox Y radius for enemy collision (measured in world units).                                         |
| Integer | `blockXL`      | Hitbox X radius for stage collision (measured in world units).                                         |
| Integer | `blockYL`      | Hitbox Y radius for stage collision (measured in world units).                                         |
| RANGE   | `view`         | Offsets to apply when drawing the bullet's sprite.                                                     |
