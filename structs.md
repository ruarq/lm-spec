# Structs
## Declaration & initialization
```lm
# Declaring a struct "Person"
struct Person {
	let name: string;
	mut age: u8;
	mut height, weight: u16;
}

# Creating an instance of `Person`
let person: Person = {
	name: "Brian",
	age: 42,
	height: 179,
	weight: 64
};
```

## Special functions
```lm
struct Person {
	# The preceding "::" means that "new" is a static function
	fn ::new() -> Person {
		ret Person{
			name: "",
			age: 0,
			height: 0,
			weight: 0
		};
	}

	# Overload new, for example to create a "newborn", whom has the age 0
	fn ::new(name: string, mut height, weight: u16) -> Person {
		ret Person{
			name: name,
			age: 0,
			height: height,
			weight: weight
		};
	}

	let name: string;
	mut age: u8;
	mut height, weight: u16;
}

# Creating a new instance of `Person`
let person = Person::new();

# Using the overload
let person = Person::new("Brian", height: 45, weight: 3);
```
