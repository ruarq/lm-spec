# Attributes
```lm
# tells the compiler that `num` might be unused
@unused let num = 42;
```

You can also apply this to functions, or even types
```lm
# The result of the function `sum` might be unused
@unused_result			# the return value of the function might be unused
@unused					# the function itself might not be used
fn sum(a, b: i32) -> i32
{
	ret a + b;
}
```
