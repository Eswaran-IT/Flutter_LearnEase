# What is Dart? 🚀

- **Definition**:  
  Dart is a **programming language** used to build mobile, desktop, server, and web applications. It is the primary language for developing **Flutter** apps. Dart is:
  - ✅ **Object-Oriented**
  - ✅ **Strongly Typed**
  - Supports **asynchronous programming** with **async/await**, making it ideal for building **fast** and **efficient** applications.

- **Nature of Dart**:  
  - 🎯 **Compiled Language**: Dart code is converted into native machine code, resulting in high performance.  
  - 🎯 **Cross-Platform**: Dart allows you to build apps for **Android**, **iOS**, **Web**, and **Desktop**.  
  - ✅ **Garbage Collected**: Dart manages memory automatically, avoiding memory leaks.
  - 🚀 **Modern Features**:
    - **Async/Await** for handling asynchronous tasks
    - **Null Safety** to avoid issues with null values
    - A **rich standard library** for everyday tasks


### 1️⃣ Entry Point (`main()` function) 🏁
- **Definition**: The `main()` function is where the Dart program starts.
- **Example**:

```dart
void main() {
  print('Hello, Dart!'); // Starting point of your program
}

```

### 2️⃣ Variables and Data Types 💡

- **Definition**:  
  Variables store data. Dart supports the following types:
  - ✅ `int`: Whole numbers 
  - ✅ `double`: Decimal numbers 
  - ✅ `String`: Textual data 
  - ✅ `bool`: True or false 
  - ✅ `List`: Ordered collection 
  - ✅ `Map`: Key-value pairs 

---

#### 1. **Integer (`int`)**

- **Create**: Declare and assign an integer value.
- **Read**: Access the value.
- **Update**: Modify the value.
- **Delete**: Remove or set to null.

```dart
int age = 25;  // Create
print(age);  // Read

age = 30;  // Update
print(age);

age = 0;  // Delete (set to zero)
print(age);
```

---

### 2️⃣ **Double (`double`)**

- **Definition**: Numbers with decimal points (e.g., 5.9, 3.14).
- **Example**:

```dart
double height = 5.9;  // Create
print(height);  // Read

height = 6.1;  // Update
print(height);

height = 0.0;  // Delete (set to zero)
print(height);

```

---

### 3️⃣ **String (`String`)**

- **Definition**: A sequence of characters, used to represent text.
- **Example**:

```dart
String name = 'Flutter Developer';  // Create
print(name);  // Read

name = 'Dart Developer';  // Update
print(name);

name = '';  // Delete (set to empty string)
print(name);

```

---

### 4️⃣ **Boolean (`bool`)**

- **Definition**: Represents a value of either `true` or `false`.
- **Example**:

```dart
bool isActive = true;  // Create
print(isActive);  // Read

isActive = false;  // Update
print(isActive);

isActive = null;  // Delete (nullable)
print(isActive);
```


---

### 5️⃣ **List (`List`)**

- **Definition**: An ordered collection of items, often of the same type.
- **Example**:

```dart
List<int> numbers = [1, 2, 3, 4];  // Create
print(numbers);  // Read

numbers[0] = 10;  // Update
print(numbers);

numbers.removeAt(2);  // Delete (remove element at index 2)
print(numbers);
```


---

### 6️⃣ **Map (`Map`)**

- **Definition**: A collection of key-value pairs.
- **Example**:

```dart
Map<String, String> user = {'name': 'John', 'email': 'john@example.com'};  // Create
print(user);  // Read

user['name'] = 'Jane';  // Update
print(user);

user.remove('email');  // Delete (remove key-value pair)
print(user);

```

---

### 7️⃣ **Dynamic (`dynamic`)**

- **Definition**: A special type that can hold any data type. It’s flexible but should be used cautiously since it doesn’t provide compile-time type checks.
- **Example**:

```dart
dynamic value = 'Hello, Dart!';  // Create
print(value);  // Read

value = 10;  // Update to an integer
print(value);

value = true;  // Update to a boolean
print(value);

value = null;  // Delete (nullable)
print(value);

```


---

### 8️⃣ **Late (`late`)**

- **Definition**: Used to delay the initialization of a variable. It tells Dart to assume the variable will be initialized before it's used, even if it’s declared but not assigned a value immediately.
- **Example**:

```dart
late String name;  // Declare without initializing

name = 'Dart';  // Initialize later
print(name);  // Read

name = 'Flutter';  // Update
print(name);
```

---

---

### 9️⃣ **Nullable Types**

- **Definition**: Dart’s null safety feature allows you to declare variables that can hold `null`. By default, all types are non-nullable unless you use the `?` operator.
- **Example**:

```dart
String? nullableString = null;  // Nullable
print(nullableString);  // Read

nullableString = 'Dart is awesome';  // Update
print(nullableString);

```
### 🔟 **Constant (`const`)**

- **Definition**: Declares a constant value that cannot be changed. The value must be known at compile-time.
- **Example**:

```dart
const pi = 3.14;  // Create constant
print(pi);  // Read

// pi = 3.14159;  // This would throw an error because 'pi' is a constant.

```
---

### 1️⃣1️⃣ **Final (`final`)**

- **Definition**: Similar to `const`, but the value can be assigned only once during runtime. It does not require compile-time evaluation.
- **Example**:

```dart
final dateTime = DateTime.now();  // Create
print(dateTime);  // Read

// dateTime = DateTime.now();  // This would throw an error because 'dateTime' is final.
```
