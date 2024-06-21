# ♨ My Java Notes

> My Java Notes - My notes on the key concepts of Java.

## Contents
| Concepts | Notes |
| --- | --- |
| What is Java? | [Click Here!](#%EF%B8%8F-what-is-java) |
| Hello World! | [Click Here!](#%EF%B8%8F-hello-world) |
| Literals in Java | [Click Here!](##%EF%B8%8F-literals-in-java) |
| Printing Data | [Click Here!](#%EF%B8%8F-printing-data) |
| Variables | [Click Here!](#%EF%B8%8F-variables) |
| Reading Input with Scanner | [Click Here!](#%EF%B8%8F-reading-input-with-scanner) |
| Coding Style Conventions | [Click Here!](#%EF%B8%8F-coding-style-conventions) |
| Arithmatic Operations | [Click Here!](#%EF%B8%8F-arithmatic-operations) |
| Booleans | [Click Here!](#%EF%B8%8F-booleans) |
| Relational Operators (Comparing Values) | [Click Here!](#%EF%B8%8F-relational-operators-comparing-values) |
| Conditional Statement | [Click Here!](#%EF%B8%8F-conditional-statement) |
| Ternary Conditional Operator | [Click Here!](#%EF%B8%8F-ternary-conditional-operator) |
| Java Program | [Click Here!](#) |

## Notes

## ➡️ _What is Java?_
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

## ➡️ _Hello World!_
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

## ➡️ _Literals in Java_
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
## ➡️ _Printing Data_
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
## ➡️ _Variables_
### Declaring and Initializing a Variable
In programming, a variable is a placeholder for storing a value of a particular type: a string, a number, or something else.
Every variable has a name (also known as an identifier) to distinguish it from others. Before you start using a variable, you must declare it. The general form of declaration is the following:
```
DataType variableName = initialization;
```
According to this declaration, we can declare the following variables of different types:
```
String language = "Java";
String dayOfWeek = "Monday";
int numberOfApples = 5;
int age = 22;
```
One important feature of variables is that they can be changed. You don't need to declare a variable again to change its value; just assign a new value to it using the = operator.

Let's declare a variable named dayOfWeek and print its value before and after changing:
```
String dayOfWeek = "Monday";
System.out.println(dayOfWeek); // Monday

dayOfWeek = "Tuesday";
System.out.println(dayOfWeek); // Tuesday
```
There is one restriction for variables: you can only assign a value of the same type as the type of the initial variable. So, the following code is not correct:
```
int number = 10;
number = 11; // ok
number = "twelve"; // it does not work!
```
### Type Inference
Since Java 10, you can write var instead of a specific type to force automatic type inference based on the type of assigned value:
```
var language = "Java"; // String
var version = 10; // int
```
> This feature can be a bit controversial: on the one hand, it allows your code to be more concise. On the other hand, since it doesn't indicate the type explicitly, it may affect the code readability in a bad way. For now, it's enough to understand the basic idea. We will not use type inference in our theory so that our educational platform is suitable for people who use earlier versions of Java. But if you would like to practice it, you may use type inference in our exercises as they fully support Java 10.

### Naming Variables
Java has some rules for naming varibles:
- names are case-sensitive
- a name can inclue Unicode letters, digits, and two special characters ($, _);
- a name cannot start with a digit;
- a name must not be a keyword (class, static, int, etc. are illegal names).
Based on these rules, you may conclude that whitespaces are not allowed in the name of a variable. 
It is important not to break these rules; otherwise, the program will not work

Here are some valid names of variables:
```
number, $ident, bigValue, _val, abc, k, var
```

### Naming Conventions for Variables
Also, there are the following conventions for naming variables:
- if a variable name is a single word it should be in lowercase (for instance: number, price);
- if a variable name includes multiple words it should be in lowerCamelCase, i.e. the first word should be in lowercase and each word after the first should have its first letter written in uppercase (for instance: numberOfCoins);
- variable names should not start with _ and $ characters, although they are allowed;
- choose a name that makes sense, e.g. score makes more sense than s, although they are both valid.

## ➡️ _Reading Input with Scanner_
The simplest method to obtain data from the standard input is using the standard class Scanner. It allows a program to read values of various types, like strings or numbers, from the standard input. To use this class:
1. You should add the following import statement at the top of your file with the source code.
```
import java.util.Scanner;
```
2. After the import, add a class with this construction:
```
public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
    }
}
```
3. In the main method, we make an object of Scanner class, which allows us to use its methods. System.in signals that the program will read the text that you entered in the standard input. You'll need this line exactly as it is for now.
The Scanner class offers two ways to read strings. If your input is an integer number or a single word, you can use the next() method. For example, the following code snippet reads the user's name and prints a hello message:
```
public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String name = scanner.next();
        System.out.println("Hello, " + name + "!");
    }
}
```
For example, if the user enters their name as James, the program's output will be:
```
Hello, James!
```
If you enter an integer number like 123 as the user's input, the program will output this number. Remember that the next() method will store 123 or some other integer number as a string, even if we know that this string represents a number.
```
Hello, 123!
```
Now, what if a user inputs a compound name like Erich Maria? The program will only output the first word:
```
Hello, Erich!
```
In this case, you'll need to invoke the next() method again:
```public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String firstName = scanner.next(); // "Erich"
        String lastName = scanner.next(); // "Maria"
        System.out.println("Hello, " + firstName + " " + lastName  + "!");
    }
}
```
4. nextLine()
It would be more efficient to use another method, the nextLine() method, which reads and outputs the entire line:
```
Hello, Erich Maria!
```
### Reading a Multiline Input
Let's explore this topic with an example:
```
|This is a simple

multiline input,

that is being read
```
If we call the next() method, the program will read the input up to the whitespace:
```
This| is a simple

multiline input,

that is being read
```
After invoking the nextLine() method, the program reads the remaining line starting from the whitespace. If there is such a line in your input, the nextLine() places the cursor at the start of the new line:
```
This is a simple

|multiline input,

that is being read
```
Here's a tricky thing about the nextLine() method, which also shows a major difference between next() and nextLine() methods. As you know already, the program will read input from the cursor's position to the new line (again, if such a line exists in your input). In this example, the cursor is placed before the new line. This means the nextLine() method will return an empty line ("") and place the cursor at the start of a new line.
```
Before:
This is a simple

multiline input,|

that is being read

After:
This is a simple

multiline input,

|that is being read
```
To sum it all up, let's look at the entire code and consider what variables we've just read:
```
import java.util.Scanner; 

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);  

        String word1 = scanner.next(); // "This"
        String line1 = scanner.nextLine(); // " is a simple" 
        String word2 = scanner.next(); // "multiline"
        String word3 = scanner.next(); // "input,"
        String line2 = scanner.nextLine(); // "" 
    }
}
```
## ➡️ _Coding Style Conventions_
> Good coding style is like correct punctuation: you can manage without it, butitsuremakesthingseasiertoread. – The Tidyverse Style Guide by Hadley Wickham

In most cases, companies and individual developers do not create their own style conventions. There are two generally accepted Java conventions that are used all over the world:
Oracle Code Conventions
Google Style Guide
Sometimes they could be modified or extended by a particular company to meet their needs.
Now let's look at some of the most basic Java conventions according to the Oracle Code Conventions.
### The number of Spaces
The first convention is to use 4 spaces as the unit of indentation in the whole program code. You have already seen our code examples before and you might note that we used this value there.
Good:
```
public class NumberOfSpacesExample {

    public static void main(String[] args) {
        System.out.println("Hi!");
        System.out.println("I'm a Java program.");
    }
}
```
Ver Bad:
```
public class NumberOfSpacesExample {

   public static void main(String[] args) {
         System.out.println("Hi!");
System.out.println("I'm a Java program.");
 }
  }
```
Sometimes tabulation is used to create an indentation. However, tab may correspond to 8 spaces instead of 4 in some IDEs, hence this note.
### The location of curly braces
1. Put the opening curly brace at the end of the line where the block begins.
2.Put the closing curly brace at the beginning of the next line.
```
public class NumberOfSpacesExample {

    public static void main(String[] args) {
        System.out.println("Hi!");
        System.out.println("I'm a Java program.");
    }
}
```
### The length of a line
The last recommendation concerns the maximum length of a line. The Oracle Code Conventions propose avoiding lines longer than 80 characters. Plenty of developers consider this restriction as outdated since modern monitors can easily display longer lines, whereas others would go on following this rule, which is handy, for example, if laptops are used. Keeping ourselves off this dispute, we will use 80 characters in the course to avoid scrollbars in our examples and web code editor. We recommend that you do the same while learning here, but keep in mind that you can violate this limitation after you start working on a real project or learning elsewhere. Other popular limit values are 100, 120, and sometimes even 140 characters.

## ➡️ _Arithmatic Operations_
### Binary Arithmatic Operators:
- addition +
- subtraction -
- multiplication *
- division /
- remainder %
These operators are called binary because they take two values as operands.
The following example prints the results of addition, subtraction, and multiplication.
```
System.out.println(13 + 25); // prints 38
System.out.println(20 + 70); // prints 90

System.out.println(70 - 30); // prints 40
System.out.println(30 - 70); // prints -40

System.out.println(21 * 3);  // prints 63
System.out.println(20 * 10); // prints 200
```
The / operator returns the integer part of the division of two integer numbers, and any fractional part is discarded.
```
System.out.println(8 / 3); // prints 2
System.out.println(41 / 5); // prints 8
```
The % in Java is the modulus or remainder operator. It returns the remainder of the division of two numbers. Note, that when the dividend is less than the divisor, the quotient is zero and the remainder equals the dividend.
```
System.out.println(10 % 3); // prints 1, because 10 divided by 3 leaves a remainder of 1
System.out.println(12 % 4); // prints 0, because 12 divided by 4 leaves no remainder
System.out.println(5 % 9); // prints 5, because 5 divided by 9 leaves a remainder of 5
```
### Unary Operators
In Java, a unary operator is an operator that performs an operation on a single operand, unlike binary operators that require two operands.
The unary plus operator indicates a positive value. It's an optional operator.
```
System.out.println(+5); // prints 5
```
The unary minus operator negates a value or an expression.
```
System.out.println(-8);  // prints -8
System.out.println(-(100 + 4)); // prints -104
```
### The precedence order
There is a precedence order of all arithmetic operators, including parentheses. The list below is sorted from the highest to the lowest precedence level.
1. Parantheses
2. Unary Plus / Minus
3. Multiplication, division, the remainder
4. addition, subtraction

## ➡️ _Booleans_
[!Note]
> You cannot assign an integer value to a boolean. In Java, 0 is not the same as false.

### Logical Operators
Variables of the boolean type are often used to build logical expressions using logical operators. Java has four logical operators: NOT, AND, OR, and XOR.
- NOT
  NOT is a unary operator that reverses the boolean value. It is denoted as !.
  ```
  boolean f = false; // f is false
  boolean t = !f;    // t is true
  ```
- AND
  AND is a binary operator that returns true if both operands are true, otherwise, it returns false. It is denoted as &&.
  ```
  boolean b1 = false && false; // false
  boolean b2 = false && true;  // false
  boolean b3 = true && false;  // false
  boolean b4 = true && true;   // true
  ```
- OR
  OR is a binary operator that returns true if at least one operand is true, otherwise, it returns false. It is denoted as ||.
  ```
  boolean b1 = false || false; // false
  boolean b2 = false || true;  // true
  boolean b3 = true || false;  // true
  boolean b4 = true || true;   // true
  ```
- XOR (exclusive OR)
  XOR (exclusive OR) is a binary operator that returns true if boolean operands have different values, otherwise, it returns false. It is denoted as ^.
  ```
  boolean b1 = false ^ false; // false
  boolean b2 = false ^ true;  // true
  boolean b3 = true ^ false;  // true
  boolean b4 = true ^ true;   // false
  ```
  The XOR operator is used less often than the others. Just remember that Java has it. If you really need it, you can use it.

### The precedence of Logical Operators
Logical Operators in decreasing priority:
1. NOT
2. XOR
3. AND
4. OR
The following variable is true:
```
boolean b = true && !false; // true, because !false is evaluated before &&
```

## ➡️ _Relational Operators (Comparing Values)_
![Screenshot 2024-06-21 at 12 27 47 PM](https://github.com/izzatkarimov/MyJavaNotes/assets/108251704/44ddcedd-01d9-4bb3-ab0a-2bdec60eafd3)

In Java, you cannot write an expression like a <= b <= c. Instead, you should join two boolean expressions using logical operators like || and &&. Here is an example:
```
number > 100 && number < 200; // it means 100 < number < 200
```

## ➡️ _Conditional Statement_
The single if case:
```
if (expression) {
    // body: do something
}
```
The if > else cases:
```
if (expression) {    
    // do something
} else {
    // do something else
}
```
For example:
```
int num = ...; // the num is initialized by some value

if (num % 2 == 0) {
    System.out.println("It's an even number");
} else {    
    System.out.println("It's an odd number");
}
```
The if > else if cases:
```
if (expression0) {
    // do something
} else if (expression1) {
    // do something else 1
// ...
} else if (expressionN) {
    // do something else N
}
```

## ➡️ _Ternary Conditional Operator_
The general syntax of the ternary operator is the following:
```
result = condition ? trueCase : elseCase;
```
Here, the condition is a Boolean expression that evaluates to either true or false. If this expression is true, the ternary operator evaluates trueCase, otherwise elseCase is evaluated. It is important that trueCase and elseCase are expressions which can be reduced to a common type.

Example:
Imagine you need to compare two integer numbers and print equal in case they are equal, more if the first one has a bigger value than the second and less otherwise. The task can be solved using a combination of 2 ternary operators:
```
int a = ...; // it's initialized by a value
int b = ...; // it's initialized by a value
String result = a == b ? "equal" :
                a > b ? "more" : "less";
```

----
⬆️ [**Back to Top**](#contents)
