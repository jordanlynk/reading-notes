# Basic Usage of Canvas
- Canvas element only has two attributes, width and height. They are both optional and can also be set using DOM properties. When neither of these two are specified, the canvas will be 300px wide and 150px high. 
- It can be styled just like any image, margin, border, background, etc. These rules, don't affect the actual drawing of the canvas. 
- Fallback Content: the canvas tag is different in the way that it is easy to define some fallback content, to be displayed in older browsers not supporting it. 
- Required Tags: unlike img tags, the canvas tag requires a closing tag.
- The <canvas> element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. In this tutorial, we focus on the 2D rendering context.
- The script includes a function called draw(), which is executed once the page finishes loading; this is done by listening for the load event on the document. This function, or one like it, could also be called using window.setTimeout(), window.setInterval(), or any other event handler, as long as the page has been loaded first.
# Drawing Shapes:
- Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y)
- fillRect(x, y, width, height); Draws a filled rectangle.
- strokeRect(x, y, width, height); Draws a rectangular outline.
- clearRect(x, y, width, height); Clears the specified rectangular area, making it fully transparent.
- Each of these three functions takes the same parameters. x and y specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle. width and height provide the rectangle's size.
- The fillRect() function draws a large black square 100 pixels on each side. The clearRect() function then erases a 60x60 pixel square from the center, and then strokeRect() is called to create a rectangular outline 50x50 pixels within the cleared square.
- beginPath(); Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
- Path methods; Methods to set different paths for objects.
- closePath(); Adds a straight line to the path, going to the start of the current sub-path.
- stroke(); Draws the shape by stroking its outline.
- fill(); Draws a solid shape by filling the path's content area.
- For drawing straight lines, use the lineTo() method.
- lineTo(x, y); Draws a line from the current drawing position to the position specified by x and y.
- To draw arcs or circles, we use the arc() or arcTo() methods.
- arc(x, y, radius, startAngle, endAngle, anticlockwise); Draws an arc which is centered at (x, y) position with radius r starting at startAngle and ending at endAngle going in the given direction indicated by anticlockwise (defaulting to clockwise).
- arcTo(x1, y1, x2, y2, radius); Draws an arc with the given control points and radius, connected to the previous point by a straight line.
# Colors:
- fillStyle = color; Sets the style used when filling shapes
- strokeStyle = color; Sets the style for shapes' outlines
- strokeStyle property to change the colors of the shapes' outlines
- globalAlpha = transparencyValue; Applies the specified transparency value to all future shapes drawn on the canvas. The value must be between 0.0 (fully transparent) to 1.0 (fully opaque). This value is 1.0 (fully opaque) by default.
- The globalAlpha property can be useful if you want to draw a lot of shapes on the canvas with similar transparency, but otherwise it's generally more useful to set the transparency on individual shapes when setting their colors
- The rgba() function is similar to the rgb() function but it has one extra parameter. The last parameter sets the transparency value of this particular color. The valid range is again between 0.0 (fully transparent) and 1.0 (fully opaque)
- *Line Styles*:
-lineWidth = value; Sets the width of lines drawn in the future.
- lineCap = type; Sets the appearance of the ends of lines.
- lineJoin = type; Sets the appearance of the "corners" where lines meet.
miterLimit = value; establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
- getLineDash(); Returns the current line dash pattern array containing an even number of non-negative numbers.
- setLineDash(segments); sets the current line dash pattern.
lineDashOffset = value; specifies where to start a dash array on a line.
# Drawing Text
- fillText(text, x, y [, maxWidth]); fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
- strokeText(text, x, y [, maxWidth]); strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
- The text is filled using the current fillStyle
- font = value; the current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
- textAlign = value; text alignment setting. Possible values: start, end, left, right or center. The default value is start.
- textBaseline = value; baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
direction = value; directionality. Possible values: ltr, rtl, inherit. The default value is inherit.
- measureText(); returns a TextMetrics object containing the width, in pixels, that the specified text will be when drawn in the current text style.
