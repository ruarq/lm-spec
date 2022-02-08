# References
Lumin supports references, also known as *pointers* in languages like C or C++.

## Usage
```lm
mut a = 5;
imut x = &a; # x is a immutable reference to mutable data a, but is not allowed to mutate the data stored in a
imut y = &mut a; # y is a immutable reference to mutable data a, and is allowed to mutate the data stored in a
```

You could also explictly declare them with types:
- `a` is of type `i32`
- `x` is of type `&i32`
- `y` is of type `&mut i32`

### *"Immutable reference"*
That reference is immutable simply means that it can't be changed what it's referring to.
In C or C++, `imut y = &mut a` would be equivalent to `int *const y = &a`, while `imut x = &a` would be equivalent to `const int *const x = &a`
