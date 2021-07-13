# ModCS.Player

The **ModCS.Player global object** represents the player (Also known as My Character/ MYC).

ModCS.Player is userdata. You may access and edit the following values from it:

| Value        | Type                                 | Usage                                                        |
| ------------ | ------------------------------------ | ------------------------------------------------------------ |
| `x`          | [Pixel Unit](/api/objects/pixel/)    | The player's X position.                                     |
| `y`          | [Pixel Unit](/api/objects/pixel/)    | The player's Y position.                                     |
| `xm`         | [Pixel Unit](/api/objects/pixel/)    | X velocity of the Player.                                    |
| `ym`         | [Pixel Unit](/api/objects/pixel/)    | Y velocity of the Player.                                    |
| `ani_no`     | Number (Casted to integer)           | Animation frame value.                                       |
| `ani_wait`   | Number (Casted to integer)           | Animation timer value.                                       |
| `direct`     | [Direction](/api/objects/direction/) | The player's direction.                                      |
| `boost_fuel` | Number (Casted to integer)           | The fuel of the Player's [Booster](/api/objects/player/equip/). |
| `air`        | Number (Casted to integer)           | Air value of the player.                                     |

## ModCS.Player.IsHit()

```lua
ModCS.Player.IsHit()
```

Returns true if the player is being hit. Returns false otherwise.

## ModCS.Player.IsLookingDown()

```lua
ModCS.Player.IsLookingDown()
```

Returns true if the player is looking down. Returns false otherwise.

## ModCS.Player.IsLookingUp()

```lua
ModCS.Player.IsLookingUp()
```

Returns true if the player is looking up. Returns false otherwise.

## ModCS.Player.GetLife()

```lua
ModCS.Player.GetLife()
```

Returns the player's current life points.

## ModCS.Player.AddLife()

```lua
ModCS.Player.AddLife(life)
```

Adds `life` to the player's life points.

## ModCS.Player.GetMaxLife()

```lua
ModCS.Player.GetMaxLife()
```

Returns the player's current maximum life points.

## ModCS.Player.AddMaxLife()

```lua
ModCS.Player.AddMaxLife(life)
```

Adds `life` to the player's max life points.

## ModCS.Player.Damage()

```lua
ModCS.Player.Damage(damage)
```

Damages the player by `damage`.

## ModCS.Player.SetRect()

```lua
ModCS.Player.SetRect(left, top, right, bottom)
ModCS.Player.SetRect(rect)
```

Sets the [Rect](/api/drawing/rect/) of the player to a Rect with `left`, `top`, `right`, `bottom`.

If a `rect` is specified, set the Rect of the player to that Rect instead.

## ModCS.Player.GetRect()

```lua
ModCS.Player.GetRect()
```

Returns the player's [Rect](/api/drawing/rect/).

## ModCS.Player.OffsetRect()

```lua
ModCS.Player.OffsetRect(left, top, right, bottom)
```

Adds `left`, `top`, `right`, `bottom` to the the `left`, `top`, `right`, `bottom` values of the [Rect](/api/drawing/rect/) of the player.

`right` and `bottom` are optional parameters. If they are not specified, `left` and `top` will be used in their place instead.

## ModCS.Player.SetViewbox()

```lua
ModCS.Player.SetViewbox(front, top, back, bottom)
ModCS.Npc.SetViewbox(rangerect)
```

Sets the sprite offset of the Player to a [RangeRect](/api/objects/range/) with `front`, `top`, `back`, `bottom`.

If a `rangerect` is specified, set the sprite offset of the Player to that RangeRect instead.

## ModCS.Player.GetViewbox()

```lua
ModCS.Player.GetViewbox()
```

Returns the sprite offset [RangeRect](/api/objects/range/) of the player.

## ModCS.Player.SetArmsYOffset()

```lua
ModCS.Player.SetArmsYOffset(offset)
```

Sets the vertical sprite offset of the weapon sprite next to the player to `offset`.