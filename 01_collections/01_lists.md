In this lesson, we will talk about **Lists**, which are also known as `Arrays` in other programming languages, and they are used to represent a collection of values.

For example, we can declare a list of countries as follows:

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

Declaring a list is like any other variable. However, the list's values must be placed within square brackets `[]`.

To print a specific country of this list, we can place the index of that country inside square brackets:

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

In the same way, we can change the value of an item, for example:

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

Remember that in programming, if we have a list with the length of `n`, we always count from `0` to `n-1` as shown below:

['Kuwait','Oman','Egypt']
&nbsp;&nbsp;&nbsp;&nbsp;↑ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ↑ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ↑
&nbsp;&nbsp;&nbsp;&nbsp;0 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2

We can iterate over all the items of the list using a `for` loop that we learned before, but with a slightly different syntax:

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

At the same time, we can use the conventional `for` loop that we used before:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];

for (var i = 0; i < countries.length; i++){
    print(countries[i]);
}
}
```

As you see, both approaches achieve the same goal, but in the conventional `for` loop, we need to manually update the index, hence we need more code. For lists, it's better to use `for-in` loops to iterate over the list.
