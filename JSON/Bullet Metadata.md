# `__group_comment`

Type: String

A comment extracted from the game's source code which describes the associated
group of bullets.


# `is_special`

Type: Boolean

If `true`, then the function `IsActiveSomeBullet` will return `true` if one of
these bullets is currently active. Used by Ma Pignon to block certain bullets.


# `damage`

Type: Integer

How much damage to inflict upon a target.


# `life`

Type: Integer

How many NPCs/bosses a bullet can hit before dissipating.


# `life_count`

Type: Integer

How many frames a bullet should last before dissipating.


# `light_offset`

Type: Integer

Positional offset applied to the light sprite. Is projected along the direction
specified by the bullet's 'direct' variable.


# `bbits`

Type: BBITS (See `BBITS.md` for more information.)

A series of booleans describing the bullet.


# `enemyXL`

Type: Integer

Width of the enemy hitbox.


# `enemyYL`

Type: Integer

Height of the enemy hitbox.


# `blockXL`

Type: Integer

Width of the level hitbox.


# `blockYL`

Type: Integer

Height of the level hitbox.


# `view`

Type: RANGE (See `RANGE.md` for more information.)

Dimensions related to the bullet's sprite. Used to centre the sprite over its
position coordinate.
