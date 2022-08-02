Let's take a look at this code:

```dart
void main() {
    Map<String, dynamic> person = {
        'name': 'Salem',
        'age': 26,
        'height': 1.78
    };
    var name = person['name'];
    print(name);
}
```

What do you think the type of the variable `name` is? Is it `String` because the `key` is a `String`? Or is it `dynamic` because the type of the value is `dynamic`?

At compile time, Dart doesn't know what the `name`'s type is. Therefore, we can assist it here and tell it what type of `as` operator we want to use:

```dart
void main() {
    Map<String, dynamic> person = {
        'name': 'Salem',
        'age': 26,
        'height': 1.78
    };
    var name = person['name'] as String;
    print(name);
}
```
