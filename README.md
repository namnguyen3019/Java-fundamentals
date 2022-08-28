# Java fundamental concept - ISAM 5638

**This repo contains Notes and programs on following topics:**
- Writing for the first Java program
- Data types
- Operators and Statements
- Create a class, fields and methods
- OOP: Inheritance, Abstraction, Encapsulation and Polymorphism
- Interfaces
- Connect to Database
- Handling Exceptions


## 1. Create the first java program
    Let's create a program show "Hello, World"

```java
/*
 * Create a public class name 'HelloWorld'
 * This MUST BE EXACTLY match the name of of the file
 * 'HelloWord.java'
 * One file MUST have only one public class
 */
public class HelloWorld {
    /*
     * main() function is very special function
     * A Java program begins execution with its main() method
     */
    public static void main(String[] args) {
        System.out.println("Hello, World");
    }
}
```
Explanation: The meaning of `public void static` keywords will be explaned later when we create a class.
For now just remember a java program will always start with this `main()` method.

- `String[] args`: the `main` method will take an array of string as its arguments. You can write `String abc[]` or `String... anything` they are the same.

Let's see this code:

```java
   public class HelloWorld {
    public static void main(String[] args) {
        System.out.println(args[0]);
        System.out.println(args[1]);
    }
} 
```
To run it, type:
```java
javac HelloWorld.java
java HelloWorld a b c
```
`javac` will transform our file to bytecodes, while `java HelloWorld a b c` will transform the bytecodes to machine code.

The program will print out:
```java
a
b
```
Because `args` = `['a', 'b', 'c']`. All command-line arguments are treated as String objects.

