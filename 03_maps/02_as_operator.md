Let's take a look at this code:

```dart
void main() {
    Map<String, dynamic> person = {
        'name': 'salem',
        'age': 26,
        'height': 1.78
    };
    var name = person['name'];
    print(name);
}
```

What do you think is the type of the variable `name`? is it a `String` because the `key` is a `String`? or is it `dynamic` because the type of the value is `dynamic`?

At compile time, dart doesn't know what type of `name` is, so we can assist dart here and tell it what type do we want here using the `as` operator:

```dart
void main() {
    Map<String, dynamic> person = {
        'name': 'salem',
        'age': 26,
        'height': 1.78
    };
    var name = person['name'] as String;
    print(name);
}
```
