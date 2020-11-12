# Functional Programming

### Concepts of Functional Programming in Javascript
- *Functional programming* is a style of building the structure and elements of computer programs, that treats computation as the evaluation of mathematical functions and avoids changing state and mutable data
- *Pure functions* has a very strict definition of purity. 
- **It returns the same result if given the same arguments** (aka deterministic); 
- An impure function would receive "radius" as the parameter, and then calculate "radius * radius * PI": This is impure because it uses a global object that was not passed as a parameter to the function. We would always pass "PI" value as a parameter to the function, so now we are just accessing parameters passed to the function. No external object
- *Reading Files* if our function reads external files, it is not pure. The file's contents can change.
- *Random number generation*: Any function that relies on a random number generator cannot be pure.
- **It does not cause any observable side effects**: examples of observable side effects include modifying a global object or a parameter passed by reference. 
- *Mutability is discouraged in functional programming*
- Pure functions are stable, consistent and predictable. Given the same parameters, pure functions will alway return the same result. 
- **Pure function benefits**: The code is easier to test, we don't have to mock anything. We can unit test pure functions with different contexts:
- Given a parameter "A" => expect the function to return value "B"
- Given a paramter "C" => expect the function to return value "D"
- A function to receive a collection of numbers and expect it to increment each element of this collection.
### Immutability: unchanging over time or unable to be changed 
- When data is *immutable*, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.
### Referential transparency: 
- A "square function" (aka pure function) will always have the same output, given the same input. Passinng 2 as a parameter of the square function will always return 4. We replace it with square(2) and now the function becomes *referentially transparent*
### Functions as first-class entities:
- The idea of functions as first-class entities is that functions are also treated as values and used as data.
- Functions as first-class entities can: refer to it from constants and variables, pass it as a parameter to other functions and return it as result from other functions.
- The idea is to treat functions as values and pass functions like data. We can then combine different functions to create new functions with new behavior.
- **Higher-order functions**: is a function that takes one or more functions as arguments or returns a function as its result. 
- **Filter**: this function expects a "true" or "false" value to determine if the element should or should not be included in the result collection. If the callback is true, the filter function will include the element in the result collection, otherwise it will not. Ex: when we have a collection of integers and we want only the even numbers.
- **Map**: the idea of map is to transform a collection by applying a function to all of its elements and building a new collection from the returned values.

# Refactoring Javascript for Performance and Readability
*Refer to link for examples on how to refactor code*
- https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec 

