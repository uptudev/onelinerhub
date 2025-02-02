# How do I get the name of a variable in Rust?
// plain

You can get the name of a variable in Rust by using the `std::stringify` macro. This function takes any valid Rust variable (or any other valid Rust code) and returns a `&'static str` containing the stringification of any tokens passed to it. If passed a variable by name, it will stringify the name.

## Example code

```rust
let x = 5;
let var_name = stringify!(x);
println!("Name of x is {}", var_name);
```

## Output example

```
Name of x is x
```

## Code explanation

- `let x = 5;`: This declares a variable `x` with the value `5`.
- `let var_name = stringify!(x);`: This uses the `std::stringify` macro to get the name of the variable `x` by changing the Rust token of `x` into `"x"`.
- `println!("Name of x is {}", type_name);`: This prints the name of the variable `x` to the console.

## Helpful links
- [std::stringify](https://doc.rust-lang.org/std/macro.stringify.html)

group: rust-variables
