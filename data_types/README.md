# Into
C supports a lot of data types. The type of the variables determines the amount of storage space required and how the bit pattern stored is interpreted. The types can be divided into four categories:

# Basic Types
They are arithmetic types and are further classified into integer types and float-point types.
## Integer Types
* char
* signed char
* unsigned char
* int
* unsigned int
* short
* unsigned short
* long
* unsigned long

## Floating-point Types
* float(4 bytes)
* double(8 bytes)
* long double(10 bytes)

## Use case
It's recommended to use the fixed-width integer types from `stdint.h` header file in the standard library. Because the size of the integer types may vary from one machine to another according to the compiler. It may cause the portability issues.

# Enumerated Types
They are used to define variables that can only assign certain discrete integer values throughout the program.
Enum has following properties:
1. Two enum variants could have the same value
2. If we could assign values explicitly, the compiler assigns values starting from 0 and increments by 1 for each variant.
3. All unassigned variants are assigned the value of the previous variant plus 1.
4. The value must be integer.
5. Enum variants must be unique in their scope. So it's recommended to use the enum name as a prefix for the variants.

## Enum vs Macro
* Enum is not type safe by default. They are integers. We could use struct to wrap them around to make them type safe.
* Enum follow scope rules

# The Void Type
It indicates there is no value available. There are three different use scenarios:
* Function returns as a void
* Function arguments as a void
* Pointers to void

# Derived Types
They are divided into the following types:

## Pointer Types
## Array Types
## Structure Types
## Union Types
## Function Types