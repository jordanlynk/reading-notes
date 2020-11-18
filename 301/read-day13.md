## Sending Form Data
- The <form> element defines how the data will be sent. All of its attributes are designed to let you configure the request to be sent when a user hits a submit button. The two most important attributes are action and method.
- The action attribute defines where the data gets sent. Its value must be a valid relative or absolute URL. If this attribute isn't provided, the data will be sent to the URL of the page containing the form — the current page.
- example absolute url: <form action="https://example.com">
- example relative url: <form action="/somewhere_else">
- Names and values of the non-file form controls are sent to the server as name=value pairs joined w/ ampersands.
- *Action* value should be a file on the server that can handle the incoming data, including ensuring server-side validation. The server will then respond, generally handling the data and loading the URL defined by the action attribute, causing a new page load (or a refresh of the existing page, if said *action* points to the same page)
- *Method* attribute defines how data is sent. The HTTP protocol provides several ways to perform a request; HTML form data can be transmitted via a number of different methods, the most common being the GET method and the POST method
- *GET* method is the method used by the browser to ask the server to send back a given resource: "Hey server, I want to get this resource." In this case, the browser sends an empty body. Because the body is empty, if a form is sent using this method the data sent to the server is appended to the URL.
- *POST* method is the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request: "Hey server, take a look at this data and send me back an appropriate result." If a form is sent using this method, the data is appended to the body of the HTTP request.
- HTTP requests are never displayed to the user.
- If you need to send a password (or any other sensitive piece of data), never use the GET method or you risk displaying it in the URL bar, which would be very insecure.
- If you need to send a large amount of data, the POST method is preferred because some browsers limit the sizes of URLs. In addition, many servers limit the length of URLs they accept.
## Retrieving the data
- Whichever HTTP you choose, the server receives a string that will be parsed in order to get data as a list of key/value pairs. The way you access said list is dependent on the dev platform you use and on any specific frameworks you're using it with.
- *PHP* offers some global objects to access the data. Assuming you've used the POST method, the following example just takes the data and displays it to the user. Of course, what you do with the data is up to you. You might display it, store it into a database, send it by email, or process it in some other way.
## Sending Files
- Files are binary data or considered as such, whereas all other data is text data. Because HTTP is a text protocol, there are special requirements for handling binary data.
- *Enctype Attribute*: This attribute lets you specify the value of the Content-Type HTTP header included in the request generated when the form is submitted. This header is very important because it tells the server what kind of data is being sent.
- If you want to send files:
- Set the method attribute to POST because file content can't be put inside URL parameters.
- Set the value of enctype to multipart/form-data because the data will be split into multiple parts, one for each file plus one for the text data included in the form body (if text is also entered into the form).
- Include one or more <input type="file"> controls to allow your users to select the file(s) that will be uploaded.