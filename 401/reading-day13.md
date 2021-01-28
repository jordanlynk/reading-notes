## Dependency Injections:

- Injects an object of a class into another class that depends on that object.
- Identify services = .Map()
- "Gives the correct service to the correct actor"
  - Controller = "Actor"
  - Dbcontext (our database) = Service
  - Dbcontext = Controller
- Makes it easy to create loosely coupled components, as we don't want to have methods that say do this, and this, also this. Cleaner code is a factor in this too.
- Allows objects to be easily swapped with replacements
- Improves overall testability
- Enables looses coupling of software components. 
- AddTransient = maps to what we are creating/calling