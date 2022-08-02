Let's learn some basic operations and methods that we can apply to `Lists`.

Assume that we have the following list:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
}
```

The first method is `.length`, and is used to check the number of items in the list:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
print(countries.length);
}
```

Output:

```
3
```

Another useful method is `.isEmpty`, which checks if the list is empty. And `isNotEmpty`, to check for the opposite:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
print(countries.isNotEmpty);
print(countries.isEmpty);
}
```

Output:

```
true
false
```

We also have `.first` and `.last` methods that are used to get the first or the last element of the list:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
print(countries.first);
print(countries.last);
}
```

Output:

```
Kuwait
Egypt
```

So far, we learned how to access an item in the list, but how to add an item to the list?

We have several options for adding a new item, depending on where we want it placed:

The first option is the `.add()` method, which is used to add a new item at the **end** of the list:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
countries.add('Jordan');
print(countries);
}
```

Output:

```
[Kuwait, Oman, Egypt, Jordan]
```

The second option is the `.insert()` method, which is used to insert an item to a specific position. `.insert()` takes two arguments: the index where you want to insert the item, and the item itself:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
countries.insert(1,'Jordan');
print(countries);
}
```

Output:

```
[Kuwait, Jordan, Oman, Egypt]
```

In order to remove an item from a `List`, we use the `removeAt()` method and we provide it with the index of the item that we want to remove:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
countries.removeAt(1);
print(countries);
}
```

Output:

```
[Kuwait, Egypt]
```

Next, let's learn how to find a certain item within the list using a method that we used before on strings which is `.contains`:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
print(countries.contains("Kuwait"));
}
```

Output:

```
true
```

Finally, we can use the `indexOf()` method to get the index of a specific item:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
print(countries.indexOf("Kuwait"));
}
```

Output:

```
0
```
