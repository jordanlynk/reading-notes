# Chapter 4: "Links"
- *Writing Links*: created by using <a> element. You can specify which page you want to link by using href. The value of href is the page that you want people directed towards when they click the link. 
- *Absolute URL*: stands for Uniform Resource Locator. It starts with the domain name for the site and can be followed by the path to the specific page, if there is no page to go to it will display the homepage.
- *Relative URL*: essentially the shorthand version of absolute URLs, as you do not need to specify the domain name. These are helpful when you want to create links between pages without having to set up a domain name or hosting
- *Relative Link Types*: 
- *Same Folder*: links a file in the same folder, just use file name. 
- *Child Folder*: use the name of child folder, forward slash and the file name.
- *Grandchild Folder*: use the child folder name, forward slash, then the name of the grandchild folder, another forward slash and the file name.
- *Parent Folder*: use ../ to show the folder above the current one, then the file name.
- *Grandparent Folder*: repeat ../ so that you may go up two folders instead of one, then the file name.
- *Email Links*: *mailto* to create a link that starts up the user's email program and addresses in email to specific email, place mailto in front of href followed by the email address you would like it to be sent to.
- *Target*: use this tag to open a link in a new window. Placed on the opening a tag, the attribute should be _blank.
- **Links use <a>**
- **The a element uses href to indicate the page you're searching for**
- **When linking pages within your own site, use relative links rather than qualified URLs**

# Chapter 15: "Layout"
- *position-static*: this is typically default within how browsers treat HTML elements, keeps it the same.
- *position:relative*: moves element in relation to normal flow. to move the box up or down, use top or bottom properties. to move the box horizontally, ues left or right properties. Values of box offset properties usually are given in pixels, percentages or erms.
- *position-absolute*: the box is taken out of normal flow and no longer affects the position of other elements on page. Specifies where the element should appear in relation to it's containing element.
- *position-fixed*: absolute positioning that requires the position property to have a value of fixed. When the user scrolls on the page, it stays in the exact same spot.
- *z-index*: controls which element sits on top
- *float*: places the element as far to the left or right of the containing element as possible.
- *clear*: says that no element should touch the left or right hand sides of box, it can take left, right, both and none as values.
- *Multi-Column Layouts W/ Floats*: width, float positions the columns next to one another and margin creates a gap between columns.
- *Fixed Width Layout*: to create this, width of main boxes on a page will usually be specified in pixels.
- *Liquid Layout*: uses percentages to specify the width of each box so the design will stretch and fit the size of the screen.
- **div elements are used as containing elements to group sections of a page**
- **browsers will display pages normally unless you specify relative, absolute or fixed positioning**
- **float property moves content to the left or right and can create multi-column layouts**
- **pages can be fixed width or liquid layouts**
- **keep pages between 960-1000 pixels wide**
- **you can include multiple CSS files in one page**

# Chapter 3: "Functions, Methods and Objects"
- *Functions* let you group a series of statements together to perform a specific task. If multiple parts repeat the same task, you can reuse the function.
- *Declaring* you give it a name and then write the statements needed to achieve said task inside curly braces.
- *Calling* to run the code in the function, use the function name followed by parantheses.

# Article: "6 Reasons for Pair Programming":
- pair programming commonly has two roles: the Driver and Navigation
- *The Driver*: the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. *The Navigator* uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.
- *Pair programming* four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves.
- Pair programming might take a little longer but produces better results. Having someone there to talk through code with at the beginning is a better foundation and helps to catch mistakes at the beginning. It also helps to enhance technical skills, team communication, and enjoyability of coding in the workplace.
- When two programmers focus on the same code, it helps to keep you on track and asking the right questions. It provides a level of accountability that working alone does not. It also helps you to ask for help when you're stuck, instead of just working on one thing for an ungodly amount of time.
- Learning from fellow students can be useful as there are a lot of different skill sets out there. You might learn how to do something a different way than what you already know or don't know at all. By gaining knowledge from others with more, you then have the ability to pass that along down the road. Thus, keeping the knowledge train rolling.
- When working with someone with a different skill set than you during pair programming, it can help you to rely heavily on communication. Even if it is outside your comfort zone, it helps to set you up for future success in that department.
- Pair programming strengthens the ability to work with and learn from others. Communication skills are as, if not more important to a company than specific technical skills. While working in pair programming it helps you to be ready when you have to do interviews for companies and be able to talk and understand what you're reading/talking about.
- A lot of companies utilize pair programming with new hires as it helps them ready working and relying on teamwork. Through code fellows, we are working towards that and will have a solid foundation built by the end.
