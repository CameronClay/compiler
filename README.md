# Compiler
Two pass compiler wtih a language similar to that of a hybrid of C and Java. Two pass compiler means the code is anyalzed twice and information from the first pass is used to do semantic checking and code generation during the second pass.

## About
During the first pass of compilation, the code is parsed against the grammer, checked for syntax errors and a symbol table is constructed which serves to enable semantic error checking in the second pass of compilation.
The goal of the second pass is to perform semantic error checking, to generate icode, and to produce target code.

## Features
- Inheritance: Single inheritance.
- Super syntax: super(class_name).
- Abstract syntax: [public|private] abstract identifier()
- Each class stores $vpointer which points to vtable for currently stored class
- VTables are stored in directives and initialized afterwards
- Supports switch statements.
- Supports cstring output.
- Supports conversion between integers and strings.

## How to run
```
compiler src [-icode] [-sym] [-lex]

[-lex]   Will output all the tokens to the console.
[-sym]   Will output the symbol table to the console.
[-icode] Will output the intermediate code to the console.
```

### Unit Testing and Integration Testing
- Unit testing and integration testing is done using Boost.Test.

### Tooling
- C++ 20
- CMake
- Boost.Test
- vcpkg

### Note
The code for this project is private but I am more than happy to show and expain the code.
