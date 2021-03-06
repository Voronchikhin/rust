# Luhn: Using a Custom Trait

Before doing this exercise you should probably do the original Luhn exercise and its successor, "Luhn: Using the From Trait"

To get the original Luhn exercise, run

```shell
exercism download --exercise=luhn --track=rust
```

To get the "Luhn: Using the From Trait" exercise, run

```shell
exercism download --exercise=luhn-from --track=rust
```

In the original Luhn exercise you only validated strings, but the Luhn algorithm can be applied to integers as well.

In "Luhn: Using the From Trait" you implemented a From trait, which also required you to create a Luhn struct.

Instead of creating a Struct just to perform the validation, what if you you validated the primitives (i.e, String, u8, etc.) themselves?

In this exercise you'll create and implement a custom [trait](https://doc.rust-lang.org/book/second-edition/ch10-02-traits.html) that performs the validation.

Note: It is [not idiomatic Rust to implement traits on on primitives](https://doc.rust-lang.org/book/second-edition/ch10-02-traits.html#implementing-a-trait-on-a-type). In this exercise we're showing something that you _can_ do, not something you _should_ do. If you find yourself implementing traits on primitives, perhaps you have a case of [Primitive Obsession](http://wiki.c2.com/?PrimitiveObsession).
