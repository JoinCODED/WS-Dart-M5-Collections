Let's learn some basic operations and methods that we can use with lists:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
}
```

Our first method is used to check the number of items in our list:

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

Another useful method is the `.isEmpty` method that checks if the list is empty or `isNotEmpty` to check for the opposite:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
print(countries.isEmpty);
print(countries.isNotEmpty);
}
```

Output:

```
false
true
```

We also have `.first` and `.last` methods to get the first or the last element of a list:

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

So far, we learned how to access and item of the list, but how to add an item to the list?

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
countries.add('Jordan');
print(countries);
}
```

Output:

```
Kuwait, Oman, Egypt, Jordan
```

We can use the `.add()` method to add a new item at the **end** of the list. and to add an item to a specific position we use `.insert()` method:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
countries.insert(1,'Jordan');
print(countries);
}
```

Output:

```
Kuwait, Jordan, Oman, Egypt
```

`.insert()` takes two arguments: the index where you want to insert the item, and the item itself.

To remove an item. we use the `removeAt()` method and we provide it with the index of the item that we want to remove:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
countries.removeAt(1);
print(countries);
}
```

Output:

```
Kuwait, Egypt
```

Next, let's learn how to find a certain item within a list using a method that we used before on strings:

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

But what if I need the index of `Kuwait`, we can use the `indexOf()` method:

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
