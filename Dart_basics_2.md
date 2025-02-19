## Conditional Statements (`if`, `else`, `switch`)

- **Definition**: Conditional statements are used to execute different blocks of code based on specific conditions.
- **Types**:
  - 🎯 `if-else`: Executes code if a condition is met.
  - 🎯 `switch`: Matches a variable with multiple possible values.

### Example:

```dart
// if-else example
int age = 20;
if (age >= 18) {
  print('Adult ✅');
} else {
  print('Minor ❌');
}

// switch example
String color = 'blue';
switch (color) {
  case 'red':
    print('Color is red');
    break;
  case 'blue':
    print('Color is blue');
    break;
  default:
    print('Unknown color');
}
```


## Loops (`for`, `while`, `do-while`)

- **Definition**: Loops allow executing a block of code multiple times.
- **Types**:
  - 🎯 `for` loop: Repeats a block of code for a specific number of times.
  - 🎯 `while` loop: Executes as long as a condition is true.
  - 🎯 `do-while` loop: Runs **at least once**, then checks the condition.

### Example:

```dart
// for loop example
for (int i = 0; i < 5; i++) {
  print('For loop iteration: $i');
}

// while loop example
int counter = 0;
while (counter < 5) {
  print('While loop count: $counter');
  counter++;
}

// do-while loop example
int count = 0;
do {
  print('Do-while loop count: $count');
  count++;
} while (count < 5);
```
