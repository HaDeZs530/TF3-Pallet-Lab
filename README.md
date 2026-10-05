# TF3 Palette Lab

Design your own Transport Fever 3 UI colors on real in-game screenshots, then download them as a ready-to-use mod.

**Open the Lab:** https://hadezs530.github.io/TF3-Pallet-Lab/

## Making a theme
1. Start from a preset (Stock, Cobalt, Teal, Mauve Dusk) or move the sliders.
2. Click anything in the screenshot to see which of the 12 palette shades paints it, and pin it to its own color if you want.
3. Hold **Hold to see stock** (or press Space) to compare with the default UI.

## Turning it into a mod
1. In **Make it a mod**, type a theme name and your name.
2. Pick the screenshot tab you want as the mod's logo.
3. Click **Download mod (.zip)**.

## Installing the mod
1. Close Transport Fever 3.
2. Unzip the download. You get one folder named after the mod ID (for example `railbaron42_ui_midnight_teal_1`).
3. Open your TF3 user folder. On Steam it is:
   `C:\Program Files (x86)\Steam\userdata\<number>\3493540\local\`
   `<number>` is your Steam account ID. If there are several, use the one with a `3493540` folder inside. If Steam is installed somewhere else, use that Steam folder. The drive the game is installed on doesn't matter.
4. Copy the whole mod folder into `local\mods\` (create `mods` if it isn't there). You should have `local\mods\<mod ID>\mod.json`, not `local\mods\<mod ID>\<mod ID>\mod.json`.
5. Start the game and turn the mod on in the mod list.
6. Turn off any other UI color mod (Dark UI, other Palette Lab themes). They all change the same 12 colors.

**Change a color later:** edit the hex values in `content\gui\main\recolor.script.tl` with Notepad, then restart the game.

**Remove it:** turn it off in the mod list, or delete its folder from `local\mods\`.

## Publishing on mod.io (optional)
1. Put the mod folder in `local\staging_area\` instead of `local\mods\`. Don't keep a copy with the same mod ID in both.
2. Restart the game, open **Mod Manager → My Mods**, select the mod and upload. The logo (`_metadata\0.png`) and the name and description (`_metadata\modinfo.json`) are already filled in.
3. After uploading, the game writes `_metadata\mod.io_fileid.txt`. Keep it. To update later, raise `revision` in `mod.json`, restart, and only upload if the dialog says "The existing mod on mod.io will be updated."

Every downloaded zip also includes these steps as `INSTALL.txt`.
