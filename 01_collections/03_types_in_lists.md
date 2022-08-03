So far, we declared our list with the `var` keyword:

```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
}
```

And we can set the type explicitly as we did with variables:

```dart
void main () {
List countries = ['Kuwait','Oman','Egypt'];
}
```

Above, we declared the type of `countries` as a `List`. Besides, we can be more specific with the type of items within this `List`:

```dart
void main () {
List<String> countries = ['Kuwait','Oman','Egypt'];
}
```

We can add angular brackets after `List`, and between them, we tell Dart the type of elements allowed in this list.

Furthermore, we can use `final` or `const` in our list declaration, but they behave a bit different.. let's see what this means:

```dart
void main () {
final List<String> countries = ['Kuwait','Oman','Egypt'];
countries = ['UAE'];
}
```

As you see, Dart is complaining that we cannot `re-assign` a `final`. Yet, you may be surprised that you can still `modify` the content of a final list:

```dart
void main () {
final List<String> countries = ['Kuwait','Oman','Egypt'];
countries[2] = 'UAE';
}
```

However, for `const`, you cannot `re-assign` nor `modify` the list.
