Tile attribute. Can be obtained with `GetAttributeRaw`.

# `ATRB_SAND_MASK`

Bitmask which can be used to extract a tile attribute's 'sand' property. When
a tile has this property enabled, the player will create `CARET_SANDDUST`
carets when walking on it.

# Other

| Name                      | Type       | Water | Blocks                    | Notes                           |
|---------------------------|------------|-------|---------------------------|---------------------------------|
| `ATRB_DISABLE`            | Misc       | No    | Nothing                   |                                 |
| `ATRB_BACK`               | Background | No    | Nothing                   |                                 |
| `ATRB_BACK_W`             | Background | Yes   | Nothing                   |                                 |
| `ATRB_BACK_EB`            | Background | No    | NPC                       |                                 |
| `ATRB_BACK_EB_W`          | Background | Yes   | NPC                       |                                 |
| `ATRB_BACK_BULTH`         | Background | No    | Player, NPC, Boss         |                                 |
| `ATRB_FRONT`              | Foreground | No    | Nothing                   |                                 |
| `ATRB_BLOCK`              | Foreground | No    | Player, NPC, Boss, Bullet |                                 |
| `ATRB_DAMAGE`             | Foreground | No    | Nothing                   | Hurts player.                   |
| `ATRB_SNACK`              | Foreground | No    | Player, NPC, Boss, Bullet | Destroyed when shot.            |
| `ATRB_EBLOCK`             | Foreground | No    | NPC, Boss, Bullet         | Ignored by `BITS_THROW_EBLOCK`. |
| `ATRB_BLIND`              | Foreground | No    | Nothing                   | Not drawn on mini-map.          |
| `ATRB_BLOCKME`            | Foreground | No    | Player                    |                                 |
| `ATRB_FRONT_BEHIND_WATER` | Foreground | No    | Player                    | Drawn behind physical water.    |
| `ATRB_TRI_A`              | Triangle   | No    | Player, NPC, Boss, Bullet |                                 |
| `ATRB_TRI_B`              | Triangle   | No    | Player, NPC, Boss, Bullet |                                 |
| `ATRB_TRI_C`              | Triangle   | No    | Player, NPC, Boss, Bullet |                                 |
| `ATRB_TRI_D`              | Triangle   | No    | Player, NPC, Boss, Bullet |                                 |
| `ATRB_TRI_E`              | Triangle   | No    | Player, NPC, Boss, Bullet |                                 |
| `ATRB_TRI_F`              | Triangle   | No    | Player, NPC, Boss, Bullet |                                 |
| `ATRB_TRI_G`              | Triangle   | No    | Player, NPC, Boss, Bullet |                                 |
| `ATRB_TRI_H`              | Triangle   | No    | Player, NPC, Boss, Bullet |                                 |
| `ATRB_FRONT_W`            | Foreground | Yes   | Nothing                   |                                 |
| `ATRB_BLOCK_W`            | Foreground | Yes   | Player, NPC, Boss, Bullet |                                 |
| `ATRB_DAMAGE_W`           | Foreground | Yes   | Nothing                   | Hurts player.                   |
| `ATRB_SNACK_W`            | Foreground | Yes   | Player, NPC, Boss, Bullet | Destroyed when shot.            |
| `ATRB_EBLOCK_W`           | Foreground | Yes   | NPC, Boss, Bullet         | Ignored by `BITS_THROW_EBLOCK`. |
| `ATRB_BLIND_W`            | Foreground | Yes   | Nothing                   | Not drawn on mini-map.          |
| `ATRB_TRI_A_W`            | Triangle   | Yes   | Player, NPC, Boss, Bullet |                                 |
| `ATRB_TRI_B_W`            | Triangle   | Yes   | Player, NPC, Boss, Bullet |                                 |
| `ATRB_TRI_C_W`            | Triangle   | Yes   | Player, NPC, Boss, Bullet |                                 |
| `ATRB_TRI_D_W`            | Triangle   | Yes   | Player, NPC, Boss, Bullet |                                 |
| `ATRB_TRI_E_W`            | Triangle   | Yes   | Player, NPC, Boss, Bullet |                                 |
| `ATRB_TRI_F_W`            | Triangle   | Yes   | Player, NPC, Boss, Bullet |                                 |
| `ATRB_TRI_G_W`            | Triangle   | Yes   | Player, NPC, Boss, Bullet |                                 |
| `ATRB_TRI_H_W`            | Triangle   | Yes   | Player, NPC, Boss, Bullet |                                 |
| `ATRB_LEFT`               | Movement   | No    | Nothing                   | Moves player left.              |
| `ATRB_UP`                 | Movement   | No    | Nothing                   | Moves player up.                |
| `ATRB_RIGHT`              | Movement   | No    | Nothing                   | Moves player right.             |
| `ATRB_DOWN`               | Movement   | No    | Nothing                   | Moves player down.              |
| `ATRB_LEFT_W`             | Movement   | Yes   | Nothing                   | Moves player left.              |
| `ATRB_UP_W`               | Movement   | Yes   | Nothing                   | Moves player up.                |
| `ATRB_RIGHT_W`            | Movement   | Yes   | Nothing                   | Moves player right.             |
| `ATRB_DOWN_W`             | Movement   | Yes   | Nothing                   | Moves player down.              |
