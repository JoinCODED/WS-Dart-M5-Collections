`Set` is also a collection type, but there is a fundamental difference between it and `List`.

`Sets` are collections of **unique** values, but lists can contain **duplicate** values.

We declare a `Set` in Dart as follows:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt']; // this is a list
var food = {'burger','pizza','pasta'}; // this is a `Set`!
}
```

The only difference in the declaration is that we use curly braces around the `Set`'s values instead of square brackets. And because of that, we can't use square brackets as well to access an item with a given index:

```dart
void main () {
var food = {'burger','pizza','pasta'};
print(food[1]); // this will throw an error
}
```

Instead, we use the `.elementAt()` method:

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

Though not all of the `Lists` methods are applicable on `Sets`, some, like `.first`, `.last`, `.length`, and `.add()` are applicable:

```dart
void main () {
var food = {'burger','pizza','pasta'};
food.add('pasta');
print(food);
}
```

Output:

```
{burger, pizza, pasta}
```

In the output above, shouldn't we get two pastas? As we said, `Sets` include unique values, so it will automatically remove any duplicate elements.

Finally, to remove an element from a `Set`, we use the `.remove()` method:

```dart
void main () {
var food = {'burger','pizza','pasta'};
food.remove('pasta');
print(food);
}
```

Output:

```
{burger, pizza}
```
