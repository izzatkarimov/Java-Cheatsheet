# ♨ My Java Notes

> My Java Notes - My notes on the key concepts of Java.

## Contents
| Concepts | Notes |
| --- | --- |
| What is Java? | [Click Here!](#anatomy-of-a-java-program) |
| Anatomy of a Java Program | [Click Here!](#anatomy-of-a-java-program) |

## Notes

#### ➡️ _What is Java?_
- Java is a high-level, class-based, object-oriented programming language. James Gosling at Sun Microsystems (now part of Oracle Corporation) designed it, and it was released in 1995. The language was developed with the "Write Once, Run Anywhere" (WORA) philosophy. This principle underscores Java's key feature - platform independence, allowing the same Java program to run on multiple platforms without modifications.

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
    - This code declares the class HelloWorld
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





⬆️ [**Back to Top**](#contents)
