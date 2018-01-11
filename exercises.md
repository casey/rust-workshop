Hello, World!
-------------

Write a program that prints "Hello, World!".

You'll need to use the `println` macro:
https://doc.rust-lang.org/beta/std/macro.println.html

Function signature:

```
fn hello() {
  // insert code here!
}
```


FizzBuzz
--------

Write a program that prints the numbers from 1 to 100. But for multiples of three print “Fizz” instead of the number and for the multiples of five print “Buzz”. For numbers which are multiples of both three and five print “FizzBuzz”.

Function signature:

```
fn fizz_buzz() {
  // insert code here!
}
```


Fibonacci
---------

Write a function that calculates the nth fibonacci number.

| n | fib(n)                  |
|---|-------------------------|
| 0 | 0                       |
| 1 | 1                       |
| n | fib(n - 1) + fib(n - 2) |

Function signature:

```
fn fib(n: u64) -> u64 {
  // insert code here!
}
```


Counting
--------

Count the occurrences of an integer in a slice of integers.

Function signature:

```
fn count(haystack: &[i32], needle: i32) -> isize {
  // insert code here!
}
```


Concatination
-------------

Write a function that takes two slices and returns a vec containing the contents of those two slices concatenated together.

Function signature:

```
fn concatinate(a: &[i32], b: &[i32]) -> Vec<i32> {
  // insert code here!
}
```


Digits
------

Write a function that returns the base 10 digits of a number. For example, when given the number "527", it should return a vector containing the characters `5`, `2`, and `7`. Note the order!

Function signature:

```
fn digits(n: ) -> Vec<char> {
  // insert code here!
}
```


Hello IO
--------

Read a name from standard input and print out a greeting using that name. This is going to be rough, given Rust's explicit error handling.

You can transform a `Result`, which might be an error, into the value it contains using the `unwrap` method. This will cause the program to panic if the `Result` is indeed an error.

Use `std::io::stdin()` to get a handle to standard input, and `read_line()` on that handle to read a line into a string:

https://doc.rust-lang.org/beta/std/io/fn.stdin.html

https://doc.rust-lang.org/beta/std/io/struct.Stdin.html#method.read_line

Transcript:

```
Please enter a name:  # from program
Bob                   # typed by user
Hello, Bob!           # from program
```
