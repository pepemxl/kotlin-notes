## Data Types

Each value in Kotlin must have a type.
Some of the most used built-in data types are:
- `Int` indicates an integer (whole number), such as 42.
- `Double` and `Float` are used to store decimal numbers, such as 12.4.
- `Char` represents a character, such as 'z'.
- `Boolean` has two possible values, either true or false.


The String type is used to represent text, such as "Hello World". The text for a String is enclosed in double quotes.
The `\n` character can be used in a string to create a line break.


## Variables


Variables are used to store data. Variables are declared using the `var` keyword.

```kotlin
fun main(args: Array<String>) {
    var num:Int = 1984
    println(num)
}
```

We can also declare variables using the `val` keyword, the difference with var is that variables declared using val cannot be changed.

```kotlin
fun main(args: Array<String>) {
    val num:Int = 1984
    println(num)
    num = 3
}
```
output:
```bash
Val cannot be reassigned
```

## Type Inference

Kotlin supports a useful feature called **type inference**, which allows it to guess the type of the variable from the value it is assigned to.


```kotlin
fun main(args : Array<String>) {
    val name = "Pepe"
    var num = 1984
    println(name)
    println(num)
} 
```

otuput:
```bash
Pepe
1984
```

```kotlin
fun main(args : Array<String>) {
    val name = "Pepe"
    var num = 1984
    println(name)
    println(num)
    num = "1985"
} 
```
output:

```bash
The value '"1985"' assigned to 'var num: Int defined in main' is never used
Type mismatch: inferred type is String but Int was expected
```

## Arithmetic Operators

Kotlin supports all common arithmetic operators:

- `+` for addition
- `-` for subtraction
- `*` for multiplication
- `/` for division
- `%` for modulus

You can use them for variables and values in your code:

```kotlin
fun main(args : Array<String>) {
    val num1 = 2
    var num2 = 3
    println(num1+num2)
    println(num1-num2)
    println(num1*num2)
    println(num1/num2)
    println(num1%num2)
} 
```

output:

```bash
5
-1
6
0
2
```


## Assignment Operators

The assignment operator `=` is used to assign a value to a variable.
Kotlin also supports arithmetic assignment operators:

- `a+=b` equivalent to `a=a+b`
- `a-=b` equivalent to `a=a-b`
- `a*=b` equivalent to `a=a*b`
- `a/=b` equivalent to `a=a/b`


Kotlin also supports the increment `++` and decrement `--` as prefix and postfix operators.

## Comparison Operators


The comparison operators compare two values and return a boolean: true or false.

Here are the comparison operators:

- `>` greater than
- `<` less than
- `>=` greater than or equals to
- `<=` less than or equals to
- `==` is equal to
- `!=` is not equal

## Comments


Comments are explanatory statements used to describe your code.

A single line comment starts with //.

If you need a longer comment that spans multiple lines, you can use multi-line comments. Everything between /* and */ is considered a comment.

