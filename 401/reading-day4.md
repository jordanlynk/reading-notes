# Classes 
- A specific type that is defined as a class is a *reference type*. During your run time, you declare a variable of a reference type, the variable contains the value "null" until you create an instance of said class by using the new operator or assign it an object of a compatible type.
- When an object is created, enough memory is allocated on the managed heap for that specific object, the variable holds only a reference to the location of this object.
## Declaring Classes
- Declared by using "class" keyword, with a unique identifier.
## Creating Objects
- A class defines an object but is not an object itself. It is a entity based on a class. "Instance of a class"
- Create an object w/ "new" keyword. 
## Class inheritance 
- inheritance is a fundamental charactersitic of object-orientated programming. 
- Inheritance is accomplished by using a derivation, which means a class is declared by using a base class from which it inherits data and behavior.
# Constructors
- Whenever you create a class a constructor is called. A class or "struct" may have multiple constructors that take in different arguments. Constructors allow programmers to set default values, limit instantiation, and write code that is flexible and easy to read. 
## Parameterless constructors 
- If you don't create a constructor for your class, C# creates one by default that will instantiate the object and set member variables to default values. 
- Syntax: a constructor is a method whose name is the same as the name of its type. Method signature includes method name and parameter list; no return type. 
## Static constructors
- Creates and activates static members of said type. These are parameterless. 
# Properties
- A property is also known as a member who provides flexible ways to read, write or compute the value of a private field. Properties can be utilized as if they are public data members, they are actually known as special methods called *accessors*. They allow data to be accessed easily and still help promote the safety and flexibilty of methods.
- Enable a class to get and set values, while hiding verification code.
- Get -> gets the value
- Set -> sends the value
- Properties can be read-write (they have both a get and a set accessor), read-only (they have a get accessor but no set accessor), or write-only (they have a set accessor, but no get accessor).
# Heap(ing) 
- Heap Vs Stack : stack is memory references vs heap which is a "blob" of memory. (arrays, objects, classes)
# Garbage Collection:
- automatic memory manager. collects the allocation and release of memory for a specific application. 
- **Benefits**: frees developers from manually releasing memory. Allocates objects on managed heap efficiently. Reclaims objects that are no longer used, clears their memory and keeps that newly cleared memory available for future allocations. Provides memory safety by ensuring an object cannot use the content from another object.

