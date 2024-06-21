# ♨ My Java Notes

> My Java Notes - My notes on the key concepts of Java.

## Contents
| Concepts | Notes |
| --- | --- |
| What is Java? | [Click Here!](#anatomy-of-a-java-program) |
| Anatomy of a Java Program | [Click Here!](#anatomy-of-a-java-program) |

## Notes

#### ➡️ _What is Java?_
Java is a high-level, class-based, object-oriented programming language. James Gosling at Sun Microsystems (now part of Oracle Corporation) designed it, and it was released in 1995. The language was developed with the "Write Once, Run Anywhere" (WORA) philosophy. This principle underscores Java's key feature - platform independence, allowing the same Java program to run on multiple platforms without modifications.

Java is designed to be both simple and powerful. It borrows its syntax from C and C++, but eliminates certain low-level programming complexities, such as explicit memory management and multiple inheritance found in C++. Known for its robustness, security, and simplicity, Java has become a popular choice among developers worldwide.
- Characteristics of Java:
    - High Level Language
    - Object-Oriented
    - Platform-Independent
    - Compiled and Interpreted
    - Strongly Typed
    - Automatic Memory Management
    - Concurrent
    - Robust and Secure

#### ➡️ _Hello World!_
```
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```
- `public class HelloWorld`:
    - It is the basic unit of a program. Every Java program must have at least one class. The definition of a class consists of the class keyword followed by the class name. A class can have any name, such as App, Main, or Program, but it must not start with a digit. A set of braces {...} encloses the body of a class.
    - This code declares the class HelloWorld.
    - `public` - Access Modifier. This indicates that this class is accessible from any other class. 
    - `class` - This is a special keyword in Java and is used to create a class.
    - `HelloWorld` - This is the name of the class. By convention, class names in Java should start with an uppercase letter.
- `public static void main(String[] args)`:
    - This code declares the main method
    - `public` - Access Modifier. This indicates that the method `main` is accessible from any other class.
    - `static` - This is a special keyword in Java. This keyword means that the method belongs to the class rather than an instance of the class. This means that only one instance of a static member exists, even if you create multiple objects of the class, or if you don't create any. It will be shared by all object This allows the Java runtime to call this method without creating an instance of the class. 
    - `void` - This means that the method does not return any value.
    - `main`- This is the name of the method. The main method is special because it is the entry point of any Java application.
    - `String[] args` - This is a parameter of the main method. It represents an array of String objects.
- `System.out.println("Hello, World!")`:
    - This code prints to the console
    - `println` - This is a method of the PrintStream class. It prints the argument passed to it (in this case, "Hello, World!") to the console, followed by a newline.

#### ➡️ _Literals in Java_
- What are literals (to begin with)?
> Consider literals as groceries. To use them, usually you need to store them somewhere. Typically, they are stored in variables, which you can think of as containers designed to hold a specific type of data. Variables can only store matching data. You wouldn't want to accidentally put honey in a cardboard cereal box or pour cereal into a salt shaker. To prevent such mistakes, learn to distinguish between the basic literals: integer numbers, strings, and characters.
- Integers
  - Examples: 0, 1, 2, 10, 11, -100
  - Example in Code: int numApples = 1000;
  - Example in Code with better readability: int numPackedApples = 1_000_000;
- Characters
  - Definition: A character is a single symbol, denoted with single quotes. You can use character literals to represent single letters like 'A', 'x', digits from '0' to '9', whitespaces (' '), and other characters or symbols like '$'.
  - Example: char charOne = '1'
  - Fun fact: characters sit between integers and strings: they resemble strings, yet you can do math with them.
- Strings
  - Examples: "text", "I want to know Java", "123456", "e-mail@gmail.com"
  - Note the difference:
    ```
    char singleQuoted = 'A'
    String doubleQuoted = "A"
    ```
#### ➡️ _Printing Data_
- println() vs print():
  - println()
    - The println method displays the passed string followed by a new line on the screen (print-line). For example, the following code snippet prints four lines:
        ```
        System.out.println("I ");
        System.out.println("know ");
        System.out.println("Java ");
        System.out.println("well.");
        ```
        Output:
        ```
        I
        know
        Java
        well.
        ```
  - print()
    - The print method displays the value that was passed in and places the cursor (the position where we display a value) after it. For example, the code below outputs all strings in a single line:
        ```
        System.out.print("I ");
        System.out.print("know ");
        System.out.print("Java ");
        System.out.print("well.");
        ```
        Output:
        ```
        I know Java well.
        ```
----
⬆️ [**Back to Top**](#contents)
