## How to debug for absolute beginners: 
- Clarify the problem by asking yourself the right questions. 
- An exception is an unexpected event encountered when running code, typically an error of some kind.
- Examine your assumptions: before investigating a bug or an error, think of the assumptions that made you expect a certain result.
- Step through your code in debugging mode to find where the problem occured.

## How to use the try/catch block to catch exceptions
- Place any code statements that might raise or throw an exception in a try block, and place statements used to handle the exception or exceptions in one or more catch blocks below the try block. Each catch block includes the exception type and can contain additional statements needed to handle that exception type.
- The Common Language Runtime (CLR) catches exceptions not handled by catch blocks. If an exception is caught by the CLR, one of the following results may occur depending on your CLR configuration:
- debug dialog box appears
- program stops execution and a dialog box with exception info appears
- error prints out to the standard error output stream

## Statement Keywords:
- Selection statements: if, else, switch, case
- Iteration statements: do, for, foreach, in, while
- Jump statements: break, continue, default, goto, return, yield
- Exception handling statements: throw, try-catch, try-finally, try-catch-finally
- Checked and unchecked
- fixed statement
- lock statement

## C# 7.0 pg 158-166:
- A try statement specifies a code block subject to error-handling or cleanup code. The try block must be followed by a catch block, a finally block or both. The catch block executes when an error occurs in the try block. The finally block executes after execution leaves the try block (or if present, the catch block), to perform cleanup code, whether or not an error occured. 
- A catch block has access to an Exception object that contains information about the error. You can use a catch block to either compensate for the error or rethrow the exception. You rethrow an exception if you merely want to log the problem, or if you want to rethrow a new, higher-level exeception type.
- A catch clause specifies what type of execution to catch. This must either be System.Exception or a subclass of System.Exception.

## Therac-25:
- It was a computer controlled radiation therapy machine produced by AECL in 1982. 
- It was involved in at least six accidents between 1985 and 1987, in which patients were given massive overdoses of radiation.
- These accidents highlighted the dangers of software control of safety-critical systems, and they have become a standard case study in health informatics and software engineering. - Additionally the overconfidence of the engineers and lack of proper due diligence to resolve reported software bugs are highlighted as an extreme case where the engineers' overconfidence in their initial work and failure to believe the end users' claims caused drastic repercussions.
- Several error messages merely displayed the word "MALFUNCTION" followed by a number from 1 to 64. The user manual did not explain or even address the error codes, nor give any indication that these errors could pose a threat to patient safety.
- The system distinguished between errors that halted the machine, requiring a restart, and errors which merely paused the machine (which allowed operators to continue with the same settings using a keypress). However, some errors which endangered the patient merely paused the machine, and the frequent occurrence of minor errors caused operators to become accustomed to habitually unpausing the machine.



