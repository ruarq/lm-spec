# Variants
Like a union in C or C++, but tagged.

```lm
# Define a variant `Value`
variant Value {
	i64,
	f64,
	string
}

# Assign integer to value
# the tag of value will be i64
mut value: Value = 42;

# match against value
# and do different things depending on the tag
# replace '?' with what you'd like to do
match (typeof(value)) {
	i64 => ?,
	f64 => ?,
	string => ?
}

io::write("{value}\n"); # 42
value = "abc"; # tag changed to string
io::write("{value}\n"); # abc
```
