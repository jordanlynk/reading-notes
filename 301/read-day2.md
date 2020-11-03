# jQuery, Events and The DOM

## JavaScript & jQuery Book:
## Pages 293-301:
- jQuery: is a simple way to achieve a variety of common JS tasks quickly and consistently, across all major browsers and without any fallback code needed.
- It is a JS file that you include in your web pages. It lets you find elements using CSS-style selectors and then do something with the elements using jQuery methods.
- jQuery object has many methods that you can utilize to work w/ the elements you select. The methods represent tasks that you commonly need to perform w/ elements.
- Why use it? *Simple Selectors*, *Common Tasks In Less Code*, *Cross-Browser Compatibility*
## Pages 306-331:
- jQuery objects store references to elements. When a selection is created with jQuery, it stores a reference to the corresonding nodes in the DOM tree. It will not create copies of them. 
- *Caching jQuery selections in variables*: a jQuery object stores references to elements. Caching a jQuery object stores a reference to it in a variable. 
- *Looping*: within jQuery, when a selector returns multiple elements, you can update all of them using the one method. There is no longer use for a loop. 
- *Chaining*: if you want to use more than one jQuery method on the same selection of elements, you can list several methods at a time using dot notation to seperate each one. The process of placing several methods within the same selector is referred to as "chaining".
- *Checking A page is ready to work with*: jQuery's .ready() method checks that the page is ready for your code to work with. 
- *THE load EVENT*: the .load() method should be used when your script relies on assets to have loaded, aka if it needs to know the dimensions of an image.
- *THE .ready() method*: checks if the browser supports the DOMContentLoaded event. If this event is supported, jQuery will create an event listener that responds to that event. The event is only supported in modern browsers.
- *Placing scripts before the closing body tag*: if you place your script at the bottom of the page, before the closing body tag the HTML will load into DOM before script runs.
- *Getting element content*: the .html() and .text() methods both retrieve and update the content of elements. *.html()*: this method will only retrieve the HTML inside the first element in the matched set, along with any of its descendants. *.text()*: it returns the content from every element in the jQuery selection, along with the text from any descendants.
- *Updating Elements*: 
- *.html(): this method gives every element in the matched set the same new content.
- *.replaceWith()*: replaces every element in a matched set with new content. Also returns the replaced elements.
- *.text()*: gives every element in the matched set the same new text content. Any markup would be shown as text.
- *.remove()*: removes all elements in the matched set.
- *Changing Content*: when updating the content of an element, you can use a string, a variable, or a function.
- *Inserting Elements*: involves two steps. 
- 1.) Create new elements in a jQuery object
- 2.) Use a method to insert content into the page
- *Getting and Setting Attribute Values*: 
- *.attr()*: can get or set a specified attribute and its value. To get the value of an attribute, you specify the name of the attribute within parenthesis.
- *.removeAttr()*: removes a specified attribute and its value. Specify the name of the attribute you want to remove from the element in parenthesis.
- *.addClass()*: adds a new value to the existing value of the class attribute.
- *.removeClass()*: removes a value from the class attribute, leaving any other class names within that attribute object.
## Pages 354-357:
- *Ways to include jQuery in your page*: In addition to hosting the jQuery file with the rest of your website, you can also use a version that is hosted by other companies. You should still have a fallback version. 
- *Loading jQuery from a CDN*: protocol relative url; When loaded from a cdn, you will often see syntax that starts with script. This will try to load jQuery from the CDN. 
- *Where to place your scripts*: the position of this element will affect how quickly a web page is loaded. Traditionally it used to be at the top of the page but now is typically placed towards the bottom right before your closing body tag.
## Article: "6 Reasons for Pair Programming":
- pair programming commonly has two roles: the Driver and Navigation
- *The Driver*: the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. *The Navigator* uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.
- Pair programming four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves.
- Pair programming might take a little longer but produces better results. Having someone there to talk through code with at the beginning is a better foundation and helps to catch mistakes at the beginning. It also helps to enhance technical skills, team communication, and enjoyability of coding in the workplace.
- When two programmers focus on the same code, it helps to keep you on track and asking the right questions. It provides a level of accountability that working alone does not. It also helps you to ask for help when you're stuck, instead of just working on one thing for an ungodly amount of time.
- Learning from fellow students can be useful as there are a lot of different skill sets out there. You might learn how to do something a different way than what you already know or don't know at all. By gaining knowledge from others with more, you then have the ability to pass that along down the road. Thus, keeping the knowledge train rolling.
- When working with someone with a different skill set than you during pair programming, it can help you to rely heavily on communication. Even if it is outside your comfort zone, it helps to set you up for future success in that department.
- Pair programming strengthens the ability to work with and learn from others. Communication skills are as, if not more important to a company than specific technical skills. While working in pair programming it helps you to be ready when you have to do interviews for companies and be able to talk and understand what you're reading/talking about.
- A lot of companies utilize pair programming with new hires as it helps them ready working and relying on teamwork. Through code fellows, we are working towards that and will have a solid foundation built by the end.