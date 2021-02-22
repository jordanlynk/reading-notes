# Razor Pages

- Razor pages can make code page-focused scenarios easier and more productive that using controllers and views.
- Designed to make common patterns used w/ web browsers easy to implement when building an app.
- Enabled within the Startup.cs
- The **@page** directive makes the file an MVC action, meaning it handles requests directly without going through a controller. 
  - Must be the first Razor directe on a page, as it affects the behavior of other Razor constructs.
- The **PageModel** class allows seperation of the logic of a page from its presentation. Defines page handlers for requests sent to the page and data used to render the page. 
   - this type of seperation allows for managing page dependencies through *dependency injection* and unit testing the pages
- **OnPostAsync** handler method, runs the "POST" requests. Flow:
- If no errors, save the data and redirect OR
- If there are errors, show the page again with validation messages. 
- Most common handlers: 
    - OnGet: initialize state needed for the page
    - OnPost: handle form submissions
