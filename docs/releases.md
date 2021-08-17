# ModCS Releases

Old releases will not be supported.

## ModCS 0.2.1.1

??? Info "Changelog"
	- Make the `pNpc` value of [ModCS.Npc](/api/objects/npc/)s return `nil` if it doesn't contain an NPC.

### Updating

To update from ModCS 0.2.1.0:

- Replace your ModCS executable with a ModCS 0.2.1.1 one.

### Download

[:material-download: Download ModCS 0.2.1.1](/assets/releases/modcs0211.zip)

## ModCS 0.2.1.0

??? Info "Changelog"
	- Add functions for adding and removing EXP from the player to [ModCS.Arms](/api/inventory/arms/).
	- Add [ModCS.Arms.GetLevels()](/api/inventory/arms/#modcsarmsgetlevels).
	- Add [ModCS.Npc.TriggerBox()](/api/objects/npc/functions/#modcsnpctriggerbox).
	- Change ModCS.Organya to [ModCS.Music](/api/sound/music/).
	- Update examples.

### Updating

To update from ModCS 0.2.0.1:

- Replace your ModCS executable with a ModCS 0.2.1.0 one.

### Download

[:material-download: Download ModCS 0.2.1.0](/assets/releases/modcs0210.zip)

## ModCS 0.2.0.1

??? Info "Changelog"
	- Fix an issue with the new way of defining [custom TextScript commands](/api/tsc/#custom-commands).
	- Fix an issue with the Polar Star recreation example script.

### Updating

To update from ModCS 0.2.0.0:

- Replace your ModCS executable with a ModCS 0.2.0.1 one.

### Download

[:material-download: Download ModCS 0.2.0.1](/assets/releases/modcs0201.zip)

## ModCS 0.2.0.0

??? Info "Changelog"
	- Add [ModCS.Arms](/api/inventory/arms/) and [ModCS.Item](/api/inventory/item/), which contain API for reading and modifying the inventory.
	- Add [ModCS.Bullet](/api/objects/bullet/), which contains API for spawning and modifying Bullets.
	- Add [ModCS.Camera](/api/camera/) which contains API for modifying and reading the in-game camera.
	- Add `arms_level.tbl` file to the `data` folder.
	- Add [multiple tile layers](/pxl/).
	- Custom game object Act functions will now be ran from an `Act` array contained in the game object's class namespace.
	- [Custom TSC Commands](/api/tsc/#custom-commands) will now be ran from a ModCS.Tsc.Command namespace.
	- Add [ModCS.Game.CanControl()](/api/game/#modcsgamecancontrol) and [ModCS.Game.CanAct()](/api/game/#modcsgamecanact).
	- Add [ModCS.Tsc.IsRunning()](/api/tsc/#modcstscisrunning).
	- Add [ModCS.Game.Update()](/api/game/#modcsgameupdate).
	- Add functions to [ModCS.Player](/api/objects/player/) for modifying the Player's [Rect](/api/drawing/rect/) and viewbox.
	- Add [ModCS.Player.SetArmsYOffset()](/api/objects/player/#modcsplayersetarmsyoffset).
	- Add [ModCS.Player.GetMaxLife()](/api/objects/player/#modcsplayergetmaxlife).
	- Add functions to game object classes that return things such as a game object's [Rect](/api/drawing/rect/), Viewbox or Hitbox.
	- Make game objects' ActCode functions' type parameter optional.
	- Make `tgt_x` and `tgt_y` accessible from [ModCS.Npc](/api/objects/npc/)s\*.
	- Add functions to [ModCS.Stage](/api/stage/) for reading every [Stage Table](/api/stage/#stage-table) parameter.
	- Add [ModCS.Mod.SetSpikeDamage()](/api/mod/#modcsmodsetspikedamage).
	- Add functions to [ModCS.Organya](/api/sound/music/) for getting and setting the position of the current playing track and setting the volume.
	- Add [ModCS.Organya.GetCurrent()](/api/sound/music/#modcsmusicgetcurrent).
	- Add [ModCS.Organya.GetOld()](/api/sound/music/#modcsmusicgetold) and [ModCS.Organya.GetOldPosition()](/api/sound/music/#modcsmusicgetposition).
	- Add functions to [ModCS.Sound](/api/sound/sound/) for modifying frequency, volume and panning of individual sound effects.
	- Add an optional direction argument to [ModCS.Caret.Spawn()](/api/objects/caret/#modcscaretspawn).
	- [ModCS.RangeRect](/api/objects/range/)s now use [Pixel Units](/api/objects/pixel/).
	- Make [ModCS.Game.Act()](/api/game/#modcsgameact) run during a `<PRI`.
	- Make [ModCS.Game.Act()](/api/game/#modcsgameact) run before any menu code on the Title Screen ([Game Mode](/api/game/#modcsgamegetmode) 2).
	- Make [ModCS.Game.Init()](/api/game/#modcsgameinit) run right before game modes enter a loop.
	- Merge [ModCS.Rect.Put2Surface()](/api/deprecated/#modcsrectput2surface) with [ModCS.Rect.Put()](/api/drawing/rect/#modcsrectput).
	- Make the bundled DoConfig display "640x480 Windowed" as the default window mode.
	- Rework a lot of things internally.
	- Update warnings.
	- Update examples.

### Updating

To update from ModCS 0.1.1.2:

1. Replace your ModCS executable with a ModCS 0.2.0.0 one.
2. From a vanilla ModCS 0.2.0.0 install copy the `arms_level.tbl` file to your mod's `data` folder.

#### Incompatibility with older releases

ModCS 0.2.0.0 has some incompatibility with older versions of the API.

- In previous versions, while not documented, `tgt_x` and `tgt_y` values were accessible from [ModCS.Npc](/api/objects/npc/)s. However, they were not returned as [Pixel Units](/api/objects/pixel/), resulting in the values being multiplied by 512 for some NPCs. From 0.2.0.0 onward they will be returned as Pixel Units.
- Some userdata such as [ModCS.Rect](/api/drawing/rect/)s supported uservalues. This feature has been removed in 0.2.0.0.

### Download

[:material-download: Download ModCS 0.2.0.0](/assets/releases/modcs0200.zip)

## ModCS 0.1.1.2

??? Info "Changelog"
	- Fix an issue where [ModCS.Rect.Put2Surface()](/api/deprecated/#modcsrectput2surface) would fail drawing if there were parts of the [Rect](/api/drawing/rect/) being drawn off the target [Surface](/api/drawing/surface/).

### Updating

To update from ModCS 0.1.1.1:

- Replace your ModCS executable with a ModCS 0.1.1.2 one.

### Download

[:material-download: Download ModCS 0.1.1.2](/assets/releases/modcs0112.zip)

## ModCS 0.1.1.1

??? Info "Changelog"
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

??? Info "Changelog"
	- Add [ModCS.Caret](/api/objects/caret/), which contains API for spawning and modifying Carets.
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

??? Info "Changelog"
	!!! Note
		This is the changelog from version 0.0.1.2, the version used for the mod [Doku Goes To McDonalds](https://doukutsuclub.knack.com/database#search-database/mod-details/5fbab65b03e82f001bcd17e7/).

	- Added "Examples" folder to `data/Scripts`.
	- Added [ModCS.Surface.Screenshot()](/api/drawing/surface/#modcssurfacescreenshot).

### Download

[:material-download: Download ModCS 0.1.0.0](/assets/releases/modcs0100.zip)

