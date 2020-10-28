# "Understanding the problem domain is the hardest part of programming"

- "Writing code is a lot like putting together a jigsaw puzzle.  We put together code with the purpose of building components that we have taken out of the “bigger picture” of the problem domain"
- "As programmers, we also are often not given complete information about the problem domain, so we don’t even have the information we need to understand it."
- "You can make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem"
- "The other choice is to become better at understanding problem domains.  As developers, we tend to think that sitting down and talking to customers or business people who know about the problem domain is a waste of time. It is easy to fall into the trap of thinking you understand enough of the problem to get started coding it.  Best to resist the temptation to “not waste anymore time talking” and make sure you understand a problem inside and out before you try and solve it with code."

# Chapter 3: "Object Literals"

- "What is an object?"
- Objects group together a set of variables and functions to create a model of something you would recognize from the real world. Variables and functions take on new names.
- *In an object: variables become known as properties*: if a variable is part of an object, it is a property. Properties tell about the object, such as name of a hotel or number of rooms.
- *In an object: functions become known as methods*: a functio that is part of an object is called a method. Methods represent tasks that are associated with the object. Ex: check how many rooms are available by subtracting the number of booked rooms from total number of rooms.
- Ex: Properties; Key; Name, Rooms, Booked, Gym, roomTypes. Value: String, Number, Number, Boolean, Array. Methods: checkAvailaility -> function


# Chapter 5: "Document Object Model"

- *"DOM"*: specifies how browsers should create a model of an HTML page & how JS can access and update the contents of a web page while it is in the browser window. 
- *The browser represents the page using a DOM tree*
- *DOM trees have four types of nodes: document, element, attribute and text.*
- *You can select element nodes by their id or class attributes, tag name or using CSS selector syntax*
- *Whenever a DOM query can return more than one node, it will always return a NodeList*
- *From an element node, you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques*
- *An element node can contain multiple text nodes and child elements that are siblings of each other*
- *In older browsers, implementation of the DOM is inconsistent, it's also a popular reason for using jQuery*
- *Browsers offer tools for viewing the DOM tree*
