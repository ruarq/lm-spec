# Operators
```lm
# aka big int
struct integer {
	fn ::new() -> integer {
		return integer {
			value: ...
		};
	}

	# create a `+` operator for the type integer.
	# imut x, y: integer = integer::new();
	# imut z = x + y;
	fn (+) (imut a, b: &integer) -> integer {
		return a.value + b.value;
	}

	mut value: ...; # imagine some representation that allows for big values, i.e. string. just imagine it.
}

Supported operators are
```lm
# arithmetic
+
+=
++

-
-=
--

*
*=

/
/=

# binary arithmetic
&
&=

|
|=

>>
>>=

<<
<<=

~
~=

^
^=

# comp
>
>=

<
<=

==
