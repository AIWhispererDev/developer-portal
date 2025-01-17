# Boolean

## Summary

- Boolean is a primitive data type in Move representing true or false values
- Essential for implementing logic and controlling program flow
- Declared using the bool type (e.g., `let a: bool = true`)
- Used in conditional statements and loops
- Can be printed and tested in Move modules
- Fundamental for effective programming and robust application development in Move

## Overview

Boolean types in Move are a primitive data type that represent two possible values: true and false. They are essential for implementing logic in your programs, allowing you to control the flow of execution based on conditions.

## Introduction

In programming, Boolean types are used to represent truth values. They are fundamental in decision-making processes, enabling conditional statements and loops.

## Declaring Boolean Variables

You can declare Boolean variables using the bool type. Here’s how to do it:

```rust
let a: bool = true;   // Declaration of a Boolean variable with value true
let b: bool = false;  // Declaration of a Boolean variable with value false
```

## Example Code

Here’s the complete example demonstrating the declaration, usage, and testing of Boolean types in Move:

```rust
module movement::boolean_type {
    use std::debug::print;

    fun bool_types() {
        let a: bool = true;
        let b: bool = false;
        print(&a);  // Outputs: true
        print(&b);  // Outputs: false
    }

    #[test]
    fun test_bool_types() {
        bool_types();  // Calls the bool_types function to test its output
    }
}
```

> Run test on terminal
> 

```ruby
movement move test --filter boolean_type
```

```json
Running Move unit tests
[debug] true
[debug] false
[ PASS ] 0xdb8a45e0e06d2bd305cdb824fda101cec6a24721cb03188c5543a5e5a8c3f3b0::MovementModule::test_bool_types
Test result: OK. Total tests: 1; passed: 1; failed: 0
{
  "Result": "Success"
}

```

## Conclusion

Boolean types are a fundamental aspect of programming in Move, enabling developers to implement logic and control flow effectively. Understanding how to declare, use, and test Boolean types will enhance your programming skills and improve your ability to write robust Move applications.

> Read more [here](https://hack.movementlabs.xyz/ch04-01-primitive-types.html)
>