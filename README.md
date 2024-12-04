write a new README
Sure! Here's a detailed README for the Ham++ programming language, outlining its features, usage, and example scripts. This README will guide users through the language and its commands.

Ham++ Programming Language
Welcome to Ham++, a simple, custom programming language designed for learning and creating basic programs. With support for boolean variables, conditional statements, loops, functions, color manipulation, and basic input/output operations, Ham++ is ideal for both beginners and experienced programmers looking to explore a new language.

Features
Boolean Variables: Declare and manipulate boolean variables.

Conditional Statements: If and else blocks for conditional execution.

Loops: funcloop for repeated execution of code blocks.

Functions: Define and call functions.

Color Manipulation: Change the print color using RGB values.

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
5. Color Manipulation
Change the print color using RGB values.

Syntax:

plaintext
Color [r] [g] [b]
Example:

plaintext
Color 255 0 0
PrintStr "This text is red"
Color 0 255 0
PrintStr "This text is green"
Color 0 0 255
PrintStr "This text is blue"
6. Input/Output
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
Example Program
Here's a simple example of a Ham++ program that demonstrates various features of the language:

plaintext
Bool pos00 1
Bool pos01 0
Bool pos02 0
Bool pos03 0
Bool pos04 0

func printGrid {
    Print pos00
    Print pos01
    Print pos02
    Print pos03
    PrintLn pos04 1
}

If pos00 {
    PrintStr "Starting the grid:"
    RUN printGrid
} else {
    PrintStr "Grid is empty"
}

funcloop loopTest 3 {
    Switch pos00
    PrintStr "Inside Loop:"
    RUN printGrid
}
Running Your Program
To run a Ham++ program, save your code in a text file (e.g., program.ham) and use the interpreter to execute it.

plaintext
Run program.ham
