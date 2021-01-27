## Entity Framework Core and APIs

- DbContext = a class that coordinates EF functionality for a given data model.
- Entity Framework Core (EF) = lightweight, extensible open source and cross platform.
- It can serve as an object-relational mapper (O/RM) which will
  - Allow .net devs to work with a database using .Net objects
  - Eliminates the need for most data-access code that typically needs to be written.
- With an EF core, data access is performed using a model, made up of entity classes and a context object that represents a session with the database.
## Model Development Approaches:
  - Generate model from exisiting database
  - Hand code a model to match a database, exactly.
  - Once the model is created, use EF migrations (which allow evolving the database as the model changes) to create a database from the model.
- *Querying*: 
  - instances of entity classes are retrieved from database
- *Saving Data*: 
  - Created, deleted and modified in the database using instances of entity classes.
- *Data Seeding*:
  - The process of populating a database with an initial set of data.
- *Model Seed Data*:
  - Seeding data can be associated with an entity type as part of the model configuration.
  - Context.SaveChanges() is a straightforward and powerful way to perform data seeding.  
