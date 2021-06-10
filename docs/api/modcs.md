# ModCS Object - Basics

All of ModCS's API is contained in the **ModCS global namespace**.

## ModCS.WriteLog()

```lua
ModCS.WriteLog(text, number1, number2, number3)
```

Write given data to a `debug.txt` file located in the same directory as the executable.

All number parameters are optional, and will be casted to integers.

## ModCS.PutText()

```lua
ModCS.PutText(text, x, y, color, surface)
```

Draw given text to screen at coordinates `x` and `y`.  `color` and `surface` parameters are optional. 

If a color is not specified the text will have the color `255, 255, 254` (`#FFFFFE`).

When a surface is specified, ModCS.PutText will draw to given surface instead.

## ModCS.PutNumber()

```lua
ModCS.PutNumber(number, x, y, zero, surface)
```

Draw given number to screen at coordinates `x` and `y`.  `zero` and `surface` parameters are optional. 

Number parameters over 9999 will display capped.

`zero` is a Boolean. If set to true a zero will be shown to the left of the number. This only applies to one-digit numbers.

When a surface is specified, ModCS.PutNumber will draw to given surface instead.

## ModCS.GetFullRect()

Returns a full [ModCS.Rect](/api/drawing/rect/).
This rect will usually equal to this:
```lua
{
	left = 0,
    top = 0,
    right = 320,
    bottom = 240
}
```

## ModCS.GetGameRect()

Returns the canvas [ModCS.Rect](/api/drawing/rect/) of the game.
This rect will usually equal to this:
```lua
{
	left = 0,
    top = 0,
    right = 320,
    bottom = 240
}
```
During the credits sequence the rect's `left` value will equal to 160.

!!! Note
	The main difference between ModCS.GetGameRect() and ModCS.GetFullRect() is how both values are used in the original game itself. The full Rect is often the default view limitng value for drawing a bitmap, while the game Rect is the view limiting value for game related objects (NPCs, player, map tiles, etc.). You can use these Rects with [ModCS.Rect.PutEx()](/api/drawing/rect/#modcsrectputex)