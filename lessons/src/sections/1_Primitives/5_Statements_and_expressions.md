# Statements and Expressions

- An **expression** evaluates to a value.
  `cats > 1_000`
- cats its self is an expression.
- Similary a function call is an exrpress.
  `cats > counts_cats(cat_areas)`
- cats is an expression, so is counts_cats and cats_areas as well as the whole line of code.

- A **statement** does not evaluate to a value.
  `println!("hello");`
- In most cases this will end with a semicolon.

### Why this distinction matters

- In rust so longas you want to return an expression.

```rs
fn multiplier(x:f64,y:f64) -> f64 {
    return x*y
}
```

- You can re-write it like this.

```rs
fn multiplier(x:f64,y:f64) -> f64 {
     x*y
}
```

- If a function ends with an expression it automatically returns that expression.

- If statements also follow the same rule as functions

```rs
let message = if cats > 1 {
    "Multiple cats"
} else {
    "Need More Cats"
}; // let is a statement
```
