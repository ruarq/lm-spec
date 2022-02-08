# Structs
## Declaration & initialization
```lm
# Declaring a struct "Person"
struct Person {
	imut name: string;			# the name of a person normally doesn't change
	mut age: u8;				# the age of a person changes, and usually won't be more than what a byte can store ;D
	mut height, weight: u16;	# the height and weight of a person can change, and also can exceed 255kg (not recommended)
}

# Creating an instance of `Person`
imut person: Person = {
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
		return Person{
			name: "",
			age: 0,
			height: 0,
			weight: 0
		};
	}

	# Overload new, for example to create a "newborn", whom has the age 0
	fn ::new(imut name: string, mut height, weight: u16) -> Person {
		return Person{
			name: name,
			age: 0,
			height: height,
			weight: weight
		};
	}

	imut name: string;
	mut age: u8;
	mut height, weight: u16;
}

# Creating a new instance of `Person`
imut person = Person::new();

# Using the overload
imut person = Person::new("Brian", height: 45, weight: 3);
```
