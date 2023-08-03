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

Control flow statements allow you to control the execution flow of a program. The main control flow statements are:
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






# C++ Symbols And Their Uses

## Assignment Operator (=)

+ **Use:** the assignment operator (=) us used to assign a value to a variable.
+ **Example:** 'int x = 5;'
### Equality Operator (`==`)

- **Use**: The equality operator (`==`)is used to check if two values are equal.
- **Example**: `if (x == 5) { /* do something */ }`

### Addition Operator (+)

- **Use**: The addition operator (+) is used to perform addition between numerical values.
- **Example**: `int sum = a + b;`

### Increment Operator (++)

- **Use**: The increment operator (++) is used to increase the value of a variable by 1.
- **Example**: `x++; // Equivalent to x = x + 1;`

### Compound Assignment Operator (+=)

- **Use**: The compound assignment operator (+=) is used to add a value to a variable and assign the result to the same variable.
- **Example**: `x += 5; // Equivalent to x = x + 5;`

### Multiplication Operator (`*`)

- **Use**: The multiplication operator (`*`) is used to perform multiplication between numerical values.
- **Example**: `int product = a * b;`

### Pointer (`*`) and Reference (&)

- **Use**: Pointers and references are used to store memory addresses of variables, allowing manipulation of data indirectly.
- **Example (Pointer): `int* ptr = &x; // Pointer to integer x`  
    Example (Reference): `int& ref = x; // Reference to integer x`
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


# C++ Data-Sets

Data sets in C++ are collections of values or objects that are grouped together and stored in memory. These data structures allow us to organize, manipulate, and access data efficiently. In this section, we'll cover some common data sets in C++ and their practical uses.

### 1. Arrays

Arrays are a collection of elements of the same type, stored in contiguous memory locations. The size of an array is fixed at compile time, and each element is accessed by its index, starting from 0.

**Example:**

```cpp
`#include <iostream>  int main() {     int numbers[5] = {1, 2, 3, 4, 5};      for (int i = 0; i < 5; ++i) {         std::cout << numbers[i] << " ";     }      return 0; }`
```

**Common Uses:**

- Storing and processing a fixed number of elements efficiently.
- Used in algorithms and operations that require sequential access to elements.


## 2. Vectors

Vectors are dynamic arrays athat can resize themselves automatically. they are part of the Standard Template Library(STL) and offer a wide range of built-in functions for easy manipulation.

**Example:**

```cpp
#include <iostream>
#include <vector>

int main() {
	std::vector<int> numbers = {1, 2, 3, 4, 5};

	for (const int&num : numbers) {
		std::cout << num << " ";
	}

	return 0;
}
```

**Common Uses:**

+ When the number of elements is not known at compile time and needs to grow or shrink during runtime.
+ used frequently when dealing with dynamic collections of data.


## 3. Linked Lists

Linked lists are data structures consisting of a series of nodes, where each node contains data and a pointer / reference to the next node in the sequence.

**Example:**

```cpp
#include <iostream>

struct Node{
	int data;
	Node* next;
};

int main() {
	Node* head = new Node{1, nullptr};
	head->next = new Node{2, nullptr};
	head->next->next = new Node{3, nullptr};

	Node* current = head;
	while (current != nullptr) {
		std::cout << current->data << " ";
		current = current->next;
	}

	return 0
}
```

**Common Uses:**

+ When elements need to be inserted or removed frequently from a collection.
+ Used in implementing other data structures like stack and queues.


## 4. Maps

Maps, also known as associative arrays or dictionaries, store key-value pairs. Each key is unique, and accessing values is done using the corresponding keys.

**Examples:**

```cpp
#include <iostream>
#include <map>

int main() {
	std::map<stdLLstring, int> ages;
	ages["Alice"] = 25;
	ages["Bob"] = 30;
	ages["Charlie"] = 22;
	std::cout << "Bob's age: " << ages["Bob"] << std::endl;

	return 0;
}
```

**Common Uses:**

+ Efficiently accessing and manipulating data using a unique key.
+ Used in various applications like symbol tables and frequency counting.

## 5. Sets

Sets are containers that store unique elements in a sorted order. It does not allow duplicate entries.

**Examples:**

```cpp
#include <iostream>
#include <set>

int main() {
	std::set<int> uniqueNumbers = {4, 2, 1, 3, 2, 5, 1}

	for (const int& num : uniqueNumbers) {
		std::cout << num << " ";
	}

	return 0;
}
```

**Common Uses:**

+ Maintaining a collection of unique elements.
+ Used in solving problems related to finding distinct elements or removing duplicates

## 6.Stack

A stack is a Last-In-First-Out(LIFO) data structure, meaning the last element inserted is the first to be removed.

**Example:**

```cpp
#include <iostream>
#include <stack>

int main() {
	std::stack<int> numbers;
	numbers.push(1);
	numbers.push(2);
	numbers.push(3);

	while (!numbers.empty()) {
		std::cout << numbers.top() << " ";
		numbers.pop();
	}

	return 0;
}
```

**Common Uses:**

+ Used in recursive algorithms and parsing expressions.
+ Used for tracking backtracking operations and function calls.

## 7. Queue

A queue is a First-In-First-Out(FIFO) data structure, meaning the first element inserted in is the first to be removed.

**Example:**

```cpp
#include <iostream>
#include <queue>

int main() {
	std::queue<int> numbers;
	numbers.push(1);
	numbers.push(2);
	numbers.push(3);

	while (!numbers.empty()) {
		std::cout << numbers.front() << " ";
		numbers.pop();
	}

	return 0;
}
```

**Common Uses:**

+ Used in scheduling tasks, simulations, and breadth-first search algorithms.
+ Handles tasks in the order they are added.

## 8. Priority Queue

A priority queue is a queue in which each element has an associated priority, and elements with higher priority are served before elements with lower priority.

**Example:**

```cpp
#include <iostream>
#include <queue>

int main() {
	std::priority_queue<int> pq;
	pq.push(3);
	pq.push(1);
	pq.push(2);
	
	while (!pq.empty()) {
		std::cout << pq.top() << " ";
		pq.pop();
	}

	return 0;
}
```

**Common Uses:**

+ used in various applications where tasks need to be processed based on priority, like Dijkstra's algorithm.