## JWT Tokens and Claims - Intro to Identity

- Identity is a membership system that adds login functionality to .net core applications.
    - can be configured using a SQL Server database to store user names, passwords and profile data. (alternative, Azure Table Storage)
- Identity has three classes which represent the identity of a user: Claim, ClaimsIdentity, ClaimsPrincipal
- *Claims*: represents a single fact about the user. (ex: first/last name, age, employer, dob, etc). A single claim holds a single piece of info. First name = one claim, last name = one claim
    - Most common constructor accepts two strings: *type*(name of claim) and *value*(info the claim is representing about the user). 
- *Identity*: represents a form of idenification (a single way of proving who you are). ClaimsIdentity represents a single form of digital identification.
    - A single instance of ClaimsIdentity can be authenticated or not authenticated.
        - can contain numerous claims about a user.
- *ClaimsPrincipal*: represents a user and contains one or more instances of ClaimsIdentity, which represents a single form of identification & contains one or more instances of claim.
- Verbs: 
    - Authenticate: get the user's info if any exists
    - Challenge: requests authentication by the user
    - SignIn: persists the users info somewhere
    - SignOut: Removes the users persisted info
    - Forbid: denies access to a resource for unauthenticated users or authenticated but unauthorized users.