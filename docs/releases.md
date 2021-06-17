# ModCS Releases

Old releases will not be supported.

## ModCS 0.1.1.2

### Changelog

- Fix an issue where [ModCS.Rect.Put2Surface()](/api/drawing/rect/#modcsrectput2surface) would fail drawing if there were parts of the [Rect](/api/drawing/rect/) being drawn off the target [Surface](/api/drawing/surface/).

### Updating

To update from ModCS 0.1.1.1:

- Replace your ModCS executable with a ModCS 0.1.1.2 one.

### Download

[:material-download: Download ModCS 0.1.1.2](/assets/releases/modcs0112.zip)

## ModCS 0.1.1.1

### Changelog

- Allow [overwriting vanilla TextScript commands](/api/tsc/#custom-commands).
- Errors are now logged to the debug console.
- Fix an issue involving [ModCS.Stage.Transfer()](/api/stage/#modcsstagetransfer) not skipping TSC characters if used in a TSC command.
- Fix a vanilla Cave Story bug where the inventory screen would have weird behavior if the player has items but no weapons.

### Updating

To update from ModCS 0.1.1.0:

- Replace your ModCS executable with a ModCS 0.1.1.1 one.

### Download

[:material-download: Download ModCS 0.1.1.1](/assets/releases/modcs0111.zip)

## ModCS 0.1.1.0

### Changelog

- Add [ModCS.Npc.Caret](/api/objects/caret/), which contains API for spawning and modifying Carets.
- Credit bitmaps, Pixel.bmp and ORGs are now contained in the `data` folder rather than in game resources.
- Add `caret.tbl` and `music.tbl` files to the `data` folder.
- Add `xm`, `ym` and `boost_fuel` to [ModCS.Player](/api/objects/player/).
- Add [ModCS.Npc.OffsetRect()](/api/objects/npc/functions/#modcsnpcoffsetrect).
- Add [ModCS.Npc.CheckBit()](/api/objects/npc/bits/#modcsnpccheckbit).
- Add [ModCS.Game.IsNew()](/api/game/#modcsgameisnew).
- Fix an issue involving [ModCS.Tsc.Jump()](/api/tsc/#modcstscjump) skipping characters.
- The title screen will now display the [mod version](/api/mod/#modcsmodsetversion) rather than the ModCS version.
- Remove and fix some warnings.
- Update examples.

### Updating

To update from ModCS 0.1.0.0:

1. Replace your ModCS executable with a ModCS 0.1.1.0 one.
2. From a vanilla ModCS 0.1.1.0 install copy the `caret.tbl` and `music.tbl` files to your mod's `data` folder.
3. Move all ORG files from Resources to a `data/Org` folder.
4. Move all Credit bitmaps from Resources to a `data/Credits` folder.
5. Move the PIXEL bitmap from Resources to the `data` folder.

### Download

[:material-download: Download ModCS 0.1.1.0](/assets/releases/modcs0110.zip)

## ModCS 0.1.0.0

Initial ModCS Release.

### Changelog

!!! Note
	This is the changelog from version 0.0.1.2, the version used for the mod [Doku Goes To McDonalds](https://doukutsuclub.knack.com/database#search-database/mod-details/5fbab65b03e82f001bcd17e7/).

- Added "Examples" folder to `data/Scripts`.
- Added [ModCS.Surface.Screenshot()](/api/drawing/surface/#modcssurfacescreenshot).

### Download

[:material-download: Download ModCS 0.1.0.0](/assets/releases/modcs0100.zip)

