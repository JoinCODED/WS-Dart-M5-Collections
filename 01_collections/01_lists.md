A collection is a group of values that belongs together.

And in dart, we have 3 types of collections:

1. Lists.
2. Sets.
3. Maps.

In this lesson we will talk about Lists, in other programming languages they are also known as `Arrays`, And they are used to represent a collection of values.

For example, we can declare a list of countries:

```dart
void main () {
    var countries = ['Kuwait','Oman','Egypt'];
    print(countries);
}
```

Output:

```
[Kuwait, Oman, Egypt]
```

We declare a list like any other variable, but we set the values in a square brackets `[]`.

And if we want to print a specific country of this list, we can use the square bracket again with the index of the item that we want:

```dart
void main () {
    var countries = ['Kuwait','Oman','Egypt'];
    print(countries[1]);
}
```

Output:

```
Oman
```

Remember that in programming, if we have a list with the length of `n` we always count from `0` to `n-1`.

We can also change the value of an item with the same operator, for example:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
countries[2] = 'Jordan';
print(countries);
}
```

Output:

```
[Kuwait, Oman, Jordan]
```

We can also iterate over all the items of the list using a `for` loop that we learned before but with a slightly different syntax:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];

for (var country in countries){
    print(country);
}

}
```

Output:

```
Kuwait
Oman
Egypt
```

And we also can use the conventional `for` loop that we used before:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];

for (var i = 0; i < countries.length; i++){
    print(country[i]);
}
}
```

As you see, both ways do the same, but in the conventional `for` loop, we need to manullay update the index, hence we need more code, so for lists, it's better to use `for-in` loops to iterate over the list.
