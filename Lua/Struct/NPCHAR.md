# Description

A non-playable character or entity.

# Members

| Type          | Name            | Description                                                                                            |
|---------------|-----------------|--------------------------------------------------------------------------------------------------------|
| Integer       | `cond`          | Condition (see COND constants).                                                                        |
| Integer       | `flag`          | NPC's collision with the stage (see FLAG constants).                                                   |
| Integer       | `x`             | X coordinate (measured in world units).                                                                |
| Integer       | `y`             | Y coordinate (measured in world units).                                                                |
| Integer       | `xm`            | X momentum (measured in world units).                                                                  |
| Integer       | `ym`            | Y momentum (measured in world units).                                                                  |
| Integer       | `xm2`           | Secondary X momentum (measured in world units).                                                        |
| Integer       | `ym2`           | Secondary Y momentum (measured in world units).                                                        |
| Integer       | `tgt_x`         | X coordinate for screen to follow (measured in world units).                                           |
| Integer       | `tgt_y`         | Y coordinate for screen to follow (measured in world units).                                           |
| Integer       | `code_char`     | NPC ID. There are no constants for these: they are always plain numbers.                               |
| Integer       | `code_flag`     | Which flag is associated with the NPC (see BITS_FLAG_ALIVE and other BITS constants).                  |
| Integer       | `code_event`    | Which event is associated with the NPC (see BITS_EVENT_HIT and other BITS constants).                  |
| Integer       | `surf`          | Which sprite-sheet the NPC should use (see SURF constants).                                            |
| Integer       | `hit_voice`     | Which sound the NPC should use when hit (see WAVE constants).                                          |
| Integer       | `destroy_voice` | Which sound the NPC should use when destroyed (see WAVE constants).                                    |
| Integer       | `life`          | NPC's current health.                                                                                  |
| Integer       | `exp`           | How much EXP the NPC should drop when destroyed.                                                       |
| Integer       | `size`          | NPC's size (see NPCSIZE constants).                                                                    |
| Integer       | `direct`        | Direction (see DIR constants).                                                                         |
| Integer       | `bits`          | NPC attributes (see BITS constants). Affects all players.                                              |
| Integer Array | `bits_mc`       | NPC attributes (see BITS constants). Affects only a specific player (index 1 affects player 1, etc.).  |
| RECT          | `rect`          | Sprite rectangle of NPC.                                                                               |
| Integer       | `ani_wait`      | Animation duration. Once expired, sprite will change.                                                  |
| Integer       | `ani_no`        | Animation number. Controls NPC sprite.                                                                 |
| Integer       | `count1`        | Miscellaneous counter.                                                                                 |
| Integer       | `count2`        | Miscellaneous counter.                                                                                 |
| Integer       | `act_no`        | Action number. Controls NPC behaviour.                                                                 |
| Integer       | `act_wait`      | Action duration. Once expired, NPC changes behaviour.                                                  |
| RANGE         | `hit`           | Hitbox dimensions.                                                                                     |
| RANGE         | `view`          | Offsets to apply when drawing the NPC's sprite.                                                        |
| LIGHT         | `light`         | Light that the NPC emits.                                                                              |
| Integer       | `tgt_mc`        | ID of targeted player (0 for P1, 1 for P2).                                                            |
| Integer       | `shock`         | Duration that NPC is stunned after being hurt.                                                         |
| Integer       | `damage_view`   | Amount of damage received by the NPC. Shown by a value-view.                                           |
| Integer       | `damage`        | Amount of damage given by the NPC. Affects all players.                                                |
| Integer Array | `damage_mc`     | Amount of damage given by the NPC. Affects only a specific player (index 1 affects player 1, etc.).    |
| NPCHAR        | `pNpc`          | Parent NPC. Useful for destroying the NPC when another NPC is destroyed.                               |
