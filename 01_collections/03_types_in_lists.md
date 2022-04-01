```dart
void main () {
var countries = ['Kuwait','Oman','Egypt'];
}
```

So far, we declared our list with the `var` keyword, and we can write the type explicitly like we did with variables:

```dart
void main () {
List countries = ['Kuwait','Oman','Egypt'];
}
```

Above, we declared the type of `countries` as a `List`, but we can be more specific with the type of the items withing this `List`:

```dart
void main () {
List<String> countries = ['Kuwait','Oman','Egypt'];
}
```

We can add angular brackets after `List` and within them, we tell dart what type of elements is allowed in this list of items.

Also, we can use `final` and `const` in our list declaration, but it behaves a bit different.. let's see what I mean:

```dart
void main () {
final List<String> countries = ['Kuwait','Oman','Egypt'];
countries = ['UAE'];
}
```

As you see, dart is complaining that we can't `re-assign` a `final`. but it may surprise you that:

```dart
void main () {
final List<String> countries = ['Kuwait','Oman','Egypt'];
countries[2] = 'UAE';
}
```

You can still `modify` the content of a final list but you can't `re-assign` it.

But for `const`, you can't `re-assign` nor `modify` the list.
