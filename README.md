# Ham++ Programming Language

Welcome to **Ham++**, a simple, custom programming language designed for learning and creating basic programs. With support for boolean variables, conditional statements, loops, functions, color manipulation, and basic input/output operations, Ham++ is ideal for both beginners and experienced programmers looking to explore a new language.

## Features
- **Boolean Variables**: Declare and manipulate boolean variables.
- **Conditional Statements**: `If` and `else` blocks for conditional execution.
- **Loops**: `funcloop` for repeated execution of code blocks.
- **Functions**: Define and call functions.
- **Color Manipulation**: Change the print color using RGB values.
- **Input/Output**: Print text and boolean values.

## Commands

### Boolean Variables
Declare and set boolean variables.

**Syntax**:
```plaintext
Bool [name] [value]
Set [Bool] 1/0
```
### Conditional Statements
Use If and else blocks to conditionally execute code.

**Syntax**:

```plaintext
If [Bool] {
    // Code to execute if Bool is true
} else {
    // Code to execute if Bool is false
}
```
### Loops
Use funcloop to execute code repeatedly.

**Syntax**:

```plaintext
funcloop [name] [loop times] {
    // Code to execute in loop
}
Functions
Define and call functions.
```
**Syntax**:

```plaintext
func [name] [valuename(optional)] {
    // Function body
}
RUN [funcname] [funcvalue(optional)]
Color Manipulation
Change the print color using RGB values.
```
### Color
**Syntax**:

```plaintext
Color [r] [g] [b]
Input/Output
Print text and boolean values.
```
### Print and PrintStr
**Syntax**:

```plaintext
PrintStr "string"
Print [Bool]      // Prints '#' if true, ' ' if false
PrintLn [Bool]    // Prints '#' if true, ' ' if false, and moves to the next line if specified
Running Your Program
```
