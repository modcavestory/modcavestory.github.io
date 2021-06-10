# ModCS.Mod

The **ModCS.Mod namespace** contains functions related to customizing releases of mods.

## ModCS.Mod.SetName()

```lua
ModCS.Mod.SetName(name)
```

Sets the window title of the game to `name`. This function will only work at top-level.

## ModCS.Mod.SetAuthor()

```lua
ModCS.Mod.SetAuthor(name)
```

Sets the author of game to `name`. The author will be displayed in the version window.

## ModCS.Mod.SetVersion()

```lua
ModCS.Mod.SetVersion(v1, v2, v3, v4)
```

Sets the version of the game to `v1`.`v2`.`v3`.`v4`. This version will be in the version window.

## ModCS.Mod.SetOpening()

```lua
ModCS.Mod.SetOpening(no, eve, wait)
```

Use [Stage](/api/stage/) `no` for the opening sequence ([Game Mode](/api/game/#modcsgamegetmode) 1). `eve` and `wait` are optional parameters.

If `eve` is specified [Event](/api/tsc/#events) `eve` will run once the opening sequence starts, otherwise Event 0 will run.

If `wait` is specified, wait `wait` ticks during the opening before transferring to the title screen.

## ModCS.Mod.SetStart()

```lua
ModCS.Mod.SetStart(no, x, y, eve)
```

Sets the default New Game starting point. Parameters are the same as the [ModCS.Stage.Transfer() function](/api/stage/#modcsstagetransfer).