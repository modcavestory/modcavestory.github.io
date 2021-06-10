# ModCS.Key

The **ModCS.Key namespace** contains functions for checking key presses.

All ModCS.Key functions follow a similar format:

```lua
ModCS.Key.Button(hold)
```

Returns `true` if the button is being pressed.

`hold` is an optional parameter and a Boolean. If set to `true` the function will return true if the button is being held.

## List of functions

```lua
ModCS.Key.Jump(hold) -- Can be set to either Z or X in DoConfig
ModCS.Key.Shoot(hold) -- Can be set to either X or Z in DoConfig
ModCS.Key.Arms(hold) -- A key
ModCS.Key.ArmsRev(hold) -- S key
ModCS.Key.Item(hold) -- Q key
ModCS.Key.Map(hold) -- W key
ModCS.Key.Ok(hold) -- Can be either the Jump button or Shoot button in DoConfig
ModCS.Key.Cancel(hold) -- Can be either the Shoot button or Jump button in DoConfig
ModCS.Key.Left(hold) -- Can be either Left arrow key or < in DoConfig
ModCS.Key.Up(hold) -- Can be either Up arrow key or L in DoConfig
ModCS.Key.Right(hold) -- Can be either Right arrow key or ? in DoConfig
ModCS.Key.Down(hold) -- Can be either Down arrow key or > in DoConfig
```