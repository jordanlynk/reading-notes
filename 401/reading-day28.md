## MVC Forms

* In the *MVC* pattern, the view handles the apps data presentation & user interaction. Views are an embedded HTML template in Razor markup (Razor markup interacts w/ HTML markup to produce a webpage sent to the client)
* *Views* are **.cshtml** files. They help establish separation of concerns by seperating the user interface markup from other parts of the app.
    * The app is easier to maintain, as it is better organized. Views are typically grouped by app feature. 
    * Parts of the app are loosely coupled.
    * Easier to test the user interface parts of the app (views are seperate units)
* *Home* controller is represented by a Home folder that contains the views for About, Contact, Index. When a user requests one of these 3, controller actions determine which of the 3 views to utilize for building and returning a webpage back to the user.
* *Layouts* provide consistent webpage sections & reduce code repetition.
* *Partial views* reduce code duplication by utilizing reusable parts of views. 
* *View Components* allow you to reduce repetitive code but are appropriate for view content that requires code to run on the server to call up the webpage.
