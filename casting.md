# Casting
Casting in Lumin is very easy. The `$` token is used to cast values to a different type.

For example, to cast a `i16` to a `i8`, you'd have to write:
```lm
let a: i16 = 420; # not in the range of min(i8) and max(i8)
let b: i8  = a; # would produce an error, typeof(a) != typeof(b)
let b: i8  = $i8(a); # no error, a has been casted to i8
```
