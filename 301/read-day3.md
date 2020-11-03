# Readings: Mustache and Flexbox

## Templating with Mustache
- *Javascript Templating* is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source. The template is HTML markup, with added templating tags that will eitehr insert variables or run programming logic. 
- Template engine replaces variables & instances declared in a template file with actual values at runtime and convert the template to HTML file that is sent to the client.
- *Mustache* is a logic-less template syntax. It can be used for HTML, config files, source code, etc. It works by expanding tags in a template using values provided in a hash or object. Often referred to as "logic-less" becuase there are no if statements, else clauses or for loops, only tags. Some tags might be replaced w/ a value, some with nothing and others a series of values.
- *mustache.js* is an implementation of the mustache template system in JavaScript.
- When they are two braces around {{ name }}, this is *mustache* syntax. It shows that it is a placeholder. When Mustache compiles this, it will look for the ‘name’ property in the object we pass in, and replace {{ name }} with the actual value.
- Mustache is not a templating engine. Mustache is a *specification for a templating language.*
- If you intend you use mustache with Node and Express, you can use mustache-express. Mustache Express lets you use Mustache and Express together easily.

## A Guide To Flexbox:
- *The Flexbox Layout* aka *Flexible Box* module, aims at providing a more efficient way to lay out, align and distribute space among items in a container, even when their size is unknown and/or dynamic.
- Main idea behind flex layout is to give the container the ability to alter its items’ width/height and order, to best fill the available space. 
- A flex container expands items to fill available free space or shrinks them to prevent overflow.
- Flexbox layout is *direction-agnostic* as opposed to the regular layouts.
- **Flexbox layout is most appropriate to the components of an application, and small-scale layouts, while the Grid layout is intended for larger scale layouts**
- *Terminology*:
- *main axis* – main axis of a flex container is the primary axis along which flex items are laid out.
- *main-start | main-end* – flex items are placed within the container starting from main-start and going to main-end.
- *main size* – flex item’s width or height, whichever is in the main dimension, is the item’s main size. The flex item’s main size property is either the ‘width’ or ‘height’ property, whichever is in the main dimension.
- *cross axis* – Axis perpendicular to the main axis is called the cross axis. Its direction depends on the main axis direction.
- *cross-start | cross-end* – Flex lines are filled with items and placed into the container starting on the cross-start side of the flex container and going toward the cross-end side.
- *cross size* – Width or height of a flex item, whichever is in the cross dimension, is the item’s cross size. The cross size property is whichever of ‘width’ or ‘height’ that is in the cross dimension.
- **Properties for the Parent (flex container)**
- *display*: defines a flex container; inline or block depending on the given value. Enables a flex content for all its direct children.
- *flex-direction*: establishes the main-axis, therefore defining the direction flex items are placed in the flex container. Flexbox is a single direction layout concept. 
- *flex-wrap*: flex items will all try to fit onto one line. nowrap= all items will be on one line. wrap= items will wrap onto multiple lines from top to bottom. wrap-reverse= will wrap onto multiple lines from bottom to top.
- *flex flow*: This is a shorthand for the flex-direction and flex-wrap properties, which together define the flex container’s main and cross axes.
- *justify-content*: defines the alignment along the main axis.
- *align-items*: defines the default behavior for how flex items are laid out along the cross axis on the current line.
- *align-content*: aligns a flex container's lines within when there is extra space in cross-aix, similar to how justify-content aligns individual items within main-axis.
- **Properties for the Children(flex items)**
- *order*: by default, flex items are laid out in the source order. However, the order property controls the order in which they appear in the flex container.
- *flex-grow*: defines the ability for a flex item to grow if necessary. It accepts a unitless value that serves as a proportion. It dictates what amount of the available space inside the flex container the item should take up.
- *flex-shrink*: defines the ability for a flex item to shrink if necessary.
- *flex-basis*: This defines the default size of an element before the remaining space is distributed.
- *flex*: This is the shorthand for flex-grow, flex-shrink and flex-basis combined. The second and third parameters (flex-shrink and flex-basis) are optional. The default is 0 1 auto, but if you set it with a single number value, it’s like 1 0.
- *align-self*: This allows the default alignment (or the one specified by align-items) to be overridden for individual flex items.