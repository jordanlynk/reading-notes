# Interfaces

- Contains definitions for a group of related functionalities that a non-abstract class must implement.
- Interface cannot declare instance data such as fields, auto-implemented properties or property-like events.
- You can include behavior from multiple sources in a class. (defined by using keyword *interface*)
- *IEquatable<T>* must contain a definition for an "equals" method that matches a signature the interface specifies.
- Can contain instance methods, properties, events, indexers or a combo of those 4.
- An interface is like an abstract base class with ONLY abstract members. 
- An interface cannot be instantiated directly. Instead members are implemented by any class or struct.
- A class or struct can implement multiple interfaces.
- Interfaces allow us to specify that a particular class meets certain expectations that other classes rely on.
- **Interfaces are always implemented by more than one class**
- 