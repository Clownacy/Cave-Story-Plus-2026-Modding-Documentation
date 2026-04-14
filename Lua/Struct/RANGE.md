# Description

Rectangle, often used to specify an NPC's hitbox.

Sometimes the game forcefully uses `back` instead of `front`, making `back`
both the left and right radii. For example, NPCs do this when checking for
collision with bullets.

Measured in world units.

# Members

| Type    | Name     | Description                |
|---------|----------|----------------------------|
| Integer | `front`  | Rectangle's right radius.  |
| Integer | `top`    | Rectangle's top radius.    |
| Integer | `back`   | Rectangle's left radius.   |
| Integer | `bottom` | Rectangle's bottom radius. |
