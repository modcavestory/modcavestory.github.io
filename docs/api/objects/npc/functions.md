# NPC Manipulation Functions

## ModCS.Npc.SetRect()

```lua
ModCS.Npc.SetRect(npc, left, top, right, bottom)
ModCS.Npc.SetRect(npc, rect)
```

Sets the [Rect](/api/drawing/rect/) of `npc` to a Rect with `left`, `top`, `right`, `bottom`.

If a `rect` is specified, set the Rect of `npc` to that Rect instead.

## ModCS.Npc.SetHitbox()

```lua
ModCS.Npc.SetHitbox(npc, front, top, back, bottom)
ModCS.Npc.SetHitbox(npc, rangerect)
```

Sets the hitbox of `npc` to a [RangeRect](/api/objects/range/) with `front`, `top`, `back`, `bottom`.

If a `rangerect` is specified, set the hitbox of `npc` to that RangeRect instead.

!!! Warning
	When editing NPC hitboxes make sure that the front and back values of the hitbox are the same, otherwise you might get weird hitbox behavior.

## ModCS.Npc.SetViewbox()

```lua
ModCS.Npc.SetViewbox(npc, front, top, back, bottom)
ModCS.Npc.SetViewbox(npc, rangerect)
```

Sets the sprite offset of `npc` to a [RangeRect](/api/objects/range/) with `front`, `top`, `back`, `bottom`.

If a `rangerect` is specified, set the sprite offset of `npc` to that RangeRect instead.

## ModCS.Npc.ActCode()

```lua
ModCS.Npc.ActCode(npc, npctype)
```

Runs the action code for [NPC Type](/api/objects/npc/id/) `npctype` to `npc`.

!!! Note
	This will run the *vanilla* act code for `npctype`. To run any overwritten act functions, run `ModCS.Npc.ActX(npc)` instead (where X is the NPC Type ID). 

## ModCS.Npc.IsHit()

```lua
ModCS.Npc.IsHit(npc)
```

Returns true if `npc` is being hit by a bullet. Returns false otherwise.

## ModCS.Npc.Delete()

```lua
ModCS.Npc.Delete(npc)
```

Deletes `npc`. Same effect as `<DNP`.

## ModCS.Npc.Kill()

```lua
ModCS.Npc.Kill(npc)
```

Kills `npc`.

## ModCS.Npc.KillOnNextFrame()

```lua
ModCS.Npc.KillOnNextFrame(npc)
```

Sets `npc` for deletion on the next frame.

## ModCS.Npc.Move()

```lua
ModCS.Npc.Move(npc)
```

Adds `xm` and `ym` of `npc` to `npc`'s `x` and `y`. 

## ModCS.Npc.Move2()

```lua
ModCS.Npc.Move2(npc)
```

Adds `xm2` and `ym2` of `npc` to `npc`'s `x` and `y`. 