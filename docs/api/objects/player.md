# ModCS.Player

The **ModCS.Player global object** represents the player (Also known as My Character/ MYC).

ModCS.Player is userdata. You may access and edit the following values from it:

| Value    | Type                                 | Usage                    |
| -------- | ------------------------------------ | ------------------------ |
| `x`      | [Pixel Unit](/api/objects/pixel/)    | The player's X position. |
| `y`      | [Pixel Unit](/api/objects/pixel/)    | The player's Y position. |
| `air`    | Number (Casted to integer)           | Air value of the player. |
| `direct` | [Direction](/api/objects/direction/) | The player's direction.  |

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

## ModCS.Player.AddMaxLife()

```lua
ModCS.Player.AddLife(life)
```

Adds `life` to the player's max life points.

## ModCS.Player.Damage()

```lua
ModCS.Player.Damage(damage)
```

Damages the player by `damage`.