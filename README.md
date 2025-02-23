# Introduction to X86 Assembly Language

## 1. Variables

The X86 assembler defines different intrinsic data types, each describing a set of values that can be assigned to variables and expressions of the given type. The following table lists these data types:

| Type    | Usage               |
|---------|---------------------|
| Byte    | 8 bits              |
| Sbyte   | 8 bits (signed)     |
| Word    | 16 bits             |
| Sword   | 16 bits (signed)    |
| Dword   | 32 bits             |
| Sdword  | 32 bits (signed)    |
| Real4   | 32-bit real         |
| Real8   | 64-bit real         |
| Real10  | 80-bit real         |

## 2. DUP

You can create arrays of bytes, words, double words, etc., either by using multiple initializers explicitly or by using the DUP (Duplicate) operator. Multiple initializers are separated by commas and are used to initialize each element of the array with an explicit number.

## 3. Data-related Operators

- **TYPE**: Size (in bytes) of each element in an array.
- **LENGTHOF**: Number of elements in an array.
- **SIZEOF**: Number of bytes used by an array initializer.
- **OFFSET**: Virtual address of a variable.

## Exercises

### Exercise 1

Write an assembly program that performs the following operation:

\[ R = -X + (Y - Z) \]

### Exercise 2

Implement the following operations in assembly:

1. \[ [0200] = [0100] + 24h \]
2. \[ [0200] = [0100] - 9ch \]
3. \[ [0300] = [[0100] AND [0200]] OR 68h \]
4. \[ [0300] = [[0100] * [0200]] / 68h \]
5. \[ [0300] = [29h * [0100]] / [[0200h] * 27h] \]
