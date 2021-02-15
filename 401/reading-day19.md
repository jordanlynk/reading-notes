## Testing and Swagger:

- When creating an identity, it may be assigned one or more claims issued by a trusted party. 
    * A claim is a name value pair that represents what the subject is, not what it can do. 
    * claims based authorization checks the value of a claim and allows access to resource based on that value. 
    * Claim based authorization checks are declarative 
    * Claims requirements are policy based, the dev must build and register a policy expressing the claims requirement. 
    * Simplest type of claim policy looks for the presence of a claim and does not check the value.
    * If you apply multiple policies to a controller or action, all policies must pass before access is granted.
    * Identity itself represents a single declaration that may have many claims associated with it. 
    * IsAuthenticated: indicates whether an identity is authenticated or not. 

- **Authentication**: the process of determining who you are 
- **Authorization**: revolves around what you are allowed to do, i.e. permissions.