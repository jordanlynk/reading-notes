# Chapter 3: "Lists"

- _Ordered Lists_: lists where items in the list is numbered
- _Unordered Lists_: lists that begin with a bullet point
- _Definition Lists_: made up of a set of terms along with the definitions for each of those terms

- **ol = ordered list**
- li = each item in the list
- **ul = unordered list**
- li = each item in the list
- **dl = definition list**
- dt = contains the term being defined
- dd = contains the definition
- ## Nested Lists**
- can be placed inside the li element to create a second list

## Summary:
- Three types of HTML lists: ordered, unordered and definition
- Ordered lists use numbers
- Unordered lists use bullets
- Definition lists define terminology
- Lists can be nested in one another

# Chapter 13: "Boxes"

- _Box Dimensions_: Width & Height
- _Limiting Width_: Min-width, specifies the smallest size a box can be displayed at when the browser window is narrow. Max-width, makes sure that lines of texts do not appear too wide within a big browser window.
- _Limiting Height_: Min-Height & Max-Height
- _Overflowing Content_: overflow; hidden is the property that hides any extra content that does not fit in the box. scroll, this property adds a scrollbar to the box so that users can scroll to see the missing content
- _Border Width_: controls the width of a border. values; thin, med & thick, border-top-width, border-right-width, border-bottom-width, border-left-width
- _Border Style_: controls the style of a border using the border-style property
- solid; single solid line
- dotted; square dots 
- dashed; short lines
- double; two solid lines
- groove; appears to be carved into the page
- ridge; sticks out from the page
- inset; embedded onto the page
- outset; coming out of the screen
- hidden/none; no border is shown
_Border Color_:
- border-top-color
- border-right-color
- border-bottom-color
- border-left-color
_Shorthand Border_:
- border; specifies the width, style and color of a border
_Padding_:
- padding; specifies how much space should appear between the content of the element and the border
- padding-top
- padding-right 
- padding-bottom
- padding-left
_Margin_:
- margin; controls the gap between boxes
- margin-top
- margin-right
- margin-bottom
- margin-left
_Centering Content_:
- if you want to center a box on the page, you can set the left or right margin to auto. In order to center the box you set a width for the box

- **CSS treats HTML elements are it's own box**
- **CSS can control the dimensions of a box, along with borders, margins and padding for each box**
- **You can hide elements using the display and visibility properties**
- **Block-level boxes can turn into inline boxes and vice versa**
- **Legibility can be altered by changing the width of boxes containing text & the leading**
- **CSS3 has the ability to create image and rounded borders**

# JS Chapter 2 Review:

- _Arrays_: can store a list of values. You should consider it an array when working with a _list_ or set of values that are _related_ to one another.
- _Creating An Array_: start with var, then name your array. Also referred to as _array literal_
- _Values In Arrays_: values are accessed as if they're in a numbered list. The start of numbering on this list starts at 0 and not 1.

# Chapter 4: Decisions and Loops

- _If...Else Statements_: checks a condition, if the resolve is true the first block is executed. If it resolves to false, the second block is run instead.
- _Switch Statements_: starts with a var called the switch value. Indicates a possible value for the var and the code that should run if the variable matches that value.
_Logical Operators_:
- Comparison operators usually return single values of true or false. Logical operators allow you to compare the results of more than one comparison operator.
- && logical and; this operator tests more than one condition. If both expressions evaluate to true than the expression returns to true. If just one of these returns false, then the expression will return false.
true && true return true
true && false return false
false && true return false
false && false return false
- | | logical or; tests at least one condition. If either expression evaluates to true, then the expression returns true. If both return false, then the expression will return false.

- ! Logical Not; this operator takes a single Boolean value and inverts it. This reverses the state of an expression. If it was false (without the ! before it) it would return true. If the statement was true, it would return false.
- Logical Expressions are evaluated left to right. If the first condition can provide enough info to get the answer, then there is no need to evaluate the second condition.

_Loops_:
- Loops check a condition. If it returns true, a code block will run. Then the condition will be checked again and if it still returns true, the code block will run again. It repeats until the condition returns false. There are three types of common loops:
- For; if you need to run code a specific # of times, use a _for_ loop. In a _for_ loop, the condition is usually a counter which is used to tell how many times the loop should run.
- While; If you do know how many times the code should run, you can use a _while_ loop. The condition can be something other than a counter to loop for as long as the condition is true.
-Do While; It will always run the statements inside the curly braces at least once, even if the condition evaluates to false.

- **Conditionals allow your code to make decisions on what to do next**
- **Logical operators allow you to combine more than one set of comparisons**
- **if...else allow you to run one set of code with conditions that are true or false**
- **Switch statements compare a value against possible outcomes, can also provide a default option if there's no match**
- **All values evaluate to truthy or falsy**
- **Three types of loops: for, while and do...while. Each repeats a set of statements**






