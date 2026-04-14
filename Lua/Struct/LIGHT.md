# Description

A light which is emitted by an NPC, player, or other entity.

If `directional` is `true`, the light will point in the direction specified by
the parent entity's `direct` member variable. Otherwise, it will point it all
directions.

If `player` is `true`, then the light will use hardcoded settings that are
specific to the player's light source:
- Emits two light sources.
  - Radius 24, directionless, white with alpha of 102.
  - Radius 8, directionless, white with alpha of 127.

# Members

| Type    | Name          | Description                                 |
|---------|---------------|---------------------------------------------|
| COLOR   | `color`       | Light's colour.                             |
| Integer | `radius`      | Light's radius.                             |
| Boolean | `directional` | Light should inherit direction from parent. |
| Boolean | `player`      | Override with special player settings.      |
