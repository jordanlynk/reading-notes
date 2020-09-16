#CSS

- CSS allows you to create rules that control each box individually and the content within it.
- CSS works by associating rules with HTML elements. These rules control how the content of specified elements should display. CSS rule contains two parts; _selector_ which indicate the element the rule applies to. The same rule can apply to more than one if you seperate the element names with commas. _Declarations_ indicate how the elements referred to the selector should be styled. They are split into two parts, a property and a value and are seperated by a colon. 
## Declarations 
- Sit inside curly brackets and each is made up of two parts; a _property_ and a _value_ seperated by a colon. 
- **Properties:** indicate the aspects of the element you want to change
- **Values:** specify the settings you want to use for the chosen properties. EX: If you want to specify a color property then the value is the color you want the text in these elements to be.
## External CSS
- **Link:** this element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. It is an empty element, meaning it does not need a closing tag. Lives inside the head element. It has three attributes:
_href_ specifies the path to the CSS file
_type_ specifies the type of document being linked to. 
_rel_ specifies the relationship between the HTML page and the file it is linked to. 
- An HTML page can use more than one CSS style sheet. to do this, it could have <link> element for every css file it uses.
## Style
- this element should use the type attribute to indicate that the styles are specified in CSS.
- Allows all pages to use the same style rules, rather than repeating them in each page.
- Keeps the content seperate from how the page looks
- You can change the styles used across all pages by altering just one file

# Selectors:
- _Universal:_ * ()
- _Type:_ h1, h2, h3 {}
- _Class:_ .note () targets any element whose class attribute has a value of note. p.note () targets only <p> elements whose class attribute has a value of note.
- _ID:_ #introduction {}
- _Child:_ li>a {}
- _Descendant:_ p a {}
- _Adjacent Sibling:_ h1+p {}
- _General Sibling:_ h1~p {}

- _Color:_ allows you to specify the color of text inside an element.
- RGB Values: express colors in terms of how much red, green and blue are used to make it up. EX: rgb(100,100,90)
- HEX: six-digit codes that represent the amount of red, green and blue in a color preceded by a pound or hash #. EX: #ee3e80
- Color Names: there are 147 predefined color names that are recognized.

# Summary of Color:
- Not only brings your site to life, also helps convery the mood and evokes reactions
- Three ways to specify colors: RGB values, hex codes and color names
- Color pickers can help you find the color you want
- It's important to ensure there is enough contrast between any text and the background color (otherwise people will not be able to read as easily)
- CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as _RGBA_
- CSS3 allows you to specify colors as HSL values, with an optional opacity value. It is known as _HSLA_
