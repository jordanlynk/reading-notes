## Routing

- Routing always invokes service methods
    - (ex) _course(which would be the service)
    - a "request flow"
- Get/Api/"" -> Sees the request, handles the request, does the work, then service request (output)

- 1.) MVC: Which controller
- 2.) Controller
    - Annotation [Http Get]
    - Run *that* method
3.) Service (repository) (DBContext Model)
    - implements the interface
    - Method
        - Context to hit the database
        - Return the data back to the method
4.) THEN output the data
- **FirstorDefaultAsync**: "go find this thing"
- **MapGet**: used to define an endpoint
- 
