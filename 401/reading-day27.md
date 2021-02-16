## Cookies 

* Stores bits of inofrmation "locally" (on the browser)
* These are not permanent 
* Tracks movements in the website 
* Transfers data to tailor your experience 
* Client aways "sends" cookies (request)
* Server can "set" a cookie (reponse)

* When an identity is created, it can be assigned one or more claims issued by a trusted party. A claim is a name "value pair" that represents WHAT the subject is, not what it can do. 
* Claims based authorization checks the value of a claim and allows access to resource based on that value.
    * they are declarative. The dev creates them in their code, against a controller or an action wihin a controller, specifying claims which the user must posses. 
    * Claim requirements are policy based, dev must build and register a policy expressing the claims requirement. 
    * The simplest type of claim policy looks for presence of a claim and not the value. 
 * The **AuthorizeAttribute** attribute can be applied to an entire controller, in this instance only identities matching the policy will be allowed access to any Action on the controller.   
    * When utilizing this attribute, if you want to allow anonymous access to certain actions apply **AllowAnonymousAttribute** attribute.
* *Authentication* deals with WHO you are, while *Authorization* deals with WHAT you are allowed to do.
