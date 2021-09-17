# Client_Server_Interface implementation

This page explains how a Client_Server_Interface is implemented in C.

## File

A Client_Server_Interface is implemented in a dedicated header file.  
The file is named : Name_Of_The_Interface.h.

## File guard

A file guard is added.  
The unique value is the name of the interface in upper case suffixed with "_H".

```C
#ifndef NAME_OF_THE_INTERFACE_H
#define NAME_OF_THE_INTERFACE_H

#endif
```

## Inclusions

The header files that implement the types used by the operations arguments of the interface are
included.

```C
/* Arguments types */
#include "Name_Of_A_Type.h"
#include "Name_Of_An_Other_Type.h"
```

## Interface

A Client_Server_Interface is implemented as structure.

```C
/* Client_Server_Interface */
typedef struct {
    
} Name_Of_The_Interface;
```

## Operations

Each operation provided by the interface is implemented as a pointer on a function which is a field
of the structure.  

```C
/* Client_Server_Interface */
typedef struct {
    void (*Name_Of_An_Operation) ( ... );
} Name_Of_The_Interface;
```

## Arguments

The arguments of the operations are passed by value for input arguments and by address for output
arguments.

```C
/* Client_Server_Interface */
typedef struct {
    void (*Name_Of_An_Operation) ( A_Type an_input_arg, ..., A_Type* an_output_arg );
} Name_Of_The_Interface;
```

## Summary

```C
#ifndef NAME_OF_THE_INTERFACE_H
#define NAME_OF_THE_INTERFACE_H

/* Arguments types */
#include "Name_Of_A_Type.h"
#include "Name_Of_An_Other_Type.h"

/* Client_Server_Interface */
typedef struct {
    void (*Name_Of_An_Operation) ( A_Type an_input_arg, ..., A_Type* an_output_arg );
} Name_Of_The_Interface;

#endif
```