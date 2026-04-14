# `save_slot_identifier`

Type: String

Unique identifier used to distinguish save data. If left empty, the expansion
will be assumed to not use save data.


# `full_name`

Type: String

The name of the expansion. Will appear in the main menu.


# `description`

Type: String

The tag-line of the expansion. Will appear when selecting the expansion.


# `difficulties`

Type: Boolean

Whether the expansion should support difficulty levels or not. If not, then the
expansion will default to Normal difficulty.


# `requirement`

Type: String

The condition under which the expansion is unlocked.

| Value           | Description                               |
|-----------------|-------------------------------------------|
| `"none"`        | The expansion is always unlocked.         |
| `"item"`        | The player has obtained a certain item.   |
| `"arm"`         | The player has obtained a certain weapon. |
| `"best ending"` | The best ending has been achieved.        |


# `requirement_number`

Type: Integer

If `requirement` is set to `"item"`, then this is the numerical ID of the item
which is required.

If `requirement` is set to `"arm"`, then this is the numerical ID of the weapon
which is required.
