# Data Transfer Objects

- Used as a container to encapsulate data and pass it between layers of the application. Ex: data passed between the service layer back to the presentation layer.
- Biggest advantage of DTOs: decoupling clients from internal data structures
- By using DTOs, you can only return data requested.

- **Some reasons for wanting to change the shape of data**:
 - Remove circular references 
 - Hide particular properties that clients shouldn't see
 - Omit some properties to reduce payload size
 - Avoid "over-posting" vulnerabilities
 
- To accomplish any of this, we can use DTO (or data transfer object). It defines how the data will be sent over the network. 
- Creating a class like "BookDetailDTO" includes all properties from the model, except the name string that holds a name. The BookDto class contains a subset of properties from this class. 
- We then replace the two "GET" methods in the controller class, with versions that now return the DTO. Use the linq "SELECT" statement to convert book properties into DTOs.
- Lastly, modify the "post" method to return a DTO.