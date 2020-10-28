# Read-01 Notes

## Chapter 1: "Structure:"

- _Structure:_ added to a document to make it easier to understand.
- _Elements:_ HTML code in blue is made up of characters that live inside angled brackets. Elements are usually made up of two tags, an opening and closing tag. Each HTML element tells the browser something about the info that sits between it's opening and closing tags.
- _Tags:_
- <html> tag indicates anything between it and a closing </html> tag is HTML code
- <body> </body> anything between will be shown inside the main browser window
- <h1> </h1> main heading
- <p> </p> paragraph of text
- <h2> </h2> sub-heading
- <head> </head> contains info about the page
- <title> inside the head tag

- _Attributes:_ provide additional info about the contents of an element. They appear on the opening tag of the element and are made up of two parts: a name and a value, seperated by an equals sign
- _Name:_ indicates what kind of extra info you are supplying about the element's content. Written in lowercase
- _Value:_ the info or setting for the attribute. Should be placed in double quotes. Different attributes can have differenet values.

## Summary:
- HTML pages are text documents
- HTML uses tags (characters that sit inside angled brackets) to give the info they surround special meaning.
- Tags are often referred to as elements
- Tags usually come in pairs. The opening tags denotes the start of a piece of content, the closing tags denotes the end.
- Opening tags can carry attributes, which tell us more about the content of that element.
- Attributes require a name and a value
- To learn HTML, you need to know what tags are available for you to use, what they do, and where they can go.

## Chapter 8: "Extra Markup:"

- _DOCTYPES:_ each webpage should begin with a DOCTYPE declaration to tell a browser which version of HTML the page is using
- _<!-- -->:_ if you wnat to add a comment to your code that will not be visible in the user's browser, you can add the text between these characters.
- _ID Attribute:_ used to uniquely identify that element from other elements on the page. It's value should start with a letter or an underscore. Also known as _global attribute_, because it can be used on any element.
- _Class Attribute:_ it's value should describe the class it belongs to. (Ex:) <p class="important">
- _Block Elements:_ known as elements that will always appear to start on a new line in the browser window. 
- _Inline Elements:_ known as elements that will always appear to continue on the same line as their neighbouring elements.
- _Div:_ allows you to group a set of elements together in one block-level box. You might create a <div> element to contain all of the elements for the header of your site.
- _Span:_ acts like an inline equivalent of the <div> element. 
- _<iframe:>_ is like a little window that has been cut into your page and in that window you can see another page. Within iframe;   _src_ = specifies the URL of the page to show in the future
_height_ = height of the iframe in pixels
_width_ = width of the iframe in pixels
_seamless_ = can be applied when scrollbars are not desired.

- _<Meta>:_ lives inside the <head> element and contains info about that page.
## Summary:
- Doctypes tell browsers which version of HTML you're using.
- You can add comments to your code between the <!-- and --> markers
- The id and class attributes allow you to identify particular elements
- The <div> and span elements allow you to group block-level and inline elements together.

## Chapter 17: "HTML 5 Layout":

## Headers and Footers:
- can be used for: 
- main header or footer that appears at the top or bottom of every page on the site or for an individual <article> or <section> within the page.
- _<nav>_ element used to contain the major navigational blocks on the site such as the primary site navigation.
- _<article> acts as a container for any section of a page that could stand alone and potentially be syndicated.
- _<aside>_ has 2 purposes. Used inside an article element, it should contain info that is related to the article but not essential to it's overall meaning or used outside, it acts as a container for content that is related to the entire page.
- _<section>_ groups related content together and typically each section would have it's own heading.
- _<hgroup> group together a set of one or more <h1> through <h6> elements so that they are treated as one single heading.
- <figure>_ can be used to contain any content that is referenced from the main flow of an article. Not just images.

## Chapter 18: "Process & Design":

- Every website should be designed for the target audience, therefore it is important to understand who your target audience is. 
- After you start to understand the who of your website demographic, start considering the why. While some will simply chance across your website, most will visit for a specific reason. 
- It is unlikely that you will be able to list every reason why someone visits your site but you're looking for key tasks & motivations. This info can help guide your site designs.
- What info your visitors need: what information do they need in order to achieve their goals quickly and effectively?
- _Site Map:_ creating a diagram of the pages that will be used to structure the site, it will show how these pages can be grouped. 
- _Card Sorting:_ involves placing each piece of info that a visitor might need to know on a separate piece of paper and then organizing the related info into groups in order to determine where it will go on what page.
- _Wireframes:_ a simple sketch of key info that needs to go on each page of a site. It shows the hierachy of the info and how much space it might require.
- _Visual Hierarchy:_ use contrast to create a visual hierarchy that gets across your key message and helps users find what they are looking for. Size; larger elements will grab users' attention first. Color; foreground and background color can draw attention to key messages. Style; an element may be the same size and color as surrounding content but have a different style applied to it to make it stand out.

## Summary

- It's important to understand who your target audience is, why and what info they want to find and when they are likely to return.
- Site maps allow you to plan the structure of a site.
- Wireframes allow you to organize the info that will need to go on each page
- Design is about communication. Visual hierarchy helps visitors understand what you are trying to tell them.
- You can differentiate between pieces of info using size, color and style.
- You can use grouping and similarity to help simplify the info you present.

# JS Ch. 1: "The ABC Of Programming":

- _Script:_ a series of instruction that a computer can follow to achieve a goal.
- Once you know the goal of your script, you can work out the individual **tasks** needed to achieve it. Each individual task may be broken down into a sequence of **steps**. 
- To approach writing a script, break down your goal into a series of tasks and then work out each step needed to complete that task.

- How a browser sees a web page:
1.) receive a page as HTML code
2.) create a model of the page and store it in memory
3.) use a rendering engine to show the page on screen