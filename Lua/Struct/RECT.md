# Description

Rectangle, often used to specify a sprite within a sprite-sheet.

The bounds are measured in pixels at the "Classic" resolution, so sprite sheets
which use high resolutions must be accounted for by dividing their pixel
coordinates by the resolution multiplier.

# Members

| Type    | Name     | Description                           |
|---------|----------|---------------------------------------|
| Integer | `left`   | Rectangle's left bound (inclusive).   |
| Integer | `top`    | Rectangle's top bound (inclusive).    |
| Integer | `right`  | Rectangle's right bound (exclusive).  |
| Integer | `bottom` | Rectangle's bottom bound (exclusive). |
