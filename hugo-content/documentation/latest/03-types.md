## Type

The types in those examples may not be part of the final language. They are still defined there to understand the different concept of the language.

### Basic Types

`void` special type, which basically means 'no type'.

### Integer Types

`byte8`, byte of 8 bits.

`i8`, `i16`, `i32`, `i64`, `i128`, signed integers respectively of 8, 16, 32, 64 byte.

### Signed Integer Types

`u8`, `u16`, `u32`, `u64`, `u128`, unsigned integers counterparts of the above.

### Floating-point Types

`f16`, `f32`, `f64`, floating points respectively of 16, 32, 64 byte.

No complex types for now.
No imaginary types for now.

### Struct Type

Struct type are composite types (type made from other types).

```wood
Point : struct { x: i32; y: i32 }
Segment : struct {a: Point; b: Point }

p : Point.{0, 1} // Construct a point

print(p.x);   // Print element 'x' of the Point p
print(p.y);   // Print element 'y' of the Point p
print(p[0]);  // Print first element of the Point p
print(p[1]);  // Print second element of the Point p
```

#### Anonymous Struct

Anonymous struct members are injected into the enclosing type.

```wood
.{ x: i32; y: i32 };

print(x);
print(y);
```

### Array Type

> NOTE:\
Maybe `arr(T)` ?

### Array View Type

> NOTE:\
Maybe `arrv(T)` ?

An array view is basically a "reference" to contiguous space of memory.
It could be represented with a pointer to the address of the first element and a length.

### Pointer Type

> NOTE:\
Maybe `ptr(T)` ?

### Multi Dimensional Array and Array View

> NOTE:\
Maybe `mdarr(T,1,2,3)` ?
Maybe `mdarrv(T,1,2,3)` ?