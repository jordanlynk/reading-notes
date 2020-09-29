# Basics of HTML, CSS & JS


## Chapter 2: "Text"
- HTML has 6 "levels" of headings: h1, h2, h3, h4, h5, h6
- <p> create a paragraph
- _Bold_ <b> makes characters appear bold
- _Italics_ <i> makes characters appear in italics
- _Superscript_ <sup> used to contain characters that should be superscript such as dates or mathematical concepts
- _Subscript_ <sub> used to contain characters that should be subscript. Commonly used with foot notes or chemical formulas
- _White Space_ add extra spaces or start some elements on new lines to create spaces in text
- _<br />_ adds a line break inside the middle of a paragraph
- _<hr />_ creates a break between themes
- _<strong>_ indicates it's content has strong importance
- _<em>_ indicates emphasis that subtly changes
- _<blockquote>_ used for longer quotes that use up a whole paragraph
- _<q>_ used for shorter quotes that sit in a paragraph
- _<abbr>_ abbreviation or an acronym uses this
- _<cite>_ used when referencing a piece of work
- _<dfn>_ used to reference the defining instance of a new term
- _<address>_  contains contact details for the author
- _<ins>_ shows content that has been inserted into a document
- _<s>_ something that is no longer accurate or relevant, that you don't want to delete

## HTML elements describe the structure of the page
## They provide emphasis on where semantic information should be placed, the meaning of any acronyms and when given text is a quotation

## Chapter 10: "Introducing CSS"
- _<link>_ tells the browser where to find the CSS file used to style the page
- _href_ specifies the path to the CSS file
- _type_ specifies the type of document that's being linked
- _rel_ specifies the relationship between HTML page and the file it's linked to. Stylesheet when linking to a CSS file
- _style_ includes CSS rules within an HTML page, usually sits inside the head of the page

- _**Selectors**_
 _universal_ applies to all elements in the document. * ()
 _type_ matches element names. h1, h2, h3, ()
 _class_ matches element that has a value that matches the one specified after the period. .note () or p.note()
 _id_ #introduction ()
 _child_ li>a ()
 _descendant_ p a ()
 _adjacent sibling_ h1+p ()
 _general sibling_ h1-p ()

 ## CSS treats HTML elements as if it appears in it's own box and uses rules to indicate how it should look
 ## Different selectors allow you to target your rules at different elements
 ## CSS rules usually appear in a seperate document but can appear within HTML

## JS Chapter 2: "Text"
- access content, modify content, program rules, react to events
- JS encompasses many of the traditional rules of programming. It can make the web page feel interactive by responding to what the user does.
- Computers approach tasks in a different way than humans, so your instructions must let the computer solve the task programmatically.

## Scripts:
- a series of instructions a computer can follow step-by-step.
- A browser may use different parts of the script depending on how the user interacts with the web page.
- Scripts can run different sections of the code in response to the situation.

## Writing A Script:
- to write a script, you need to first state your goal and then list the tasks that need to be completed in order to achieve it.
- Break down your big picture into what you want to achieve, break that down into smaller steps.
- Define the goal; once you know the goal of your script, you can work out the individual tasks needed to achieve it. The taks can be represented using a flowchart.
- Design the script; each task may be broken down into a sequence of steps. When you're ready to code the script, each step can then be translated into individual lines of code.
- Code each step

## Expressions:
- evaluates into a single value. There are two types of expression;
- expressions that just assign a value to a variable. var color = 'beige'; the value of the color is now beige.
- expressions that use two or more value to return a single value. var area = 3 * 2; the value of area is now 6.

## Operators:
- expressions rely on things called operators; they allow programmers to create a single value from one or more values.
- _Assignment operators:_ assign a value to a variable. color = 'beige';value of the color is now beige.
- _Arithmetic operators:_ perform basic math. area = 3 * 2; value of area is now 6.
- _String operators:_ combine two strings. greeting = 'Hi ' + 'Molly'; value of greeting is now Hi Molly.
- _Comparison Operators:_ compare two values and return true or false. buy = 3 > 5; value of buy is false.
- _Logical operators:_ combine expressions and return true or false. buy = (5 > 3) && (2 < 4); value of buy is now true.

## Arrays: 
- special type of variable. It stores more than one piece of related info

## Arithmetic Operators
- Addition: +
- Subrtraction: -
- Division: /
- Multiplication: *
- Increment: ++ adds one to the current number
- Decrement: -- subtracts one from the current number
- Modulus: % divides the two values and returns the remainder
- **Multiplication and division happen _before_ addition and subtraction**
- Concatenation; the process of joining two or more strings to create one new string.

## Functions
- functions let you group a series of statements together to perform a specific task. 
- When you ask it to perform its task, its known as *calling* the function
- Pieces of info passed to a function are known as _parameters_
- When you write a function and expect it to provide you an answer, the response is known as _return value_
- **Functional Declaration:** give it a name and then write the statements needed to achieve it's task inside the curly braces.
- **Calling the Function:** having declared the function, you can then execute all of the statements between it's curly braces with just one line of code.
- **Parameters:** sometimes a function needs specific info to perform its task. When you declare the function you give it this.

## JS Chapter 4: "Decisions and Loops"
- Conditional statements allow your code to decide what to do next
- Comparision operators (===, !==, ==, !=, <, >, <=, =>) compare two operators
- Logical operators allow you to combine multiple sets of comparison operators
- if...else statements run one set of code if a condition is true or false
- switch statements allow you to compare a value against possible outcomes, provides a default if none match

# Booleans:
- == is equal to
- != is not equal to 
- === strict equal to
- !== strict not equal to
- > greater than
- >= greater than or equal to
- < less than
- <= checks if the number on the left is less than or equal to the number on the right 

## Loops
- Loops check a condition. If it returns true, a code block will run. Then the condition will be checked again and if it still returns true, the code block will run again. It repeats until the condition returns false. There are three types of common loops:
- For; if you need to run code a specific # of times, use a _for_ loop. In a _for_ loop, the condition is usually a counter which is used to tell how many times the loop should run.
- While; If you do know how many times the code should run, you can use a _while_ loop. The condition can be something other than a counter to loop for as long as the condition is true.
-Do While; It will always run the statements inside the curly braces at least once, even if the condition evaluates to false.

## Logical Operators:
- Comparison operators usually return single values of true or false. Logical operators allow you to compare the results of more than one comparison operator.
- && logical and; this operator tests more than one condition. If both expressions evaluate to true than the expression returns to true. If just one of these returns false, then the expression will return false.
true && true return true
true && false return false
false && true return false
false && false return false
- | | logical or; tests at least one condition. If either expression evaluates to true, then the expression returns true. If both return false, then the expression will return false.
- ! Logical Not; this operator takes a single Boolean value and inverts it. This reverses the state of an expression. If it was false (without the ! before it) it would return true. If the statement was true, it would return false.
- Logical Expressions are evaluated left to right. If the first condition can provide enough info to get the answer, then there is no need to evaluate the second condition.
