```lm
mut a: i32 = 42;

match (a) {
	1..10 -> std.write("a is ${a}"),

	42 -> {
		std.write("a is the meaning of life");
		a *= 2;
	}
}
