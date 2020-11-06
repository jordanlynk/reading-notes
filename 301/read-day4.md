# How Heroku Works

## Defining an application:
- An application is a collection of source code written in one of these languages, perhaps a framework, and some dependency description that instructs a build system as to which additional dependencies are needed in order to build and run the application.
- The source code for your application, together with the dependency file, should provide enough information for the Heroku platform to build your application, to produce something that can be executed.
## Knowing what to execute:
- You don't need to make many changes to an application in order to run it on Heroku. One requirement is informing the platform which parts of your app are runnable.
- If you’re using some established framework, Heroku can figure it out. For other applications, you may need to explicitly declare what can be executed. You do this in a text file that accompanies your source code - *a Procfile.* Each line declares a *process type*, a named command that can be executed against your built application.
- The earlier definition of an application can now be refined to include this single additional Procfile.
- Heroku is a polyglot platform – it lets you build, run and scale applications in a similar manner across all the languages – utilizing the dependencies and Procfile. The Procfile exposes an architectural aspect of your application (in the above example there are two entry points to the application) and this architecture lets you, for example, scale each part independently.
## Deploying applications:
- Heroku platform uses Git as the primary means for deploying applications (there are other ways to transport your source code to Heroku, including via an API).
- When you create an application on Heroku, it associates a new Git remote, typically named heroku, with the local Git repository for your application.
- As a result, deploying code is just the familiar git push, but to the heroku remote instead:
*git push heroku main*
## Building applications:
- When the Heroku platform receives the application source, it initiates a build of the source application. The build mechanism is typically language specific, but follows the same pattern, typically retrieving the specified dependencies, and creating any necessary assets (whether as simple as processing style sheets or as complex as compiling code)


## Article for reference:
- https://devcenter.heroku.com/articles/how-heroku-works 
- https://devcenter.heroku.com/categories/nodejs-support
- https://devcenter.heroku.com/articles/deploying-nodejs 