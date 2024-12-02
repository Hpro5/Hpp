Make a README
Sure! Here's a detailed README for the Ham++ programming language, outlining its features and usage:

Ham++ Programming Language
Ham++ is a simple, custom programming language designed for learning and creating basic programs. It supports boolean variables, conditional statements, loops, functions, and basic input/output operations. This README will guide you through the language's features and provide examples to get you started.

Features
Boolean Variables: Declare and manipulate boolean variables.

Conditional Statements: If and else blocks for conditional execution.

Loops: funcloop for repeated execution of code blocks.

Functions: Define and call functions.

Input/Output: Print text and boolean values.

Commands
1. Boolean Variables
Declare and set boolean variables.

Syntax:

plaintext
Bool [name] [value]
Set [Bool] 1/0
Example:

plaintext
Bool flag 1
Set flag 0
2. Conditional Statements
Use If and else blocks to conditionally execute code.

Syntax:

plaintext
If [Bool] {
    // Code to execute if Bool is true
} else {
    // Code to execute if Bool is false
}
Example:

plaintext
Bool flag 1
If flag {
    PrintStr "Flag is true"
} else {
    PrintStr "Flag is false"
}
3. Loops
Use funcloop to execute code repeatedly.

Syntax:

plaintext
funcloop [name] [loop times] {
    // Code to execute in loop
}
Example:

plaintext
funcloop loopTest 3 {
    PrintStr "This is a loop"
}
4. Functions
Define and call functions.

Syntax:

plaintext
func [name] [valuename(optional)] {
    // Function body
}
RUN [funcname] [funcvalue(optional)]
Example:

plaintext
func greet {
    PrintStr "Hello, World!"
}
RUN greet
5. Input/Output
Print text and boolean values.

Syntax:

plaintext
PrintStr "string"
Print [Bool]      // Prints '#' if true, ' ' if false
PrintLn [Bool]    // Prints '#' if true, ' ' if false, and moves to the next line if specified
Example:

plaintext
Bool flag 1
PrintStr "Initial State:"
Print flag
PrintLn flag 1
