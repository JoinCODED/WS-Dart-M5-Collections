The last type of collections is `Maps`, aka `dictionaries` or `objects` in other programming languages.

A `Map` is used to store a collection of `key-value` pairs.

For example, we have the following `key-value` pairs:

```
name: Salem
age: 26
height: 1.78
```

To define a `Map` in Dart with those `key-value` pairs above, we need to place them inside curly brackets like the example below:

```dart
void main () {
    var person = {
        'name': 'Salem',
        'age': 26,
        'height': 1.78
    };
}
```

Keys in Dart should always be unique, and in the example above, all keys are of type string, while the values are in mixed types.

To explicitly tell Dart what type of keys and values this map has:
Within angular brackets after the `Map` keyword, we write the keys type followed by a comma, followed by the type of the values. In our case, keys are strings and the values are dynamic because they might be int, double, or a string.

```dart
void main () {
    Map<String, dynamic> person = {
        'name': 'Salem',
        'age': 26,
        'height': 1.78
    };
}
```

To access a value within this map, we can use the square brackets:

```dart
void main () {
    Map<String, dynamic> person = {
        'name': 'Salem',
        'age': 26,
        'height': 1.78
    };

    print(person['name']);
}
```

Output:

```
Salem
```

Same way to set a value for a specific key:

```dart
void main () {
    Map<String, dynamic> person = {
        'name': 'Salem',
        'age': 26,
        'height': 1.78
    };
    person['age'] = 40;
    print(person);
}
```

Output:

```
{name: Salem, age: 40, height: 1.84}
```

We can also add new keys and values to our map:

```dart
void main () {
    Map<String, dynamic> person = {
        'name': 'Salem',
        'age': 40,
        'height': 1.78
    };
    person['married'] = false;
    print(person);
}
```

Output:

```
{name: Salem, age: 40, height: 1.84, married: false}
```

**Note:** when you add new `key-value` pairs, the map will check if the key you added already exists. If so, it will replace that key's value with the one you added, otherwise it's going to add it as a new `key-value` pair.
