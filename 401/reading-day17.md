# Razor Pages:


## Why?
- File-based routing approach
- Good for simple pages that read-only or do basic data input.
- While MVC is entity & action-focused, Razor pages are more page-focused
- Easier to get web development for beginners
- Fits well to small scenarios where building controllers and models as seperate classes is overkill.
- Can seperate logic from presentation
- When making a request, the default ASP.NET routing config will attempt to locate the page requested in the "Pages" folder

## What?
- Pages are marked with "@page" that tells the view engine it is a Razor page & not a regular MVC view.
- Object-oriented
- Similiar to MVC but there are no folders for controllers/views.
- **Pages folder**: contains Razor pages & supporting files. In a pair of files:
    - .cshtml file : has HTML markup with C# code using Razor syntax
    - .cshtml.cs : has C# code that handles page events.
    - Any supporting files that begin with an underscore, configure UI elements common to all pages. 
    - When making a request, the default ASP.NET routing config will attempt to locate the page requested in the "Pages" folder
- Displaying data: add properties to your Page Model.    