# Collections:

- **Enumeration(Enums)**: provides an efficient way to help us normalize our data. The choices feel binary and definition varies based on context throughout C#. Defined by using *enum* keyword and then the specified names of the enum members. Default constant values are type of **int**; start with 0 and increase by one following the definition text order.
- Methods cannot be defined inside the definition of enumeration type. Adding functionality to an enumeration type is done by extension method. It can be used to represent a choice from a set of mutually exlcusive values or combo of choices. 
- **Conversions**: *cast* an enum value to its underlying type and the result is the associated value of an enum number. 
- **Collections** allow for a more flexible way to work with a group(s) of objects. Different from arrays, group of objects you work with can grow and shrink as the app changes. It is a class, so you MUST declare an instance of it class before any elements may be added to the collection.
- *For* may be used in place of a *foreach* to iterate through a collection and access the collection elements by their index position, rather than the "name". Index start at 0 and ends at the element count - 1. 
