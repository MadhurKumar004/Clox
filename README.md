# Clox - A C Implementation of the Lox Programming Language

## Overview

Clox is a tree-walk interpreter that compiles Lox source code to bytecode and executes it on a stack-based virtual machine. This implementation demonstrates fundamental concepts in programming language design and implementation, including:

- **Lexical analysis** (scanning/tokenization)
- **Parsing** (recursive descent parser)
- **Bytecode compilation**
- **Virtual machine execution**
- **Memory management**
- **Hash table implementation**
- **Object system with strings**

## Features

### Language Support
- **Data Types**: Numbers (double-precision floating point), booleans, nil, strings
- **Operators**: Arithmetic (`+`, `-`, `*`, `/`), comparison (`>`, `>=`, `<`, `<=`, `==`, `!=`), logical (`!`)
- **Variables**: Global and local variable declarations and assignments
- **Control Flow**: Conditional statements, loops (planned)
- **Functions**: Function declarations and calls (planned)
- **Classes**: Object-oriented programming features (planned)

### Runtime Features
- **REPL Mode**: Interactive Read-Eval-Print Loop for testing expressions
- **File Execution**: Run Lox programs from source files
- **Error Handling**: Compile-time and runtime error reporting with line numbers
- **Memory Management**: Automatic memory allocation and deallocation
- **String Interning**: Efficient string storage and comparison

## Building and Running

### Prerequisites
- GCC or Clang compiler
- Make (optional)
- Standard C library

### Compilation
```bash
# Simple compilation
gcc -o clox *.c

# With debug information
gcc -g -o clox *.c

# With optimizations (for release)
gcc -O2 -o clox *.c
```

### Usage

#### Interactive Mode (REPL)
```bash
./clox
> print "Hello, World!";
Hello, World!


#### File Execution
./clox program.lox
#currently under work

```
## Debugging

The interpreter includes built-in debugging features controlled by preprocessor flags in `common.h`:

- `DEBUG_PRINT_CODE`: Disassembles and prints bytecode after compilation
- `DEBUG_TRACE_EXECUTION`: Shows stack state and instruction execution during runtime

## Future Enhancements

Following the "Crafting Interpreters" book progression:
- [ ] Control flow statements (if/else, while, for loops)
- [ ] Functions and closures
- [ ] Classes and inheritance
- [ ] Garbage collection
- [ ] Standard library functions

## Learning Resources

This implementation closely follows:
- **"Crafting Interpreters"** by Robert Nystrom - [craftinginterpreters.com](https://craftinginterpreters.com/)
- The book's chapter on "A Bytecode Virtual Machine" (Part III)
