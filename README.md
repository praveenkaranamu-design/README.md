# Dart Programming Language

## Dart Modules
1. [Introduction and Basics](#1-introduction-and-basics)
2. [Conditions and Loops](#2-conditions-and-loops)
3. [Functions in Dart](#3-functions-in-dart)
4. [Collections in Dart](#4-collections-in-dart)
5. [File Handling in Dart](#5-file-handling-in-dart)
6. [OOP in Dart](#6-oop-in-dart)

## 1. Introduction and Basics
Dart is a programming language developed by Google. It is mainly used for building mobile apps (Android & iOS), web apps, desktop apps, and especially Flutter applications. Dart is object-oriented, easy to learn, and supports both ahead-of-time (AOT) and just-in-time (JIT) compilation, making it fast and efficient for UI development.

### 10 Examples of Dart Basics

#### Example 1: Print Hello World
```dart
void main() {
  print("Hello, Dart!");
}
```
**Output:**
```
Hello, Dart!
```
#### Example 2: Variables and Data Types
```dart
void main() {
  int age = 21;
  double height = 5.9;
  String name = "Praveen";
  bool isStudent = true;

  print("Name: $name, Age: $age, Height: $height, Student: $isStudent");
}
```
**Output:**
```
Name: Praveen, Age: 21, Height: 5.9, Student: true
```
### Example 3: Arithmetic Operations
```dart
void main() {
  int a = 10;
  int b = 3;
  print("Addition: ${a + b}");
  print("Subtraction: ${a - b}");
  print("Multiplication: ${a * b}");
  print("Division: ${a / b}");
}
```
**Output:**
```
Addition: 13
Subtraction: 7
Multiplication: 30
Division: 3.3333333333333335
```
### Example 4: String Concatenation
```dart
void main() {
  String first = "Hello";
  String second = "World";
  print(first + " " + second);
}
```
**Output:**
```
Hello World
```
### Example 5: Using Constants and Final
```dart
void main() {
  const pi = 3.14;
  final today = DateTime.now();
  print("Pi: $pi, Today: $today");
}
```
**Output:**
```
Pi: 3.14, Today: 2025-10-30 11:00:00.000
```
### Example 6: Type Conversion
```dart
void main() {
  int num = 10;
  String str = num.toString();
  print("Converted number to string: $str");
}
```
**Output:**
```
Converted number to string: 10
```
### Example 7: Comments in Dart
```dart
void main() {
  // This is a single-line comment
  /* This is a multi-line comment */
  print("Comments are ignored by the compiler!");
}
```
**Output:**
```
Comments are ignored by the compiler!
```
### Example 8: Input from User (works in console)
```dart
import 'dart:io';
void main() {
  stdout.write("Enter your name: ");
  String? name = stdin.readLineSync();
  print("Hello, $name!");
}
```
**Output:**
```
Enter your name: Praveen
Hello, Praveen!
```
### Example 9: Null Safety Example
```dart
void main() {
  String? name;
  name = "Dart Learner";
  print(name);
}
```
**Output:**
```
Dart Learner
```
### Example 10: Code Units Example
```dart
void main() {
  String str = "Hi";
  print(str.codeUnits);
}
```
**Output:**
```
[72, 105]
```
## 2. Conditions and Loops

### Overview
Conditions and loops are fundamental concepts in programming used to control the flow of a program.

### 10 Examples of Conditions and Loops

### Example 1: If Statement
```dart
void main() {
  int num = 10;
  if (num > 5) {
    print("Number is greater than 5");
  }
}
```
**Output**
```
Number is greater than 5
```
### Example 2: If-Else
```dart
void main() {
  int num = 3;
  if (num % 2 == 0)
    print("Even");
  else
    print("Odd");
}
```
**Output:**
```
Odd
```
### Example 3: Else-If Ladder
```dart
void main() {
  int marks = 85;
  if (marks >= 90)
    print("A Grade");
  else if (marks >= 75)
    print("B Grade");
  else
    print("C Grade");
}
```
**Output:**
```
B Grade
```
### Example 4: Nested If
```dart
void main() {
  int a = 10, b = 20;
  if (a != b) {
    if (a < b) print("a is smaller");
  }
}
```
**Output:**
```
a is smaller
```
### Example 5: For Loop
```dart
void main() {
  for (int i = 1; i <= 5; i++) {
    print("Number $i");
  }
}
```
**Output:**
```
Number 1
Number 2
Number 3
Number 4
Number 5
```
### Example 6: While Loop
```dart
void main() {
  int i = 1;
  while (i <= 3) {
    print(i);
    i++;
  }
}
```
**Output:**
```
1
2
3
```
### Example 7: Do-While Loop
```dart
void main() {
  int i = 1;
  do {
    print(i);
    i++;
  } while (i <= 3);
}
```
**Output:**
```
1
2
3
```
### Example 8: Break Statement
```dart
void main() {
  for (int i = 1; i <= 5; i++) {
    if (i == 3) break;
    print(i);
  }
}
```
**Output:**
```
1
2
```
### Example 9: Continue Statement
```dart
void main() {
  for (int i = 1; i <= 5; i++) {
    if (i == 3) continue;
    print(i);
  }
}
```
**Output:**
```
1
2
4
5
```
### Example 10: Largest Number
```dart
void main() {
  int num1 = 1200, num2 = 1000, num3 = 150;
  if (num1 > num2 && num1 > num3)
    print("Num1 is greatest: $num1");
  else if (num2 > num3)
    print("Num2 is greatest: $num2");
  else
    print("Num3 is greatest: $num3");
}
```
**Output:**
```
Num1 is greatest: 1200
```
## 3. Functions in Dart

### Overview
Functions in Dart are blocks of code that perform a specific task. You write a function once, and you can use (call) it multiple times in your program. Functions help you organize code, reduce repetition, and improve readability.

### Why We Use Functions
- **Reuse Code**
- **Break complex problems into small parts**
- **Improve code structure**
- **Make debugging easier**

### 10 Examples of Functions in Dart

### Example 1: Simple Function
```dart
void greet() {
  print("Hello from function!");
}
void main() {
  greet();
}
```
**Output:**
```
Hello from function!
```
### Example 2: Function with Parameter
```dart
void printName(String name) {
  print("Hello $name");
}
void main() {
  printName("Praveen");
}
```
**Output:**
```
Hello Praveen
```
### Example 3: Function with Return Type
```dart
int add(int a, int b) {
  return a + b;
}
void main() {
  print(add(5, 3));
}
```
**Output:**
```
8
```
### Example 4: Arrow Function
```dart
int multiply(int a, int b) => a * b;
void main() => print(multiply(2, 3));
```
**Output:**
```
6
```
### Example 5: Optional Positional Parameter
```dart
void greet([String name = "User"]) {
  print("Hello $name");
}
void main() => greet();
```
**Output:**
```
Hello User
```
### Example 6: Named Parameter
```dart
void display({required String name, int age = 0}) {
  print("Name: $name, Age: $age");
}
void main() => display(name: "Praveen", age: 22);
```
**Output:**
```
Name: Praveen, Age: 22
```
### Example 7: Anonymous Function
```dart
void main() {
  var list = [1, 2, 3];
  list.forEach((n) => print(n));
}
```
**Output:**
```
1
2
3
```
### Example 8: Recursive Function (Factorial)
```dart
int factorial(int n) => (n <= 1) ? 1 : n * factorial(n - 1);
void main() => print(factorial(5));
```
**Output:**
```
120
```
### Example 9: Function Returning Function
```dart
Function greetMaker(String message) {
  return () => print(message);
}
void main() {
  var greeter = greetMaker("Hi!");
  greeter();
}
```
**Output:**
```
Hi!
```
### Example 10: Function as Parameter
```dart
void execute(Function action) {
  action();
}
void main() => execute(() => print("Running function inside function!"));
```
**Output:**
```
Running function inside function!
```
## 4. Collections in Dart

### Overview
Collections in Dart are data structures that hold multiple values. Dart provides several built-in collection types: List, Set, Map, and Queue.

 - **List – Ordered collection of items**
 - **Set – Unordered collection of unique items**
 - **Map – Collection of key-value pairs**

### 10 Examples of Collections in Dart

### Example 1: List Example
```dart
void main() {
  var fruits = ["Apple", "Banana", "Mango"];
  print(fruits);
}
```
**Output:**
```
[Apple, Banana, Mango]
```
### Example 2: Add Item to List
```dart
void main() {
  var numbers = [1, 2, 3];
  numbers.add(4);
  print(numbers);
}
```
**Output:**
```
[1, 2, 3, 4]
```
### Example 3: ForEach Loop on List
```dart
void main() {
  var colors = ["Red", "Green", "Blue"];
  colors.forEach((color) => print(color));
}
```
**Output:**
```
Red
Green
Blue
```
### Example 4: Set Example (No Duplicates)
```dart
void main() {
  var uniqueNums = {1, 2, 2, 3};
  print(uniqueNums);
}
```
**Output:**
```
{1, 2, 3}
```
### Example 5: Map Example
```dart
void main() {
  var student = {'name': 'Praveen', 'age': 22};
  print(student);
}
```
**Output:**
```
{name: Praveen, age: 22}
```
### Example 6: Access Map Value
```dart
void main() {
  var user = {'name': 'Alex', 'city': 'Delhi'};
  print(user['city']);
}
```
**Output:**
```
Delhi
```
### Example 7: Add to Map
```dart
void main() {
  var details = {'Name': 'Sam'};
  details['Age'] = 20;
  print(details);
}
```
**Output:**
```
{Name: Sam, Age: 20}
```
### // Example 8: List of Maps
```dart
void main() {
  var students = [
    {'name': 'A', 'age': 18},
    {'name': 'B', 'age': 20},
  ];
  print(students[1]['name']);
}
```
**Output:**
```
B
```
### Example 9: Using List Methods
```dart
void main() {
  var nums = [10, 20, 30];
  nums.remove(20);
  print(nums);
}
```
**Output:**
```
[10, 30]
```
### Example 10: Set Operations
```dart
void main() {
  var a = {1, 2, 3};
  var b = {3, 4, 5};
  print(a.union(b));
  print(a.intersection(b));
}
```
**Output:**
```
{1, 2, 3, 4, 5}
{3}
```
## 5. File Handling in Dart

### Overview
File handling in Dart allows you to read from and write to files on the local filesystem. Dart provides the `dart:io` library for file operations, which includes classes like `File`, `Directory`, and `FileSystemEntity`.

### Key Concepts
- **File**: Represents a file on the filesystem
- **Directory**: Represents a directory on the filesystem
- **FileSystemEntity**: Base class for both files and directories
- **Path operations**: Working with file and directory paths
- **Asynchronous operations**: Most file operations are asynchronous

### 10 Examples of File Handling in Dart

#### Example 1: Write to File
```dart
void main() {
  File('output.txt').writeAsStringSync('Hello Dart File!');
}
```
**Output:**
```
(output.txt created with content "Hello Dart File!")
```
### Example 2: Read from File
```dart
void main() {
  String data = File('output.txt').readAsStringSync();
  print(data);
}
```
**Output:**
```
Hello Dart File!
```
### Example 3: Append to File
```dart
void main() {
  File('output.txt').writeAsStringSync('\nNew Line', mode: FileMode.append);
}
```
**Output:**
```
(Appends "New Line" at the end of output.txt)
```
### Example 4: Check if File Exists
```dart
void main() {
  var file = File('output.txt');
  print(file.existsSync());
}
```
**Output:**
```
true
```
### Example 5: Delete File
```dart
void main() {
  File('temp.txt').deleteSync();
}
```
**Output:**
```
(temp.txt deleted successfully)
```
### Example 6: Create a New File
```dart
void main() {
  File('newfile.txt').createSync();
}
```
**Output:**
```
(newfile.txt created)
```
### Example 7: Read Lines
```dart
void main() {
  var lines = File('output.txt').readAsLinesSync();
  print(lines);
}
```
**Output:**
```
[Hello Dart File!, New Line]
```
### Example 8: Directory List
```dart
void main() {
  Directory.current.listSync().forEach((f) => print(f.path));
}
```
**Output:**
```
/home/user/output.txt
/home/user/newfile.txt
```
### Example 9: Create Directory
```dart
void main() {
  Directory('testDir').createSync();
}
```
**Output:**
```
(Directory "testDir" created)
```
### Example 10: Delete Directory
```dart
void main() {
  Directory('testDir').deleteSync();
}
```
**Output:**
```
(Directory "testDir" deleted)
```

## 6. OOP in Dart

### Overview
Object-Oriented Programming (OOP) in Dart is built around classes and objects. Dart supports all major OOP concepts including encapsulation, inheritance, polymorphism, and abstraction.

### Key Concepts
- **Class**: Blueprint for creating objects
- **Object**: Instance of a class
- **Constructor**: Special method for initializing objects
- **Inheritance**: Creating new classes based on existing ones
- **Polymorphism**: Same interface, different implementations
- **Encapsulation**: Hiding internal implementation details
- **Abstract Classes**: Classes that cannot be instantiated
- **Interfaces**: Contracts that classes must implement

### 10 Examples of OOP in Dart

### Example 1: Simple Class and Object
```dart
class Person {
  String name = "Praveen";
  void show() => print("Hello $name");
}
void main() => Person().show();
```
**Output:**
```
Hello Praveen
```
### Example 2: Constructor Example
```dart
class Student {
  String name;
  Student(this.name);
}
void main() => print(Student("John").name);
```
**Output:**
```
John
```
### Example 3: Named Constructor
```dart
class Car {
  String brand;
  Car.named(this.brand);
}
void main() => print(Car.named("Tesla").brand);
```
**Output:**
```
Tesla
```
### Example 4: Inheritance
```dart
class Animal {
  void sound() => print("Animal sound");
}
class Dog extends Animal {
  void bark() => print("Dog barks");
}
void main() {
  var d = Dog();
  d.sound();
  d.bark();
}
```
**Output:**
```
Animal sound
Dog barks
```
### Example 5: Method Overriding
```dart
class Parent {
  void greet() => print("Hello from Parent");
}
class Child extends Parent {
  @override
  void greet() => print("Hello from Child");
}
void main() => Child().greet();
```
**Output:**
```
Hello from Child
```
### Example 6: Abstract Class
```dart
abstract class Shape {
  void draw();
}
class Circle extends Shape {
  void draw() => print("Drawing Circle");
}
void main() => Circle().draw();
```
**Output:**
```
Drawing Circle
```
### Example 7: Getters and Setters
```dart
class Rectangle {
  double _width = 0;
  set width(double w) => _width = w;
  double get area => _width * 2;
}
void main() {
  var r = Rectangle();
  r.width = 5;
  print(r.area);
}
```
**Output:**
```
10.0
```
### Example 8: Static Members
```dart
class MathUtil {
  static double pi = 3.14;
  static double area(double r) => pi * r * r;
}
void main() => print(MathUtil.area(5));
```
**Output:**
```
78.5
```
### Example 9: Interface Implementation
```dart
class Printer {
  void printData() {}
}
class Epson implements Printer {
  void printData() => print("Printing...");
}
void main() => Epson().printData();
```
**Output:**
```
Printing...
```
### Example 10: Encapsulation Example
```dart
class Account {
  double _balance = 0;
  void deposit(double amt) => _balance += amt;
  double get balance => _balance;
}
void main() {
  var acc = Account();
  acc.deposit(1000);
  print("Balance: ${acc.balance}");
}
```
**Output:**
```
Balance: 1000.0
```







































