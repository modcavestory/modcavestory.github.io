# Caret Manipulation Functions

## ModCS.Caret.SetRect()

```lua
ModCS.Caret.SetRect(crt, left, top, right, bottom)
ModCS.Caret.SetRect(crt, rect)
```

Sets the [Rect](/api/drawing/rect/) of `crt` to a Rect with `left`, `top`, `right`, `bottom`.

If a `rect` is specified, set the Rect of `crt` to that Rect instead.

## ModCS.Caret.ActCode()

```lua
ModCS.Caret.ActCode(crt, carettype)
```

Runs the action code for [Caret Type](/api/objects/caret/id/) `carettype` to `crt`.

!!! Note
	This will run the *vanilla* act code for `crttype`. To run any overwritten act functions, run `ModCS.Caret.ActX(crt)` instead (where X is the Caret Type ID). 

## ModCS.Caret.Delete()

```lua
ModCS.Caret.Delete(crt)
```

Deletes `crt`.

## ModCS.Caret.Move()

```lua
ModCS.Caret.Move(crt)
```

Adds `xm` and `ym` of `crt` to `crt`'s `x` and `y`. 
