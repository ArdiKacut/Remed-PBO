```dart
void main() {
  
  // Aritmatika
  int a = 5;
  int b = 3;
  int sum = a + b;
  print('Sum of $a and $b is $sum');

  // List 
  List<int> numbers = [1, 2, 3, 4, 5];
  print('List: $numbers');

  // Percabangan
  if (sum > 5) {
    print('Sum is greater than 5');
  } else {
    print('Sum is 5 or less');
  }

  // Perulangan
  for (int i = 0; i < numbers.length; i++) {
    print('Number at index $i is ${numbers[i]}');
  }

  // Function parameter dan return value
  int multiply(int x, int y) {
    return x * y;
  }

  int product = multiply(a, b);
  print('Product of $a and $b is $product');

  // Anonymous function
  var add = (int x, int y) => x + y;
  int result = add(a, b);
  print('Result of anonymous function add: $result');

  // Closure
  Function makeAdder(int addBy) {
    return (int i) => addBy + i;
  }

  var add2 = makeAdder(2);
  var add3 = makeAdder(3);

  print('Add 2 to 3 using closure: ${add2(3)}'); // 5
  print('Add 3 to 3 using closure: ${add3(3)}'); // 6
}
```