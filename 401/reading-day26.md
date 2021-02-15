# Intro into MVC

- What is it? 
  * A lightweight, highly testable presentation framework that is integrated w/ exisiting ASP.Net frameworks (master pages, authorization, etc.)
  * A design pattern that helps in developing web applications in an efficient way, compared to traditional ASP.Net web application. 
  * MVC makes the design of the app into three layers:
      * **Model**: represents the objects in our app. Also a class which has all objects and its properties/methods defined in it. 
      * **View**: has all the HTML controls which define the UI of the app. We utilize Razor Engine available with VS to help rendering the view. 
      * Views are files with .cshtml extensions (contains both html and server code)
      * Can use "@" to access C# code to access server side dynamic data.
      * **Controller**: handles the request from the user. It is responsible to handle the request and return a repsonse to user by loading appropriate view w/ data from the Model. 
      * Essentially a class with a groupo of methods called *actions*, every action method returns view. 

- In traditional .net web application approach, the user action and UI are combined, tightly coupled. In MVC, the view only deals with the UI of the page and the user actions are defined in the controller.
- MVC is *action-based architecture*: based on the action, an appropriate *View* is displayed. The code within MVC is very clean and organized.
- Page Life Cycle in MVC: this concept does not exist here. Instead, when a request is made the request will hits the *Controller*, which then hits the appropriate action. The controller then collects the required data from the model and is rendered in the appropriate *View* to user. In turn, this mean that the repsonse time is low. 
- *Testing*: In MVC, it enhances the test-driven deployment by making the UI and action logic loosely coupled. Models, Controllers and Views are all seperate layers, can be tested easily.
