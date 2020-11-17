## EJS Partials
- Partials come in handy when you want to reuse the same HTML across multiple views
- Partials can be thought of like functions, they make large websites easier to maintain as you won't hvae to go and change a piece of text in every page it is in. In place, you define the reusable bundle of code in a file and include it wherever you need it 
- In *EJS*, any JS or non-HTML syntax you include in your templates is always surrounded by **<% %>** delimeters
- Including a partial in EJS you use **<%- include(PARTIAL_FILE) %>** where the partial file is relative to the template you use it in.
- **NOTE** The <% %> tags allow you to output the *unescaped* content onto the page (mind the -). It is important when using the include() statement since you won't want EJS to escape your HTML characters like '<', '>', etc.
- Creating and including partials is very straightforward with EJS. 

## Intro to EJS- Partials Video
- **code: <%- include('partials/onepartial;) %>**
- *Take not of the single "-" in the code above*
- Inlcudes the particular ejs file
- Go to views, new folder = partials
- Create file within partials folder, "one-partial.ejs"
- Within ejs file type some proof of life 
- *The above steps help to use reusable text*
