# learn_rust

[[_TOC_]]

# Variable

```rust
// Declaration d'un entier immubale, constante ?
let mut age: i32 = 25;
// Declaration d'un flottant, d'une variable
let temperatur: f64 = 24.5;
// Declaration d'un caractere
let grade : char = 'A';
let keyboard = '⌨';
// Declaration d'un booleen
let is_active : bool = false;
// Déclaration d'un tableau d'entier
let array: [i32; 5] = [0, 1, 2, 3, 4];

// Declaration d'une chaine de catactere
let user_name : String = "Bob123".to_string() ;
// Declaration d'un chaine de caractere
let mut name: &str = "Alice";
// Affiche sur la console
println!("Hello {}!", name);
```

# Control et boucle

# if

```rust
let x = 3;

if x < 10 {
	println!("{} is less than 10", x);
} else {
	println!("{} is greater than or equal to 10", x);
}

```
# loop

```rust
let mut x = 0;

loop{
	x++;

	if x >= 100 {
		println!("{} is now over 100 so we break the loop", x);
		break; // Permet de sortir de la boucle
	}
	
	if x % 3 != 0 {
		continue; // The print statment following this if statement will not be printed
	}

	println!("{} is divisible by 3", x);
}
```
# while

```rust
let mut x = 0;

while x <= 100 {
	x += 1;

	if x % 3 == 0 {
		println!("{} is divisible by 3", x);
	}
}
```

# For-In Loop

```rust
for x in 1..101 {
	if x % 3 == 0 {
		println!("{} is divisible by 3", x);
	}
}
```

# Functions in Rust

```rust
fn main(){
	divisible_by_three_between(1,31);
	println!("The square of 12 is {}", square_num(12));
}

fn divisible_by_three_between(min: i32, max_exclusive: i32) {
	for x in min..max_exclusive {
		if x % 3 == 0 {
			println!("{} is divisible by 3", x);
		}
	}
}

fn square_num(n: i32) -> i32 {
	n * n
}
```

```rust
```
```rust
```
