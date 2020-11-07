# NODE.js

## What is Node.js?
- Node.js is a JS runtime built on Chrome's V8 JS engine- per the project's home page
- Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google's V8 JS engine and libuv library- per Stack Overflow
- Simplified: Node is built on Google Chrome's V8 JS engine
- The engine is the open-source JS engine that runs in Google Chrome and other Chrome-based web browsers. It was designed with performance in mind and is reponsible for compiling JS directly to native machine code that computers can execute.
- Node programs are not executed in a browser. The created of Node(Ryan Dahl) took the engine and enhanced it with various features, such as a file system API, an HTTP library and a number of operating-system related utility methods.
- Node.js is a program we can use to execute JS on our computers, aka a JS runtime.

## How to install Node.js
- *Node Binaries vs Version Manager*: it is suggested to use a version manager instead of grabbing node binaries for your system. Version manager allows you to install multiple versions of Node and switch between them at will. There are a number of advantages to using version manager, such as negating potential permission issues when using Node with npm and lets you set a Node version on a per-project basis.
- You can check that Node is installed on your system by opening terminal and typing "node -v". If it has gone well, you should see your version installed. Next, create your new file "hello.js" and copy in "console.log("Hello, World!"); 
- This will use *Node's built-in console module* to display a message in the terminal window. To run it, use the command *node hello.js* If configured properly, you should see "Hello, World!"
## Node.js is excellent support for Modern Javascript
- Node has excellent support for ECMAScript 2015 (ES6) and beyond. Since you are only targeting one runtime (a specific version of the V8 engine), this means that you can write your JavaScript using the latest and most modern syntax. You also generally won't have to worry about compatibility issues.
## NPM: JS Package Manager
- To check what version of npm you have run this code *npm -v*
- NPM is the package manager but is also the world's largest software registry. There are over 1,00,000 packages of JS code available for download.
- **Installing a package globally** npm install -g jshint; this will install the jshint package globally on your system. You can use it to lint the index.js file. From there you should see a number of ES6-related errors, fix them up by adding /* jshint esversion: 6 */ to the top of the index.js file, re-run the command and the linting should pass.
- **Installing a package locally** npm init -y; creates and auto-populates package.json file in the same folder. Next, use npm to install the lodash package and save it. *npm install lodash --save* 
- **Working with the package.json file**: within the test directory, you'll notice a folder "node_modules". This is where npm has saved lodash and any libraries that lodash depends on. The node_modules folder shouldn't be checked in to version control, and can be re-created at any time by running npm install from the project's root.
- If you open the package.json file, you’ll see lodash listed under the dependencies field. By specifying your project’s dependencies in this way, you allow any developer anywhere to clone your project and use npm to install whatever packages it needs to run.
## What is Node.js used for?
- It is designed to automate the process of developing modern JS application.
- They can be used for anything such as, bundling your JS files and dependencies into static assets, to running tests, or automatic code linting and style checking. 
- If you want to start developing apps with any modern JS framework, like react or angular, you'll be expected to have a working knowledge of Node and npm. You don't need a Node back end to run these frameworks but these frameworks and many related packages are all available via npm and rely on Node to create a sensible development environment in which they can run.