# OOP Principles

## Inheritance: 
- This is one of the three primary characteristics of object-orientated programming. Inheritance allows you to create new classes that reuse, extend and modify the behavior defined in other classes. 
- A *derived* class is a specialization of the base class. Ex: (you might have a base class of "animal" and a derived class named "mammal" and "reptile".)
- A *virtual* base class can override the method with its own implementation. 

## Abstract & Sealed Classes & Class Members:
- *Abstract*: enables you to create classes and class members that are incomplete & must be called upon in a derived class.
- *Sealed* (place sealed keyword before the class definition) enables you to prevent the inheritance of a class or certain class members that were previously "virtual". It cannot be used as a base class and therefore cannot be an abstract class. They prevent derivation.
- An *abstract* class cannot be instantiated. Their purpose is to provide a common definition base class that multiples derived classes can share. Ex: a class library may define an abstract class that is used as a parametere to many of its functions. Abstract classes may also define *abstract methods* (do so by adding abstract before the return type).
- If a *virtual* method is declared *abstract*, it is still virtual to any class inheriting from the abstract class. Virtual methods allow you to work with groups of related objects in a uniform way. 
## Polymorphism: 
- "many-shaped" and two distinct aspects: 
- At run time, objects of a derived class may be treated as objects of a base class in places such as method parameters & collections/arrays.
- Base classes may define and implement virtual methods and derived classes can override them, which means they provide their own definition and implementation. 
## Object-Oriented Programming (C#): 
- 4 techniques used in oop:
- **Abstraction** hiding the unnecessary details from type consumers
- **Encapsulation** a group of related properties, methods and other members are treated as a single object.
- **Inheritance** the ability to create new classes based on a exisiting class.
- **Polymorphism**: you can have multiple classes that can be used interchangeably, even though each class implements the same properites/methods in different ways.
