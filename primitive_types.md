# Primitive types
The *default*, *primitive types* or *standard types* that Lumin supports: `u8`, `u16`, `u32`, `u64`, `i8`, `i16`, `i32`, `i64`, `f32`, `f64`, `bool`, `char`, `wchar`, `long` and `ulong`

## Unsigned integer types
### `u8`
8-bit / 1-byte unsigned integer

### `u16`
16-bit / 2-byte unsigned integer

### `u32`
32-bit / 4-byte unsigned integer

### `u64`
64-bit / 8-byte unsigned integer

## Signed integer types
### `i8`
8-bit / 1-byte signed integer

### `i16`
16-bit / 2-byte signed integer

### `i32`
32-bit / 4-byte signed integer

### `i64`
64-bit / 8-byte signed integer

## Floating point types
### `f32`
32-bit / 4-byte / *single precision* floating point
**Note**: Required to be 32-bit in width

### `f64`
64-bit / 8-byte / *double precision* floating point
**Note**: Required to be 64-bit in width

## Other types
### `bool`
Special type for `true` or `false` values that is like a `u8` but can only have the values `1` or `0` / `true` or `false`

### `char`
Alias for `u8`

### `wchar`
Alias for `u16`

### `long`
- On 32-bit systems: Alias for `i32`
- On 64-bit systems: Alias for `i64`

### `ulong`
- On 32-bit systems: Alias for `u32`
- On 64-bit systems: Alias for `u64`
