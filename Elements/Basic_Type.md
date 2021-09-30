# Basic_Type implementation

This page explains how Basic_Types are implemented in C.

Each Basic_Types C is implemented using a data type defined by the C standard. These data types
are defined in C standard header files or natively handled by the language.  
The table below gives the mapping between each Basic_Type and its corresponding C data type and
eventually the required C standard header file.

Basic_Type | Header file | C type
-|-|-
boolean | stdbool.h | bool
sint8 | stdint.h | int8_t
sint16 | stdint.h | int16_t
sint32 | stdint.h | int32_t
sint64 | stdint.h | int64_t
uint8 | stdint.h | uint8_t
unit16 | stdint.h | uint16_t
uint32 | stdint.h | uint32_t
uint64 | stdint.h | uint64_t
float32 | - | float
float64 | - | double
character | - | char
characters_string | - | char*
uint8_array | stdint.h | uint8_t*