# Description

'カレット' ('ka-ret-to'), whatever that means.

These are similar to particle effects, in that they are decorative entities
which do not interact with anything.

# Members

| Type    | Name           | Description                                                                  |
|---------|----------------|------------------------------------------------------------------------------|
| Integer | `cond`         | Condition (see COND constants).                                              |
| Integer | `code`         | Caret ID (see CARET constants).                                              |
| Integer | `direct`       | Direction (see DIR constants).                                               |
| Integer | `x`            | X coordinate (measured in world units).                                      |
| Integer | `y`            | Y coordinate (measured in world units).                                      |
| Integer | `xm`           | X momentum (measured in world units).                                        |
| Integer | `ym`           | Y momentum (measured in world units).                                        |
| Integer | `act_no`       | Action number. Controls caret behaviour.                                     |
| Integer | `act_wait`     | Action duration. Once expired, caret changes behaviour.                      |
| Integer | `ani_no`       | Animation number. Controls caret sprite.                                     |
| Integer | `ani_wait`     | Animation duration. Once expired, sprite will change.                        |
| Integer | `view_left`    | X offset to apply when drawing the caret's sprite (measured in world units). |
| Integer | `view_top`     | Y offset to apply when drawing the caret's sprite (measured in world units). |
| Boolean | `glow`         | Whether the caret should display a glow overlay from `Caret2.X.png`.         |
| LIGHT   | `light`        | Light that the caret emits.                                                  |
| RECT    | `rect`         | Sprite rectangle.                                                            |
