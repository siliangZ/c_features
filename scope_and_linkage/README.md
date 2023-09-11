https://www.geeksforgeeks.org/scope-rules-in-c/

# Declaration vs Definition
Declaration is a statement that introduces an identifier into the current scope. It's a statement that tells compiler about the name and type of the variable.
Definition allocates memory for the variable or function.
A variable or function could be declared many times, but defined only once.
Sometimes declaration and definition are done in one statement.

# What is Scope
It's the area under which the variable is visible.

# Global Scope
A variable declared outside all functions is said to be in global scope. The scope of the identifier starts at the beginning of the file and ends at the end of the file.

It could be accessed in different file through external linkage.

# Local Scope
It's a region inside a block or function.

1. We have name shadowing in C. It means that a variable declared in a block hides the variable of the same name declared in the outer block.

# Internal Linkage and external linkage

## Difference with Scope
Scope is a property handled by compiler, whereas linkage is a property handled by linker.

## Internal Linkage
It's implemented by keyword static. All constants are by default internally linked.

## External Linkage
It's implemented by keyword extern. We use extern to declare a variable that is defined in another file.


## How to define a variable with external linkage
1. use the header file to contain an extern declaration of the variable.
2. The header file is included in the file that defines the variable.
3. The header file is included in other files that reference the variable.