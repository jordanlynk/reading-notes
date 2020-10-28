# SMACSS and Responsive Web Data

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
