# SPWN-Canvas

Simple SPWN canvas for all your needs

## Usage

1) Copy `canvas.spwn` in your directory
2) Import canvas with `canvas = import 'canvas.spwn'`
3) Create a new canvas (see below)
4) You're ready to go!

## Methods

### new

Creates a new canvas.

```spwn
myCanvas = canvas.new(
    x,y,            // position
    width,height,   // width and height in pixels
    scale?,         // the pixel-scaling of the canvas
    groups?         // the group(s) it should add to all the pixels of the canvas (array or group)
)

myCanvas = canvas.new(
    10,10,
    31,31,
    0.7,
    ?g
)
```

### setColor

Sets the current color for drawing.

```spwn
myCanvas.setColor(r,g,b)

myCanvas.setColor(255,192,203)
```

### drawPixel

Draws one pixel on the canvas

```spwn
myCanvas.drawPixel(x,y)

myCanvas.drawPixel(1,3)
```

### drawRect

Draws a rectangle on the canvas

```spwn
myCanvas.drawRect(x,y,width,height)

myCanvas.drawRect(3,4,5,2)
```

### drawFill

Draws the entire canvas

```spwn
myCanvas.drawFill()
```

### drawEllipse

Draws an ellipse on the canvas

```spwn
myCanvas.drawEllipse(x,y,width,height)

myCanvas.drawEllipse(4,5,4,7)
```

### drawCircle

Draws a circle on the canvas

```spwn
myCanvas.drawEllipse(x,y,radius)

myCanvas.drawEllipse(3,2,6)
```
