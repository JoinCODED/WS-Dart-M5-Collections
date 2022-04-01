Sets are also a collection type, but there's a fundamental difference between them.

Sets are collections of **unique** values, but lists can contain **duplicate** values.

So how can we declare a set in dart:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt']; // this is a list
var food = {'burger','pizza','pasta'}; // this is a set!
}
```

The only difference in declaration is that we use curly braces instead of square brackets.

And because we don't use square brackets for declaration, we can't also use square brackets to access an item with a given index:

```dart
void main () {
var food = {'burger','pizza','pasta'};
print(food[1]); // this will throw an error
}
```

Instead, we use `.elementAt()` method:

```dart
void main () {
var food = {'burger','pizza','pasta'};
print(food.elementAt(1));
}
```

Output:

```
pizza
```

We can also use the same `add()` method we used with lists:

```dart
void main () {
var food = {'burger','pizza','pasta'};
food.add('pasta');
print(food);
}
```

Output:

```
burger, pizza, pasta
```

Shouldn't we get 2 pastas?, As we said, sets includes only unique values, so it will automatically remove any duplicate element.

To remove an element from a set, we use the `remove()` method:

```dart
void main () {
var food = {'burger','pizza','pasta'};
food.remove('pasta');
print(food);
}
```

Output:

```
burger, pizza
```

And we can also use `first`, `last` and `length` on sets.
