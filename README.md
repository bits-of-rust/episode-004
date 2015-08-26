# episode-004
Where we bind a variables

## Setup
We need to prepare

* A project called `variables`
* A `println!` call with an argument

## Script
Variables our a way to reuse certain values in your program. We start from the a familiar `println!` expression.

```rust
println!("Hello, {}!", "world");
```

If we would also want to say `Goodbye, world!`, this could be achieved by adding the following line.

```rust
println!("Goodbye, {}!", "world");
```

But what if we would want to say hello and goodbye to the moon? We would have to change the argument to the two `println!`.

```rust
println!("Hello, {}!", "moon");
println!("Goodbye, {}!", "moon");
```

Which seem wasteful. Let's see how a variable can help in this situation.

With `let` we can introduces a variable `subject` with the value `world`, that is used as an argument in the `println!` call.

```rust
let subject = "world";

println!("Hello, {}!", subject);
println!("Goodbye, {}!", subject);
```

Saying goodbye to moon can be achieved by changing the `subject` to `moon`.

```rust
let subject = "moon";
```

And there you have it, we bound a variable.


