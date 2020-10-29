# SMACSS and Responsive Web Data

# Responsive Web Design

## Responsive Overview
- Responsive web design is the practice of building a website suitable to work on every device and screen size. It is focused around providing an user friendly and intuitive experience for all users. 

## Responsive vs. Adaptive vs. Mobile
- Responsive and adaptive web design are closely related, and are often portrayed as one in the same. Responsive generally reacts quickly & positively to any change, while adaptive means to be easily modified for a new purpose or situation, aka change. With responsive design websites continually and fluidly change based on different factors, while adaptive are built to a group of preset factors. A combo of the two is ideal.
- Mobile generally means to build a seperate website commonly on a new domain solely for mobile users. Mobile websites can be extremely light and come with a dependency on a new code base and browser sniffing. This can be an obstacle for both developers and users.
## Flexible Layouts
- Responsive web design is broken down into three main components: flexible layouts, media queries, and flexible media
- *Flexible Layouts* builds the layout of a website with a flexible grid, which is capable of dynamically resizing to any width. Flexible grids are built using relative length units, most commonly percentages or em units. These relative lengths are then used to declare common grid property values such as width, margin, or padding. Flexible layouts do not advocate the use of fixed measurement units, such as pixels or inches.
- *Flexible Grid* Taking the flexible layout concept, and formula, and reapplying it to all parts of a grid will create a completely dynamic website, scaling to every viewport size. For even more control within a flexible layout, you can also leverage the min-width, max-width, min-height, and max-height properties. The flexible layout approach alone isn’t enough. At times the width of a browser viewport may be so small that even scaling the the layout proportionally will create columns that are too small to effectively display content. Specifically, when the layout gets too small, or too large, text may become illegible and the layout may begin to break. In this event, media queries can be used to help build a better experience
- *Media Queries*  built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation. You can use @media rule inside of an existing style sheet, importing a new style sheet using the @import rule, or by linking to a separate style sheet from within the HTML document. Generally speaking it is recommend to use the @media rule inside of an existing style sheet to avoid any additional HTTP requests. Each media query may include a media type followed by one or more expressions. Common media types include all, screen, print, tv, and braille.
- *Logical Operators in Media Queries* help build powerful expressions. 3 different logical operators available for use: and, not and only. Using *and* allows an extra condition to be added, making sure that a browser or devices does both a, b, c, (example). The *not* negates the query, specifiying any query but the one identified. The *only* is a new operator and is not recognized by user agents using the HTML4 algorithm, therefore hiding the styles from devides or browsers that don't support media queries.
- *Media Features in Media Queries* knowing media query syntax and how the logical operators work is a great place to start with media queries.
- *Heigh and Width Media Features* use height and width media features, as well as min or max, min-width or max-width. 
- *Orientation Media Feature* The orientation media feature determines if a device is in the landscape or portrait orientation. The landscape mode is triggered when the display is wider than taller, and the portrait mode is triggered when the display is taller than wider. This media feature plays a large part with mobile devices.
- *Aspect Ratio Media Features* The aspect-ratio and device-aspect-ratio features specifies the width/height pixel ratio of the targeted rendering area or output device. The min and max prefixes are available to use with the different aspect ratio features, identifying a ratio above or below that of which is stated. The value for the aspect ratio feature consist of two positive integers separated by a forward slash. The first integer identifies the width in pixels while the second integer identifies the height in pixels.
# All About Floats:
- *Float* is a CSS positioning property. In a print layout, images may be set into the page so that the text wraps around them as needed. Commonly known as "text wrap"
- In page layouts, boxes that hold the text can be told to adhere to the text wrap or ignore it. Ignoring it will allow the words to flow right over an image. This is a key difference between that image being part of the *flow* of the page (or not).
- Page elements with CSS *float* property applied to them are just like images in the print layout where the text flows around them. Floated elements remain a part of the flow of the web page. Absolute positioned page elements are *removed* from the flow of the page. Absolute positioned page elements will not affect the position of other elements and vice versa. 
## Valid Values for float property: 
-*Left and Right* float elements those directions. 
-*None* makes sure an element does not move and 
- *Inherit* which will assume the float value from that elements partent element.
## What are floats used for?
- Wrapping text around images, floats can also create entire web layouts
- Floats are also beneficial when using in smaller instances
## Clearing Float
- *clear* will make it so that an object will not move up adjacent to the float like the float desires, but will instead move itself down past the float.
## Valid Values for Clear
- *Both* clears float coming from either direction
- *Left and Right* can be used to only clear float from one direction respectively.
- *None* is default, typically will not use unless removing a clear value from a cascade
- *Inherit* only clears the left or right float, very unlikely to use this.
## The Great Collapse
- Floats can affect the element that contains them(parent element). If said parent element contained nothing but floated elements, the height of it would collapse to nothing. This is not always noticeable but something to be aware of
- If a block element on top were to have auto expanded to accommodate the floated element, there would be unnatural spacing break in the flow of text coming between paragraphs, with really no way to fix it.
- Collapsing almost always need to be dealt with to prevent strange layout and cross-browser problems. It is fixed using the float *after* the floated elements in the container but *before* the close of the container.
## Techniques for Clearing Floats
- If you always know what the succeeding element is, you can utilize *clear:both;* 
- *Empty Div Method* is exactly what it sounds like. "<div style="clear: both;"></div>" *Div* is more commonly used as it has no browser default styling and doesn't have any special function, it is also unlikely to be generically styled with CSS.
## Overflow Method
- Relies on setting the overflow CSS property on a parent element. If property is set to auto or hidden on the parent, the parent will expand to contain the floats, clearing it for succeeding elements.
## Easy Clearing Method
- Utilizes a CSS pseudo selecter (:after) to clear floats. Instead of setting the overflow on the parent, you apply an additional class such as "clearfix" to it.
## Problems with Floats
- *Pushdown* is a symptom of an element inside a floated item being wider than the float itself(typically an image). Most browsers will render the image outside the float, but not have the part sticking out affect other layout. 
- *Double Margin Bug* If you apply a margin in the same direction as the float, it will double the margin. Quick fix: "display: inline" on the float.
- *3px Jog* when text that is up next to a floated element is mysteriously kicked away by 3px. Quick fix: set a width or height on the affected text
- *Bottom Margin Bug* when a floated parent has floated children inside it, bottom margin on those children is ignored by the parent. Quick fix: use bottom padding on the parent
