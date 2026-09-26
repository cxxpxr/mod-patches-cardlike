# Cardlike mod patches

Patches that turn existing mods into mods for Cardlike.

A patch (`.clpatch`) holds only the files written for the Cardlike version of a mod: its Lua code and its manifest. It does not contain the original mod. When you install a patch, Cardlike takes every other file (pictures, sounds) from the original mod archive that you download yourself, and checks each one by its SHA-256.

## Patches

| Patch | Makes | Needs this original archive | Get it from |
|---|---|---|---|
| [`patches/pokermon.clpatch`](patches/pokermon.clpatch) | Pokermon for Cardlike | Pokermon 3.9.1 (`Pokermon-3.9.1.zip`) | [Pokermon 3.9.1 source archive](https://github.com/InertSteak/Pokermon/archive/refs/tags/3.9.1.zip) ([repository](https://github.com/InertSteak/Pokermon)) |

## Install

1. Download the patch and the original archive named in the table. Use the archive as downloaded: do not unpack or change it.
2. In Cardlike, press **Mods** on the main menu.
3. Drop the `.clpatch` file and the original `.zip` onto the Mods window together (or one after the other).
4. Reload the page.

If the archive is a different version, Cardlike lists the files that are missing or different and does not install the mod.

## What is in a patch

A patch is plain text, so you can read it before you install it:

- `== copy` blocks name a file of the original archive by its SHA-256. Cardlike copies it as it is.
- `== source` and `== picture` blocks build a picture from rectangles of original pictures (for example a sprite sheet with the frames packed together).
- `== file` blocks are the Cardlike mod's own files, written out in full.

The Cardlike modding documentation (Mods window, "Mod patches") describes the format in full.

## Disclaimer

- These patches are unofficial fan work. They are not made, reviewed, endorsed or supported by the authors of the original mods, by the developers or publishers of the games those mods were made for, or by the Cardlike team.
- Pokermon is a mod for Balatro. This project is not affiliated with LocalThunk or Playstack, or with Nintendo, Game Freak, Creatures Inc. or The Pokémon Company. All names and trademarks belong to their owners.
- The patches contain no art, sounds or other files of the original mods. You get those from the original authors.
- A Cardlike port works like the original where Cardlike allows it. Some cards work differently or are missing because Cardlike has no matching feature. Problems with a port belong in this repository's issues, not with the original mod's authors.
- The patches are provided as is, without any warranty. See the license.

## Credits

- **Pokermon** by InertSteak and the Pokermon contributors: <https://github.com/InertSteak/Pokermon>. The Cardlike version keeps the original's credits. Please support the original mod.

## License

This repository is licensed under the [GNU General Public License v3.0](LICENSE).

The patches contain code and text adapted from the original mods. Pokermon is licensed under the GNU General Public License v3.0, and the Pokermon patch is shared under the same license. The original mods' art and sounds are not part of this repository and keep their own licenses.
