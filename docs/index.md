class: center, middle

<img src="img/rust-logo.svg" height="400px">

---

class: center, middle

## Ask questions!

---

## Agenda

- Setup
- Why Rust?
- Why not Rust?
- Tricky bits
- Resources
- Let's code!

---

## Setup

- Get Rust using Rustup:  
  https://www.rustup.rs

- Make sure `cargo --version` works

- Cheat sheet:
  ```
cargo init --bin DIRECTORY   # create a new binary project
cargo init --lib DiRECTORY   # create a new library project
cargo build                  # build the project
cargo test                   # run unit tests
cargo run                    # run the main binary
```

- Can also use rust playground:  
  https://play.rust-lang.org

---

class: center, middle

## Why Rust?

---

## Why Rust?

### Memory safety without garbage collection

---

## Why Rust?

### Garbage collected languages are inefficient

- Power hungry, bad for mobile

- Expensive at scale

- Bad for resource-constrained environments

---

## Why Rust?

### C and C++ are not good enough

- Insecure, even at the expert level
- C++ is a garbage heap of poorly-interacting features

---

## Why Rust?

### Excellent interoperability with C and C++

- FFI between C and Rust is easy
- Interoperability means that there is an upgrade path!

---

## Why Rust?

### Powerful and ergonomic language features

- Enums and pattern matching
- Iterators
- Hygienic macro system (like Lisp, not C)
- Move semantics
- Good take on object-oriented programming

---

## Why Rust?

### Language design prevents many bugs

- Explicitly sized types (`u8`, `i32`, `f32`, etcetera)

- No problematic implicit conversions

- Explicit error handling

---

## Why Rust?

### Best build system and package manager in the world!

- Excellent dependency management

- Very easy to publish libraries and binaries for others to use

- Statically linked binaries so deploying is easy

---

## Why Rust?

### Excellent community

- IRC and subreddit are full of friendly, nice, *smart* people

---

class: center, middle

## Why not Rust?

---

## Why not Rust?

- Explicit error handling is verbose

- Type system makes many fine distinctions
  - `String` vs `CString` vs `OSString`

- Borrow and lifetime checker can reject valid programs

---

## Tricky bits

- Mutability
  - Variables are immutable by default
  - [example](https://play.rust-lang.org/?gist=2b11a692d4941fb3472bd4f5e92d68a2&version=stable)

- Move semantics  
  - Values can be efficiently "consumed"
  - [example](https://play.rust-lang.org/?gist=ac8e9de26377836be14b83b77baf5daf&version=stable)

- Ownership  
  - Distinction between "I own this value." and "Someone else owns this value."
  - [example](https://play.rust-lang.org/?gist=52de079ae848caa55f041cba7de9b1df&version=stable)

- Lifetimes
  - Annotations to allow the compiler to make sure you are using memory safely
  - [example](https://play.rust-lang.org/?gist=7b7e047966f262d3bd111325de25b25f&version=stable)

---

## Resources

- Rustup, the Rust toolchain installer:  
  https://www.rustup.rs

- The Rust Playground:  
  https://play.rust-lang.org

- The Rust Book:  
  https://doc.rust-lang.org/book/second-edition

- /r/rust:  
  https://www.reddit.com/r/rust

- Rust community links:  
  https://www.rust-lang.org/en-US/community.html

- IRC Cloud:  
  https://www.irccloud.com

- These slides:  
  https://github.com/casey/rust-workshop

---

class: center, middle

## Let's code!

---

## Let's code!

- Rust can be brutally difficult. Don't worry if it takes a lot of effort to understand something.

- im here for you bb <3
