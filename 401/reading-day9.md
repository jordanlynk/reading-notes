# LINQ (Language Integrated Query)

## Imperative vs Declarative
- Imperative: can be used as a Foreach loop
- Declarative: can be used as a LINQ statement.
- A query is an expression that will transform sequences with query operators. 
- Standard query operators are implemented by the extensions methods, call "Where" onto names
- *Three distinct actions in query operations*:
- Obtain the data source 
- Create the query - question in the form of a statement
- Execute query - "then, use the data"
- **Deferred Execution**: query var that holds the query command won't execute until it is iterated over. (foreach loop). The var does not hold the result and instead just the command. It can be iterated over and over, with possible difference in the answers.
