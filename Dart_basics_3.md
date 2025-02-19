## Classes and Objects 🏛️

- **Definition**:  
  A **class** is a **blueprint** for creating objects. It defines properties (**variables**) and behaviors (**functions/methods**).  
  An **object** is an **instance** of a class, meaning it's created from a class.

- **Why use classes?**  
  ✅ Helps **organize code** better.  
  ✅ Allows **code reuse** (same structure for multiple objects).  
  ✅ Makes **big projects easy to manage**.

### Example:

```dart
class Person {
  String name;
  int age;

  // Constructor
  Person(this.name, this.age);

  // Method (Function inside a class)
  void greet() {
    print('Hello, my name is $name and I am $age years old.');
  }
}

// Creating an object
void main() {
  Person p1 = Person('Alice', 25);
  p1.greet();  // Output: Hello, my name is Alice and I am 25 years old.
}
```

## Functions in Dart ⚙️

- **Definition**:  
  A function is a **block of code** that does a specific task.  
  Instead of writing the same code **again and again**, we write it once inside a function and **reuse it**.

- **Why use functions?**  
  ✅ Makes code **clean and reusable**.  
  ✅ Helps **avoid repetition**.  
  ✅ Easier to **debug and manage**.

### Example:

```dart
// Function without parameters
void sayHello() {
  print('Hello, Dart!');
}

// Function with parameters
int add(int a, int b) {
  return a + b;
}

// Calling functions
void main() {
  sayHello();  // Output: Hello, Dart!
  print(add(5, 3));  // Output: 8
}

```
## Async and Await ⏳ (Handling Asynchronous Code)

- **Definition**:  
  Dart is **single-threaded**, meaning it runs **one task at a time**.  
  But some tasks, like **downloading data from the internet**, take time.  
  Instead of **waiting and blocking everything**, Dart uses **async** and **await** to **continue running other code** while waiting.

- **Why use async/await?**  
  ✅ Prevents **program from freezing** while waiting.  
  ✅ Helps **handle time-consuming tasks smoothly**.  
  ✅ Makes **code readable and easy to manage**.

### Example:

```dart
// Simulating a delayed task
Future<String> fetchData() async {
  await Future.delayed(Duration(seconds: 2)); // Simulates a delay
  return 'Data loaded';
}
void main() async {
  print('Fetching data...');
  String data = await fetchData();  // Waits for the result
  print(data);  // Output after 2 seconds: Data loaded
}
```


---

### Summary 📝  
- **Classes and Objects**: Used to create **blueprints** for reusable code.  
- **Functions**: Blocks of code that do **specific tasks** and can be **reused**.  
- **Async/Await**: Used to handle **time-consuming tasks** **without freezing** the program.  

---

