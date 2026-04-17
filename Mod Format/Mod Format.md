Mods could be installed directly to the game's files, but the intended way is
to install them in your 'Documents' folder, like this:

- Videos
- Pictures
- Downloads
- Documents
  - My Games
    - Cave Story+
      - Mods
        - Forever Halloween
        - Example Mod 1
        - Example Mod 2
        - Example Mod 3
        - mods.txt

'mods.txt' lists each mod that is to be enabled. It looks like this:

```
+ C:/Users/USERNAMEGOESHERE/Documents/My Games/Cave Story+/mods/Forever Halloween
+ C:/Users/USERNAMEGOESHERE/Documents/My Games/Cave Story+/mods/Example Mod 1
+ C:/Users/USERNAMEGOESHERE/Documents/My Games/Cave Story+/mods/Example Mod 2
+ C:/Users/USERNAMEGOESHERE/Documents/My Games/Cave Story+/mods/Example Mod 3
```

Each line is an absolute path to a mod's folder. The '+' at the start means
that this mod is enabled. Changing it to '-' will disable the mod. Ensure that
'USERNAMEGOESHERE' is replaced with your Windows username!

(Note: I am aware that relative file paths would be better here.)

Modded files go inside a mod's folder, and will override files in the game. In
the Halloween Forever mod, the Halloween season's 'Metadata.json' file is
overridden to make the season last for the full year. Many other files can be
overridden, such as images, level data, and Lua code.
