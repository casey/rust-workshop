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
fn digits(n: u64) -> Vec<char> {
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


Go Forth
--------

Write a postfix notation arithmetic interpreter. It should take a string of space-separated numbers and arithmetic operators, and return the result of evaluating them as a postfix notation expression.

For example:

```
$ 1 2 +
3
$ 3 7 *
21
$ 8 2 /
4
$ 10 11 8 * * 2 /
440
```

You'll need to use a Vec as a stack.

You should print a discriptive error if input is malformed.


Go Forther
----------

Extend the interpreter in the previous exercise with additional functionality:

- An equality testing operator, `=`, that returns 1 if the top two items of the stack are equal, and 0 if not:

```
$ 1 1 =
1
$ 1 2 =
0
```

- A modulus operator, `%`, that returns the second from the top item on the stack modulo the top item on the stack:

```
$ 10 5 %
0
$ 1 2 %
1
$ 7 3 %
1
```


Go Forthest
-----------

Extend the interpreter in the previous exercise with additional functionality:

- Conditional execution, with `IF <A> ELSE <B> THEN`. If the top item of the stack is 1, execute the operations between IF and ELSE, else execute the operations between ELSE and THEN.

```
$ 1 IF 10 ELSE 20 THEN
10
$ 0 IF 10 ELSE 20 THEN
20
```

- Functions. A function is defined with `: NAME <BODY> ;`. After the function definition, a reference to `NAME` executes the operations between `NAME` and `;`:

```
$ : EVEN 2 % 0 = ; 10 EVEN
1
```

Go Fortheseter
--------------

Write `fib` in the interpreter you wrote in the previous exercise.
