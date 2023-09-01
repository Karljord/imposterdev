---
title: "Go basic types"
date: 2023-02-10T13:32:56+01:00
draft: false
---


## Boolean
  Like many other major languages GO has the built in boolean type, which in go is represented by the keyword bool. And kan have the values true or false.

  ```go
  var myBoolean bool = true
  ```

## Numeric
  Numerics can be subdivded into three parts. Integers, floats and complex 
### Integer

```go
Unsigned

| keyword | Min. val    | Max. val   |
| ------- | ----------- | ---------- |
| uint    |             |            | // Depends on underlying system
| uint8   | 0           | 255        |
| uint16  | 0           | 65535      |
| uint32  | 0           | 4294967295 |
| uint64  | 0           | 2^64       |

Signed

| keyword | Min. val    | Max. val   |
| ------- | ----------- | ---------- |
| int     |             |            | // Depends on underlying system
| int8    | -128        | 127        |
| int16   | -32758    	| 32767      |
| int32   | -2147483648 | 2147483647 |
| int64   | -2^63       | 2^63 - 1   |

Special

| keyword | alias for |
| ------- | --------- |
| rune    | int32     |
| byte    | uint8     |
```

### Float
```go
| keyword | Val. range                                            |
| ------- | ----------------------------------------------------- |
| float32 | the set of all IEEE-754 32-bit floating-point numbers |
| float64 | the set of all IEEE-754 64-bit floating-point numbers |
```

###   Complex
```go

| keyword    | Val. range                                                           |
| ---------- | -------------------------------------------------------------------- |
| complex64  | the set of all complex numbers with float32 real and imaginary parts |
| complex128 | the set of all complex numbers with float64 real and imaginary parts |

var y complex64  = complex(1, 2)  // 1+2i
var x complex128 = complex(1, 2)  // 1+2i
```

## String
```go
var myString string = "My first string"
```