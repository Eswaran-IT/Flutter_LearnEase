### 1️⃣ Entry Point (`main()` function) 🏁
- **Definition**: The `main()` function is where the Dart program starts.
- **Example**:

```dart
void main() {
  print('Hello, Dart!'); // Starting point of your program
}

```

### 2️⃣ Variables and Data Types 💡

- **Definition**: Variables store data. Dart supports types like int, double, String, bool, List, and Map.
  - `int`: Whole numbers 
  - `double`: Decimal numbers 
  - `String`: Textual data 
  - `bool`: True or false 
  - `List`: Ordered collection 
  - `Map`: Key-value pairs 
- **Example**:

```dart
var name = 'Flutter Developer'; // String
int age = 25; // Integer
double height = 5.9; // Double
bool isActive = true; // Boolean
List<int> numbers = [1, 2, 3, 4]; // List of integers
Map<String, String> user = {'name': 'John', 'email': 'john@example.com'}; // Map

```

### 3️⃣ Conditional Statements ⚖️

- **Definition**: Used to make decisions based on conditions.
  - `if-else`: Executes code if the condition is true or false.
- **Example**:

```dart
int age = 20;

if (age >= 18) {
  print('Adult ✅');
} else {
  print('Minor ❌');
}

```

### 4️⃣ Loops 🔄

- **Definition**: Repeats a block of code multiple times.
  - `for` loop: Loop for a specific number of times 🔁
  - `while` loop: Loop until a condition is false 🔂
- **Example**:

```dart
// For loop
for (int i = 0; i < 5; i++) {
  print('Loop $i');
}

// While loop
int counter = 0;
while (counter < 5) {
  print('Counter: $counter');
  counter++;
}

```


### 5️⃣ Functions 🛠️

- **Definition**: Reusable block of code to perform a specific task. Functions can accept parameters and return results.
- **Example**:

```dart
int add(int a, int b) {
  return a + b;
}
print(add(3, 4)); // Output: 7

```

### 6️⃣ Arrow Functions (Short Functions) ➡️


- **Definition**: A more concise way to write functions.
- **Example**:

```dart
var multiply = (int a, int b) => a * b;
print(multiply(4, 5)); // Output: 20

```

### 7️⃣ Classes and Objects 🏫


- **Definition**: A class is a blueprint for creating objects. It defines properties and methods.
- **Example**:

```dart
class Person {
  String name;
  int age;

  Person(this.name, this.age); // Constructor

  void greet() {
    print('Hello, $name! You are $age years old.');
  }
}

var person = Person('Alice', 30);
person.greet(); // Output: Hello, Alice! You are 30 years old.

```

### 8️⃣ Null Safety 🚫

- **Definition**: Ensures variables can't hold null unless explicitly allowed by `?`.
- **Example**:

```dart
String? nullableString = null; // Nullable String
nullableString = 'Hello, Dart!'; // Now it holds a value
print(nullableString); // Output: Hello, Dart!
```
