JS DE

EXECUTION CONTEXTS
The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scop

EXECUTION CONTEXT

Every statement in a script lives in one of three execution contexts:
+  GLOBAL CONTEXT
Code that is in the script, but not in a function.
There is only one global context in any page.
+ FUNCTION CONTEXT
Code that is being run within a function.
Each function has its own function context.
+  EVAL CONTEXT (NOT SHOWN)
Text is executed like code in an internal function
called eva l {}

**VARIABLE SCOPE**
The first two execution contexts correspond with the
notion of scope (which you met on p98):
+ Q GLOBAL SCOPE
If a variable is declared outside a function, it can
be used anywhere because it has global scope.
If you do not use the var keyword when creating
a variable, it is placed in global scope.
+ FUNCTION-LEVEL SCOPE
When a variable is declared within a function,
it can only be used within that function. This is
because it has function-level scope. 

EXECUTION CONTEXT
& HOISTING
Each time a script enters a new execution context, there are two phases
of activity:
1: PREPARE
• The new scope is created
• Variables, functions, and arguments are created
• The value of the this keyword is determined 

2: EXECUTE
• Now it can assign values to variables
• Reference functions and run their code
• Execute statementS
![Scope](https://davidql.github.io/scope_talk/scope_diagram.png)


UNDERSTANDING ERRORS
![error](https://th.bing.com/th/id/OIP.-yIy3o59HMViKAveiz0C3QHaD4?w=299&h=180&c=7&o=5&dpr=1.25&pid=1.7)
If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handl ing code.

|PROPERTY|DESCRIPTION|
|-------:|----------:|
|name| Type of execution|
|message| Description|
|fileNumber| Name of the JavaScript file|
|lineNumber| Line number of error |

![error2](https://th.bing.com/th?id=OIF.0%2buNIsmKcwTsJmZpEXTQFg&w=295&h=180&c=7&o=5&dpr=1.25&pid=1.7)

|OBJECT|DESCRIPTION  |
|-------:|----------:|
|Error|Generic error - the other errorsare all based upon this error |
|Syntax Error|Syntax has not been followed  |
| Ref erenceError |Tried to reference a variable that is not declared/within scope |
|TypeError | An unexpected data type that cannot be coerced|
|Range Error | Numbers not in acceptable range |
|URI Error | encodeURI ().decodeURI(),and similar methods used incorrectly |
|EvalError | eval () function used incorrectly |

