# C++ Basics

## Introduction to C++

C++ is a powerful and widely used programming language known for its efficiency, flexibility, and performance. It supports both procedural and object-oriented programming paradigms, making it suitable for various applications, including systems programming, game development, and audio programming. 

### Installing a C++ Compiler

Before you start coding in C++, you need a C++ compiler. There are several options available for different platforms:

- For Windows: Visual Studio, MinGW, Cygwin
- For macOS: Xcode Command Line Tools (installed with Xcode) or Homebrew GCC
- For Linux: GCC (usually installed by default)

Choose a compiler suitable for your operating system and install it before proceeding.

## Hello World in C++

Like every language you usually are greeted with a hello world tutorial:

```c++
#include <iostream>

int main(){
std::cout << "Hello World!" << std::endl;
return 0;
}
```
In this method '#include iostream' includes the input/output stream library, allowing us to see the 'std::cout' (console output) and 'std::endl' (newline) statements. The 'main()' function is the entry point of every C++ program. and it returns in integer (usually 0) to the operating system upon successful execution.

## Variables and Data Types

In C++ and pretty much every language youll see variables are used to store and manipulate data. Beofre using a varaible, you must declare its data type. Here are some common data types:

+ int: Integer type (e.g.,24, -17, 12)
+ float: Single-precision floating-point type (e.g., 0.1, 2.34, 17.00)
+ double: Double-precision floating-point type (e.g., 3.14159, -123.456)
+ char: Character type (e.g., 'A', 'B', "@")
+ bool: Boolean type (either 'true' or 'false')

## Variable Declaration And Assignment

Declaring and initializing varaibles in c++ looks like this:

```c++
#include <iostream>

int main() {
	int age = 25;
	float score = 5.12;
	char grade = "C";
	bool isStudent = true;

	std::cout << "Age: " << age << std::endl;
	std::cout << "Score: " << score << std::endl;
	std::cout << "Grade: " << grade << std::endl;
	std::cout << "Is Student: " << isStudent << std::endl;

	return 0;
}
```

## Control Flow

Control flow statements allow you yo control the execution flow of a program. The main control flow statements are:
+ if-else: Executes a block of code conditionally based on a Boolean expression ("if this is true then do this").
+ for: Executes a block of code repeatedly for a specified number of iterations ("for each variable in this variable do something")
+ while: Executes a block of code repeatedly as long as a condition is true. ("while this is true do this")
+ switch: Allows you to select one of many blocks of code to execute based on a variable's value.

## If-Else Statement

The 'if' statement allows us to perform different actions based on a condition:
```c++
#include <iostream>

int main() {
    int age = 18;

    if (age >= 18) {
        std::cout << "You are an adult." << std::endl;
    } else {
        std::cout << "You are a minor." << std::endl;
    }

    return 0;
}

```

## For-Loop

The for loop is used to execute a block of code repeatedly for a specific number of iterations:

```c++
#include <iostream>

int main() {
    for (int i = 1; i <= 5; ++i) {
        std::cout << "Iteration: " << i << std::endl;
    }

    return 0;
}

```

## While Loop

The while loop is used to execute a block of code repeatedly as long as a condition is true:

```c++
#include <iostream>

int main() {
    int count = 1;

    while (count <= 5) {
        std::cout << "Count: " << count << std::endl;
        ++count;
    }

    return 0;
}

```

## Switch Statement

The switch statement allows you to select one of many blocks of code to execute based on a variables value:

```cpp
#include <iostream>

int main() {
    int choice = 2;

    switch (choice) {
        case 1:
            std::cout << "You selected option 1." << std::endl;
            break;
        case 2:
            std::cout << "You selected option 2." << std::endl;
            break;
        case 3:
            std::cout << "You selected option 3." << std::endl;
            break;
        default:
            std::cout << "Invalid option." << std::endl;
            break;
    }

    return 0;
}

```





# Functions

Functions in C++ are blocks of code that can be called and executed at different parts of the program. They allow us to modularize code and improve code readability.

## Function Declaration and Definition

Here's a simple example of a function that adds two numbers and returns the result:

```c++
#include <iostream>

// Function declaration
int add(int a, int b);

int main() {
    int num1 = 5;
    int num2 = 7;
    int sum = add(num1, num2);
    std::cout << "Sum: " << sum << std::endl;

    return 0;
}

// Function definition
int add(int a, int b) {
    return a + b;
}

```



# Classes and Object-Oriented Programming(OOP)

C++ supports object-oriented programming, which allows us to create classes that encapsulate data and behavior's. Here's a basic example of a 'Person' class:

```c++
#include <iostream>
#include <string>

class Person {
public:
    // Constructor
    Person(std::string name, int age) : name(name), age(age) {}

    // Member function
    void displayInfo() {
        std::cout << "Name: " << name << ", Age: " << age << std::endl;
    }

private:
    std::string name;
    int age;
};

int main() {
    // Create an instance of the Person class
    Person person("John Doe", 30);

    // Call the member function
    person.displayInfo();

    return 0;
}

```

## Class Members
+ Constructor: A special member function that initializes class objects. it has the same name as the class and is executed when an object is created.
+ Member Function: Functions defined within a class that operate on class data.  They are called member functions because they belong to the class. 
